# Hi, I'm Eugen | Systems Semantics & Performance Engineering ⚙️

I build graph-oriented systems focused on deterministic execution, explicit dataflow, memory locality, and structurally derived optimization.

My work combines:
- Systems programming
- Arena-based memory models
- Graph semantics
- Zero-copy architectures
- Compiler experimentation
- Hardware-aware execution models

The goal is not adding abstraction layers —
the goal is removing unnecessary ones.

---

## 🧠 Core Project: **Leek**
**An experimental systems semantics framework with graph-based execution and pluggable language frontends.**

Leek is not just another programming language.
It is an attempt to formalize deterministic systems programming through explicit semantics, scoped lifetimes, and structural compiler analysis.

### Core Concepts
- Deterministic execution
- Pure / Impure separation
- Arena-scoped memory
- Explicit dataflow graphs
- KPN-inspired parallelism
- Graph-derived optimization
- Zero hidden runtime behavior
- DOT/SVG execution graph export
- Frontend-agnostic semantic model

### Current Status
Early-stage research compiler and semantic prototype.

Current implementation includes:
- AST generation
- Semantic graph construction
- Scope isolation
- Arena layouts
- DOT graph export
- Basic C backend generation
- Validation infrastructure for graph invariants

---

## 🚀 Featured Project: **BumpArena**
**A lightweight high-performance arena allocator for Bun & Node.js.**

BumpArena explores deterministic memory behavior inside JavaScript runtimes by replacing object-heavy allocation patterns with flat binary memory regions.

### Features
- Zero dependencies
- Flat `ArrayBuffer` memory model
- Deterministic O(1) arena reset
- Reduced GC pressure
- Cache-friendly linear allocation
- Optimized for large streaming workloads

---

## 📊 Benchmark (10M Records)

Comparison against traditional JS allocation strategies when processing 10 million records.

| Metric | Naive Array | Standard Array | **BumpArena** | **BumpArena (Turbo)** |
| :--- | :--- | :--- | :--- | :--- |
| **Total Time** | 2.99s | 6.21s | 5.35s | **4.02s** |
| **Throughput** | 3.3M lines/s | 1.6M lines/s | 1.8M lines/s | **2.4M lines/s** |
| **RSS Memory** | 1.75 GB | 1.73 GB | 2.25 GB | **1.39 GB** |
| **Heap Usage** | 0.63 GB | 0.69 GB | 0.64 GB | **0.60 GB** |

[Full Benchmark Details](https://github.com/eugen252009/BumpArena/blob/main/bench/bench.md)

---

## 🧪 Work in Progress: **vBuf**
A future zero-copy structured buffer system intended to build on top of Leek semantics and graph-based execution principles.

The long-term goal is a deterministic, structure-aware transport and parsing layer with:
- Zero-copy access patterns
- Offset-based data traversal
- Explicit lifetime ownership
- Arena-compatible layouts
- Streaming-oriented processing

---

## ⚙️ Areas of Interest

- Systems semantics
- Compiler construction
- Graph execution models
- Arena allocators
- Dataflow systems
- Kahn Process Networks
- Hardware-aware optimization
- Deterministic execution
- SIMD-friendly layouts
- Zero-copy parsing

---

## 📫 Currently Exploring

- Graph-based compiler architectures
- DOT/SVG execution tracing
- Deterministic parallel scheduling
- Explicit effect systems
- Hardware-constrained pipelines
- Real-time capable semantic models

---

> “Structure first. Optimization follows naturally.”
