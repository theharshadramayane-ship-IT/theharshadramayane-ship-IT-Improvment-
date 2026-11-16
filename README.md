# Hi, I'm The Harshad Ramayane 👋
### Systems & Backend Engineer | Fintech Infrastructure | MERN & Rust

> *"Building resilient systems where correctness, state, and performance are non-negotiable."*

I am an Information Technology student (Class of 2027) specializing in backend architecture, low-level systems programming, and distributed system reliability. I don't just build web apps; I engineer state machines, safe FFI boundaries, and durable data pipelines. 

Currently, I am bridging the gap between **Go**, **Rust**, and **PostgreSQL** to build high-assurance financial infrastructure.

---

### 🚀 Core Competencies

> **Backend Engineering & Architecture**
> - **Go (Golang):** Concurrency (Goroutines/Channels), REST API design, Clean Modular Architecture, cgo/FFI integration.
> - **Node.js / Express:** Event-driven architecture, middleware orchestration, API gateways.
> - **Rust:** Memory safety, Ownership/Borrowing, C-ABI interoperability, zero-cost abstractions.

> **Data & Persistence**
> - **PostgreSQL:** Transactions, ACID compliance, JSONB, connection pooling, durable idempotency, migrations.
> - **MongoDB:** NoSQL data modeling, aggregation pipelines.
> - **MySQL:** Relational schema design.

> **Systems & Reliability (In Progress)**
> - Duplicate-order protection, Event-driven lifecycles, Broker reconciliation, Distributed locks.
> - C-ABI FFI (Foreign Function Interface) boundaries between Rust and Go.

---

### 🛡️ Featured Infrastructure Project: OrderGuard
*(Currently in Active Development)*

A production-minded trading order reliability and protection infrastructure.
- **The Problem:** Traders suffer financial loss due to accidental duplicate orders and "UNKNOWN" broker states caused by network timeouts.
- **The Architecture:** `React (TS)` → `Go Backend` → `Rust Safety Library (cgo)` → `Hosted PostgreSQL`.
- **The Engineering:** Implements explicit order state machines, durable idempotency keys, and a zero-trust FFI boundary to evaluate safety rules without I/O blocking.

---

### 📌 Additional Projects

- **Blood-D-System:** Full-stack blood management application (React, Node.js/Express, MongoDB). *Focus: scalable state management and RESTful API design.*
- **SentraBand:** H₂S Exposure Monitoring Concept (Hardware + Web Prototype). *Focus: IoT data ingestion and record management.*
- **Mihir Ceramics Website:** Business web deployment. *Focus: Frontend performance and accessibility.*

---

### 🛠️ The Tech Stack

<div align="left">
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" alt="Go" />
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
</div>

---

### 🧠 Engineering Philosophy

> [!IMPORTANT]  
> **Correctness over speed.** I prefer building an idempotent, crash-safe transaction pipeline over a fast but unreliable endpoint. 
> 
> **Safety at the boundaries.** Using Rust via FFI in Go allows me to keep business logic orchestrated in Go, while delegating deterministic, memory-safe rule evaluations to Rust.
> 
> **Observability by default.** A system that fails silently is broken. State machines must explicitly track transitions, and failures must be auditable.

---

### 📫 Connect With Me

I am always open to discussing backend architectures, distributed systems, and fintech reliability.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/harshad-ramayane-34b48731b/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/theharshadramayane-ship-IT)

---
<p align="center">
  <i>"A system that fails silently is a system that cannot be trusted."</i>
</p>
