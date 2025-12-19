<p align="center">
  <img src="https://media.giphy.com/media/3oEjI6SIIHBdRxXI40/giphy.gif" alt="matrix" width="100"/>
</p>

<h1 align="center">Hi, I’m <code>s1mpleog</code> 👋</h1>
<p align="center"><em>Low-level backend tinkerer • C/C++ & Rust fan • obsessed with how computers *really* work</em></p>

<p align="center">
  <!-- Badges -->
  <img src="https://img.shields.io/badge/OS-Arch%20Linux-1793d1?style=for-the-badge&logo=linux" alt="arch linux"/>
  <img src="https://img.shields.io/badge/Language-C/C++-00599C?style=for-the-badge&logo=c" alt="c/c++"/>
  <img src="https://img.shields.io/badge/Rust-Backend-DEA584?style=for-the-badge&logo=rust&logoColor=000" alt="rust"/>
  <img src="https://img.shields.io/badge/Framework-Axum-black?style=for-the-badge" alt="axum"/>
  <img src="https://img.shields.io/badge/Frontend-Next.js-111827?style=for-the-badge&logo=next.js" alt="nextjs"/>
</p>

---

# About me

* 🔧 I build backend systems that I can explain at the assembly level. I don’t just type `cargo run` — I ask *why*.
* 🧠 Passionate about memory management, pointers, compilers, OS internals, and tiny, elegant APIs.
* 🛠️ Comfortable in **C/C++**, **Rust**; I use **Axum** for Rust backends and dabble in **Next.js** when a UI is needed.
* 🐧 Favorite OS: **Arch Linux** — minimal, configurable, and fast.
* 📚 Currently studying: advanced systems programming and math (real analysis is my north star).

---

# What I make (high level)

* **Low-latency services** in Rust & C++ that squeeze predictable performance out of hardware.
* **Systems-level tooling**: small utilities, allocators, tracing helpers, and instrumentation.
* **Educational code**: minimal reproducible examples that show how things work (assembly, memory layout, cache effects).

---

# Tech Radar

| Area            | Tools & Tech                                                                   |
| --------------- | ------------------------------------------------------------------------------ |
| Languages       | `Rust`, `C`, `C++`, `Assembly`, `Go` (learning)                                |
| Backend         | `axum`, `tokio`, `hyper`, `actix-web` (experimental)                           |
| Frontend        | `Next.js`, `Vite` (when I need a tiny UI)                                      |
| DevOps / Infra  | `systemd`, `Docker`, `nginx`, `prometheus` (observability)                     |
| Other interests | compilers, OS internals, memory allocators, Vulkan/OpenGL (graphics low-level) |

---

# Skill Highlights

* ✅ Deep interest in **memory layout**, stack vs heap, pointer aliasing, and undefined behavior — I read/write assembly and debug with `gdb`/`rr`/`perf`.
* ✅ Strong in systems programming fundamentals: concurrency, lock-free patterns, and cache-conscious design.
* ✅ Comfortable architecting backends that trade off ergonomics for performance and predictability.

---

# Projects & Showcases

> *This section is customizable — swap in repo links you want pinned.*

* **`tiny-allocator`** — Minimal allocator written to understand heap management (conceptual + assembly walkthrough).
* **`axum-playground`** — Small, production-minded services built with Axum and Tokio, instrumented for latency profiling.
* **`low-level-demos`** — Micro projects: syscall wrappers, tiny VMs, assembly puzzles, and cache-timing experiments.

---

# How I work

1. Start from first principles: what does the CPU see? what's in L1 vs L3? where are we allocating?
2. Prototype a small, idiomatic implementation (Rust/C++).
3. Measure and profile (perf, flamegraphs).
4. Iterate with micro-optimizations only where they actually matter.

---

# Code Snippets (style & intent)

```rust
// minimal axum route — small, explicit, and instrumentable
use axum::{routing::get, Router};

async fn health() -> &'static str { "ok" }

fn app() -> Router {
  Router::new().route("/health", get(health))
}
```

```c
// peek: how a pointer is a pointer — intentionally explicit
int *alloc = malloc(sizeof(int)*4);
// layout matters: look at addresses, not just values
```

---

# Readme Candy (dynamic cards)

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=s1mpleog&show_icons=true&theme=tokyonight" alt="github stats"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=s1mpleog&layout=compact&theme=tokyonight" alt="top langs"/>
</p>

> ⚠️ If you deploy this to GitHub, these cards will render live — great for showing off languages & activity.

---

# How to reach me

* GitHub: `https://github.com/s1mpleog`
* Twitter / X: *(optional — add if you want)*
* Email: `hi at s1mple dot dev` *(replace with your email if you want to show it)*

---

# Want this style but different tone?

I can produce variations:

* Minimal / resume-style
* Hacker-y terminal aesthetic
* Playful / gaming aesthetic

---

<p align="center">Made with ⚙️ and a tiny obsession for how bits actually move.</p>

<!-- Footer: small, sleek -->

<p align="center">⭐️ If you like low-level systems, follow along — I ship small, readable experiments that teach one idea at a time.</p>
