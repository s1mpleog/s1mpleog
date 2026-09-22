<div align="center">

<img src="./graven471_banner.svg" width="100%" />

<br/>

`C++23` &nbsp;·&nbsp; `Rust` &nbsp;·&nbsp; `x86-64 ASM` &nbsp;·&nbsp; `Vulkan` &nbsp;·&nbsp; `Linux`

</div>

---

### SELECTED REPOSITORIES

<details open>
<summary><b><code>wind</code></b> — Vulkan Real-Time Renderer & Graphics Engine <code>C++23</code> <code>Vulkan</code></summary>
<br>

* **Architecture:** Modular 3D rendering pipeline engineered entirely from scratch.
* **Synchronization:** Explicit timeline semaphores, automated layout transitions, and fine-grained barrier graphs.
* **Memory & Recording:** Stateless command buffer generation with custom GPU buffer/image sub-allocators.
* **Link:** [`github.com/graven471/wind`](https://github.com/graven471/wind)

</details>

<details open>
<summary><b><code>peel</code></b> — x86-64 Machine-Code Disassembler & PE Inspector <code>C++23</code> <code>x86-64</code></summary>
<br>

* **Binary Analysis:** Standalone zero-dependency visualizer and instruction-stream decoder.
* **Manual Compliance:** Decodes prefixes, opcodes, ModR/M, and SIB addressing directly from raw bytes using Intel specifications.
* **Format Inspection:** Complete traversal of Portable Executable (PE32+) headers, section headers, and imports.
* **Link:** [`github.com/graven471/peel`](https://github.com/graven471/peel)

</details>

<details>
<summary><b><code>clmm-math</code></b> — Deterministic Fixed-Point Math Engine <code>Rust</code> <code>Solana</code></summary>
<br>

* **Numerical Precision:** High-precision math primitives tailored for concentrated liquidity AMM protocols.
* **Arithmetic:** Deterministic Q64.64 fixed-point operations with guaranteed zero-overflow arithmetic under strict compute budgets.
* **Tick Math:** Tick-to-square-root-price algorithms and precise token delta conversions.
* **Link:** [`github.com/graven471/clmm-math`](https://github.com/graven471/clmm-math)

</details>

<details>
<summary><b><code>wind-cooker</code></b> — Offline Asset Pipeline & Compiler <code>Rust</code> <code>Tooling</code></summary>
<br>

* **Shader Processing:** Direct compilation, validation, and reflection of shader stages into SPIR-V binaries.
* **Data Packing:** Converts raw geometry and textures into memory-mappable, zero-copy runtime file formats.
* **Link:** [`github.com/graven471/wind-cooker`](https://github.com/graven471/wind-cooker)

</details>

---

### TECHNICAL SCOPE

<details open>
<summary><b><code>[+]</code> Systems & Runtime Internals</b></summary>
<br>

* **Memory Models:** Custom slab, arena, and pool allocators with explicit alignment and cache line padding.
* **Binary Formats:** Direct parsing of PE32+ and ELF executables, symbol tables, and relocation entries.
* **Architecture:** x86-64 calling conventions, ABI specifications, and hardware register constraints.

</details>

<details>
<summary><b><code>[+]</code> Graphics & Hardware Pipelines</b></summary>
<br>

* **Vulkan Primitives:** Manual memory allocation, dynamic descriptor sets, and timeline semaphore execution.
* **Shader Pipelines:** Multi-stage GLSL/HLSL compilation to SPIR-V, descriptor reflection, and specialization constants.
* **Engine Core:** Data-oriented scene graphs and stateless command recording patterns.

</details>

<details>
<summary><b><code>[+]</code> Protocol Mechanics & Math</b></summary>
<br>

* **Fixed-Point Arithmetic:** Exact integer math, discrete tick indexing, and invariant curve formulas.
* **State Machines:** Zero-copy serialization, high-throughput on-chain safety, and state verification.

</details>

---

### WORKSPACE & TOOLCHAINS

* **Toolchains:** `clang++` · `gcc` · `rustc` · `nasm` · `vulkan-sdk`
* **Environment:** `linux` (arch / gentoo) · `neovim` · `tmux` · `git`
* **Profiling & Trace:** `renderdoc` · `gdb` · `valgrind`

---

<p align="center">
  <code>build</code> &nbsp;·&nbsp; <code>break</code> &nbsp;·&nbsp; <code>inspect</code> &nbsp;·&nbsp; <code>understand</code> &nbsp;·&nbsp; <code>repeat</code>
</p>
