# System Architecture: OrderGuard

## The Problem
In trading systems, network timeouts create "Uncertain States." If a client clicks "BUY" twice, and the broker network drops the first response, the trader risks duplicate financial exposure.

## The Solution (High-Assurance Pipeline)
We designed a system where **durability** and **safety** are handled at the database and systems level, not just in the UI.

```text
[ Frontend (React/TS) ]
         │  (REST + Idempotency Key)
         ▼
[ Go Backend (Orchestrator) ]
         │
         ├──> [ PostgreSQL (Hosted) ] ── Durable state & Idempotency Records
         │
         └──> [ Rust Safety Library (cgo) ]
                  └── Deterministic Duplicate Detection Rules

                  Key Engineering Decisions
Why Rust for Safety Rules? To guarantee memory safety and zero-cost abstractions when evaluating complex duplicate-order logic. It acts as a pure function: input JSON → output boolean/error.

Why Go for Orchestration? Go's concurrency model (Goroutines) is perfect for managing asynchronous broker responses and handling timeouts.

Why PostgreSQL? It is the single source of truth. Even if the app crashes mid-order, the idempotency key ensures the order cannot be duplicated upon restart.

