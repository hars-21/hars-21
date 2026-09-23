# Harshil Gupta

**Backend engineer building systems that handle real concurrency and state.**

I build backend systems, developer tools and products from the ground up, currently going deep in distributed systems and developer tooling.

[![Portfolio](https://img.shields.io/badge/Portfolio-111111?style=flat-square&logo=google-chrome&logoColor=white)](https://harshilgupta.me)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/harshil-sync)
[![X](https://img.shields.io/badge/X-111111?style=flat-square&logo=x&logoColor=white)](https://x.com/_Harshil05_)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.gg/NJEjK3qv)

---

## What I'm Building

### [PaperDrill](https://github.com/hars-21/paperdrill)

A live exchange simulator with a price-time-priority matching engine, order book, REST API, and WebSocket market feed.

- O(log n) price-level insertion and O(1) best-bid/ask lookup
- Redis Streams for order sequencing and Redis Pub/Sub for correlated request/response
- A separate worker consumes trades and builds OHLCV candles outside the matching path

#### Production benchmark

| Scenario               |           Workload |                                     Result | p95 latency |
| ---------------------- | -----------------: | -----------------------------------------: | ----------: |
| Unmatched limit orders |             10,000 |              517 orders/sec · 100% success |    163.2 ms |
| Matched limit orders   |              5,000 |              507 orders/sec · 100% success |    168.4 ms |
| Single-order sweep     | 1,000 maker orders |                      Completed in 148.4 ms |           — |
| WebSocket fan-out      |    500 connections | Opened in 107 ms · 500/500 received update |     24.6 ms |

[Live](https://www.paperdrill.dev) · [Source](https://github.com/hars-21/paperdrill)

### [reqsh](https://github.com/hars-21/reqsh)
A stateful alternative to curl, built from scratch in Rust - stores base URLs, headers and variables so you're not retyping the full request every time.

- **50+ GitHub stars · 150+ release downloads · 70+ installs via Crates.io · 3 external contributors**
- Keeps base URLs, headers, variables, saved requests, and command history across sessions
- Uses an AST-based parser with separate execution and session modules
- Supports 7 HTTP methods and ships binaries for macOS, Linux, and Windows
- Built with Rust, Reqwest, Reedline, and Serde

[Website](https://reqsh.dev) · [Source](https://github.com/hars-21/reqsh) · [Releases](https://github.com/hars-21/reqsh/releases)

---

## Tech

**Languages**

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=000000)

**Backend**

![Bun](https://img.shields.io/badge/Bun-000000?style=flat-square&logo=bun&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white)
![REST APIs](https://img.shields.io/badge/REST_APIs-005571?style=flat-square)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socketdotio&logoColor=white)

**Data**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)

**Infrastructure**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=000000)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

---

<p align="center">
  <sub>Build systems. Ship software. Learn from what breaks.</sub>
</p>
