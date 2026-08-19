# Harshil Gupta

**Backend engineer building systems that handle real concurrency and state.**

I build backend systems, developer tools and products from the ground up, currently going deep in distributed systems and developer tooling.

[![Portfolio](https://img.shields.io/badge/Portfolio-111111?style=flat-square&logo=google-chrome&logoColor=white)](https://harshilgupta.me)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/harshil-sync)
[![X](https://img.shields.io/badge/X-111111?style=flat-square&logo=x&logoColor=white)](https://x.com/_Harshil05_)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.gg/NJEjK3qv)

---

## What I'm Building

### [reqsh](https://github.com/hars-21/reqsh) - Interactive HTTP Shell
A stateful alternative to curl, built from scratch in Rust - stores base URLs, headers and variables so you're not retyping the full request every time.

- **48 GitHub stars · 111 release downloads · 59 installs via Crates.io · 3 external contributors**
- Persistent sessions, variable interpolation and pretty-printed JSON output across 23 commands
- Cuts ~10-15s off every repeated API call by eliminating request reconstruction

→ [reqsh.dev](https://www.reqsh.dev)

### [PaperDrill](https://github.com/hars-21/paperdrill) - Exchange infrastructure for developers
A limit-order matching engine and exchange backend, built to understand how real trading systems work end to end.

- **3,392 orders/sec throughput · 0.82ms average match latency · 500 concurrent WebSocket connections with zero drops** (local benchmark)
- Order book built for O(log n) insertion and O(1) best-bid/ask lookup, with price-time priority matching
- Orders are sequenced through Redis Streams into a single-threaded matching engine, race conditions are eliminated by design, not patched with locks
- A dedicated worker aggregates the trade stream into OHLCV candles in real time, independent of the matching engine's critical path

→ [paperdrill.dev](https://www.paperdrill.dev)

---

## Tech

**Languages**
`Rust` `TypeScript` `JavaScript` `Python`

**Backend**
`Node.js` `Express` `Next.js` `REST APIs` `WebSockets`

**Data & Infrastructure**
`PostgreSQL` `Redis` `MongoDB` `Docker` `Linux` `Git` `Nginx`

**Going Deeper**
`Concurrency` `Networking` `Async Systems` `Distributed Systems`

**Currently Exploring**
`LLM Fundamentals` `AI Systems`

---

<p align="center">
  <sub>Build systems. Ship software. Learn from what breaks.</sub>
</p>
