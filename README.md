# 🐺 Wolfitway Core

> **The Sovereign, Memory-Safe European Web Runtime & Local AI Engine in Rust.**  
> Built and maintained by **Drăguța Dan-Ioan** ([Wolfitway Agency SRL](https://wolfitway.com)).

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Language: Rust](https://img.shields.io/badge/Language-Rust-orange.svg)](https://www.rust-lang.org/)
[![Runtime: Loco.rs / Axum](https://img.shields.io/badge/Framework-Loco.rs-green.svg)](https://loco.rs/)

---

## 🇪🇺 Vision & European Digital Sovereignty

The modern web is dominated by memory-unsafe legacy systems (PHP/C++) and centralized foreign cloud monoliths that extract recurring subscription rents and force data into closed US AI APIs.

**Wolfitway Core** is an open-source, digital commons foundation extracted from the 300,000+ line Wolfitway OS architecture. It provides an auditable, high-performance, memory-safe alternative designed for independent creators, self-hosters, and European micro-enterprises.

### 🛡️ Core Pillars
* **100% Memory-Safe:** Built ground-up in asynchronous Rust (Tokio, Axum, SeaORM, Loco.rs) to eliminate entire classes of memory corruption and injection vulnerabilities.
* **European & Local AI Autonomy:** Native Bring-Your-Own-Key (BYOK) interfaces supporting **Mistral AI** and offline GPU/CPU inference via **Ollama / LocalAI** — zero telemetry, zero forced cloud lock-in.
* **1-Click GDPR Data Custody:** Flat SQLite/JSON zero-lock-in export with optional AEAD encryption. You own your data, your database, and your identity.
* **Open Syndication:** Built-in open web standards including RSS 2.0, Atom, and structured semantic feeds.

---

## 🗺️ Workspace Architecture

Wolfitway OS uses a modern Cargo workspace to maintain a strict, auditable boundary between the open-source digital commons and optional commercial modules:

```text
wolfitway-os/
├── Cargo.toml                  # Workspace root
├── crates/
│   ├── wolfitway-core/         # 🟢 GPLv3 — Sovereign Base, Auth, BYOK, Mistral/Ollama, CMS
│   └── wolfitway-server/       # 🚀 Binary crate — Standalone Community Server
└── migration/                  # 🟢 Database migrations (SeaORM / SQLite / PostgreSQL)
