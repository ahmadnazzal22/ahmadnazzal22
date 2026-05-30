 الإضافات

`bash id="p0x7a1"
npm install three @react-three/fiber @react-three/drei
npm install framer-motion lucide-react
npm install clsx tailwind-merge
```

---

# 🌌 2. Neural Network Animated Background (Three.js)

## `components/NeuralBackground.tsx`

tsx id="n3u7b1"
"use client"

import { Canvas, useFrame } from "@react-three/fiber"
import { Points, PointMaterial } from "@react-three/drei"
import { useMemo, useRef } from "react"
import * as THREE from "three"

function NeuralPoints() {
  const ref = useRef<any>()

  const points = useMemo(() => {
    const p = new Float32Array(500 * 3)
    for (let i = 0; i < p.length; i++) {
      p[i] = (Math.random() - 0.5) * 10
    }
    return p
  }, [])

  useFrame(() => {
    if (ref.current) ref.current.rotation.y += 0.0008
  })

  return (
    <Points ref={ref} positions={points} stride={3} frustumCulled>
      <PointMaterial
        transparent
        color="#00ffcc"
        size={0.02}
        sizeAttenuation
        depthWrite={false}
      />
    </Points>
  )
}

export default function NeuralBackground() {
  return (
    <div className="fixed inset-0 -z-10 bg-black">
      <Canvas camera={{ position: [0, 0, 5] }}>
        <NeuralPoints />
      </Canvas>
    </div>
  )
}
```

---

# 🤖 3. AI Chat داخل الموقع (واجهة فقط)

## `components/AIChat.tsx`

tsx id="c7h9d2"
"use client"

import { useState } from "react"

export default function AIChat() {
  const [messages, setMessages] = useState([
    { role: "ai", text: "Hello! Ask me anything about Ahmad 👋" },
  ])
  const [input, setInput] = useState("")

  const sendMessage = () => {
    if (!input) return

    const userMsg = { role: "user", text: input }
    const aiMsg = {
      role: "ai",
      text: "This is a demo AI response (connect API later)",
    }

    setMessages([...messages, userMsg, aiMsg])
    setInput("")
  }

  return (
    <div className="fixed bottom-6 right-6 w-80 bg-white/10 backdrop-blur-xl border border-white/20 rounded-2xl p-3">
      
      <div className="h-60 overflow-y-auto text-sm space-y-2">
        {messages.map((m, i) => (
          <div key={i} className={m.role === "ai" ? "text-cyan-300" : "text-white"}>
            {m.text}
          </div>
        ))}
      </div>

      <div className="flex mt-2 gap-2">
        <input
          className="flex-1 bg-black/40 p-2 text-sm rounded-lg outline-none"
          value={input}
          onChange={(e) => setInput(e.target.value)}
        />
        <button onClick={sendMessage} className="px-3 bg-cyan-500 rounded-lg">
          →
        </button>
      </div>
    </div>
  )
}
```

---

# 🖥️ 4. Terminal Intro Loading Screen

## `components/TerminalIntro.tsx`

tsx id="t9r4k1"
"use client"

import { useEffect, useState } from "react"

export default function TerminalIntro({ onFinish }: { onFinish: () => void }) {
  const lines = [
    "Initializing AI Portfolio...",
    "Loading Neural Network...",
    "Connecting LLM modules...",
    "Deploying UI System...",
    "Done ✔",
  ]

  const [index, setIndex] = useState(0)

  useEffect(() => {
    if (index < lines.length) {
      const t = setTimeout(() => setIndex(index + 1), 700)
      return () => clearTimeout(t)
    } else {
      setTimeout(onFinish, 500)
    }
  }, [index])

  return (
    <div className="fixed inset-0 bg-black flex items-center justify-center text-green-400 font-mono">
      <div>
        {lines.slice(0, index).map((l, i) => (
          <p key={i}>> {l}</p>
        ))}
      </div>
    </div>
  )
}
```

---

# 🌫️ 5. Glassmorphism UI (Tailwind Style Helper)

## أضف هذا لأي Card / Section:

tsx id="g1a2b3"
className="bg-white/10 backdrop-blur-xl border border-white/20 rounded-2xl shadow-xl"
```

---

# 🎯 مثال Hero بعد التحديث

tsx id="h3e0r1"
export default function Hero() {
  return (
    <section className="h-screen flex flex-col items-center justify-center text-center">
      
      <h1 className="text-6xl font-bold bg-gradient-to-r from-cyan-400 to-white text-transparent bg-clip-text">
        Ahmad Nazzal
      </h1>

      <p className="text-gray-400 mt-3">
        AI Agent Developer · Neural Systems · RAG Architect
      </p>
    </section>
  )
}
```

---

# 🧩 6. دمج كل شيء في الصفحة

## `app/page.tsx`

tsx id="m8p2x9"
"use client"

import { useState } from "react"
import NeuralBackground from "@/components/NeuralBackground"
import TerminalIntro from "@/components/TerminalIntro"
import AIChat from "@/components/AIChat"
import Hero from "@/components/Hero"

export default function Home() {
  const [loading, setLoading] = useState(true)

  return (
    <>
      {loading && <TerminalIntro onFinish={() => setLoading(false)} />}

      {!loading && (
        <>
          <NeuralBackground />
          <Hero />
          <AIChat />
        </>
      )}
    </>
  )
}

بس قلّي:
**"حوّله لمستوى OpenAI style portfolio"** 🚀
