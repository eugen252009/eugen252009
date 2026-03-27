# Hi, I'm Eugen | Systems Architect in TypeScript and Go 🏎️💨

I build software that runs faster than the engines it’s built on. My focus is on **Extreme Performance**, **Zero-Copy Architectures**, and pushing **TypeScript** to its absolute physical limits.

## 🛠️ The Philosophy: "Mechanical Sympathy"
I don’t believe in "good enough" performance. I believe in understanding the underlying engine (V8/JSC) so deeply that I can bypass its overhead. My projects are designed to eliminate Garbage Collection (GC) pressure and object-header bloat by treating memory as a raw, high-speed resource.

> *"JavaScript was designed for convenience. I use it for throughput."*

---

## 🚀 Featured Project: **BumpArena**
**The ultra-fast, zero-overhead memory arena for Bun & Node.js.**

BumpArena is a 1.8kB powerhouse that redefines how we handle millions of data records in TypeScript. It bypasses the standard JS object-model to achieve raw, deterministic performance.

* **1.8 kB** Minified (Zero dependencies).
* **3M+ records/s** throughput.
* **Zero GC Pressure:** Manages memory in a flat `ArrayBuffer`.
* **The Irony:** A library so optimized that the only remaining bottleneck is the engine's own drive shaft.

---

## 🧪 In the Lab: **FlexBuf**
The logical successor to the Arena. A **Zero-Copy JSON-like Parser** that doesn't instantiate objects. 

* **No String Parsing:** Uses `start` and `length` offsets directly from the source buffer.
* **Fixed-Point Math:** Parses numbers using integer-multiplication tricks to avoid `parseFloat` overhead.
* **The Goal:** Moving data from a stream to logic with literally **zero** intermediate objects.

---

## 📊 Performance over Hype
I prefer a **1.8kB** solution that solves a problem permanently over a **50MB** framework that just hides it. 

| Metric | Standard TS/JS | My Approach (Arena/FlexBuf) |
| :--- | :--- | :--- |
| **Memory** | Bloated by Object-Headers | Pure Binary Density |
| **Cleanup** | Unpredictable GC Pauses | O(1) Instant Reset |
| **Speed** | Engine-Limited (Logic) | Engine-Bound (Hardware) |

---

## ⚡ Fun Fact
I once spent a week not writing a single line of code because the architecture needed to "ripen" in my head. The result? A refactoring roundtrip that distilled `alloc` down to its absolute essence. It’s not just code; it’s a performance statement.

## 📫 Connect with me
* **Currently exploring:** Low-level optimizations in Bun, Byte-level manipulation, and SharedArrayBuffers.
* **Ask me about:** Why your 10 million objects are killing your app’s latency.

---
*Generated with a touch of irony and peak performance.*