# Hey, I'm Fabi 🧠

**Building an entire personal stack where one AI sits at the center.**

That AI is **[Lucid](https://lucid-ai.app)** — agent-first, with real long-term memory and custom fine-tuned weights. Everything else I ship feeds it data and gets context from it: a productivity OS, a jailbroken biometric bridge, a calorie tracker, a Claude Code agent skeleton, a self-hosted inference server. **One brain, many surfaces.**

Solo founder, Lucid AI Labs · 🇩🇪 Germany

---

## 🧬 The Stack (everything orbits one AI)

### 🧠 The AI

- **Lucid** — custom Qwen-based LoRA fine-tunes. V5 shipped, V6 in identity-collapse training
- **Self-hosted inference** — `llama.cpp` on a custom GPU server, OpenAI-compatible adapter at `api.lucid-ai.app`
- **2026 SOTA neural memory** — Contextual Retrieval · RAG-Fusion · HyDE · FLARE · HyperGraphRAG · Temporal Knowledge Graph · MMR re-ranking
- **Memory lifecycle** — ACT-R base-level activation, memory reconsolidation, CLS sleep consolidation, spaced-repetition reinforcement
- **Active research** — memory-in-weights, beyond RAG into continuous learning

### 🦴 The Skeleton

- **The Caveman** — custom Claude Code agent OS: hot-reload dynamic instructions, neural-compaction hooks, pre-compact extraction, session rehydration, shard-injection
- **Multi-agent runtime** — Claude Code + Codex share **one** Supabase brain
- **One source of truth** — single `knowledge_entries` store with embeddings on every record. No fragmented RAG silos
- **Open-source MCPs** — tools I ship along the way (see pinned)

### 🌐 The Surfaces

- **[lucid-ai.app](https://lucid-ai.app)** — public PWA: productivity, tasks, mood, habits, calendar
- **Lucid Cockpit** — native Tauri Windows app, live Stripe + business metrics
- **iOS Bridge** — jailbroken Whoop streaming raw BLE biometrics (HR, HRV, DFA-α1, RR intervals) at ~5× the resolution Whoop's own app exposes. 343k+ rows live
- **Calorie tracker** — custom AI-aware nutrition logging (shipped May 2026)
- **More to come** — every personal-data surface I touch eventually feeds the brain

### 🖥️ The Server

- **GPU inference server** — `llama.cpp` + LoRA hot-loading, no merging required
- **Self-hosted Postgres** — Supabase, vector embeddings on every memory table
- **Cloudflare Access** — single-user OTP gate on private endpoints
- **Vercel** — front-end auto-deploys
- **Sovereign-by-default** — my data, my model, my server

---

## 🛠️ Stack badges

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Tauri](https://img.shields.io/badge/Tauri-FFC131?style=for-the-badge&logo=tauri&logoColor=black)
![Swift](https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![llama.cpp](https://img.shields.io/badge/llama.cpp-000000?style=for-the-badge&logo=meta&logoColor=white)
![Qwen](https://img.shields.io/badge/Qwen_LoRA-FF6A00?style=for-the-badge&logo=alibabacloud&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

---

## 🧬 What I think about

- **Agent-first AI vs tool-first AI** — most "AI apps" are just chat windows over an API. I'm building the opposite: an autonomous agent at the center, with apps as its sensory organs
- **Memory architectures that behave like a mind** — decay, reconsolidation, sleep consolidation. Not a vector database with extra steps
- **Sovereign personal AI** — my data, my model, my weights. No cloud lock-in
- **One AI knowing one person deeply**, not many people shallowly
- **The line between augmentation and autonomy** — when does a tool stop being a tool?

---

## 🌐 Find me

- 🌍 [lucid-ai.app](https://lucid-ai.app)
- 📷 [@fabi.spl](https://instagram.com/fabi.spl)
- 📧 Fabi@lucid-ai.app

---

> *"Building the kind of AI I'd actually want to use — and the entire stack underneath it."*
