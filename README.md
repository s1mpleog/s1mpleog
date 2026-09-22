<div align="center">

<img src="./graven471_banner.svg" width="100%" />

<br/>

[![C++23](https://img.shields.io/badge/C%2B%2B23-161b22?style=flat-square&logo=c%2B%2B&logoColor=c9d1d9)](https://github.com/graven471)
[![Rust](https://img.shields.io/badge/Rust-161b22?style=flat-square&logo=rust&logoColor=c9d1d9)](https://github.com/graven471)
[![x86-64](https://img.shields.io/badge/x86--64-161b22?style=flat-square&logo=assemblyscript&logoColor=c9d1d9)](https://github.com/graven471)
[![Vulkan](https://img.shields.io/badge/Vulkan-161b22?style=flat-square&logo=vulkan&logoColor=c9d1d9)](https://github.com/graven471)
[![Linux](https://img.shields.io/badge/Linux-161b22?style=flat-square&logo=linux&logoColor=c9d1d9)](https://github.com/graven471)

</div>

---

### selected engineering

* **[`wind`](https://github.com/graven471/wind)** &nbsp;`c++23` `vulkan` `spir-v`  
  Vulkan real-time renderer and modular 3D engine core engineered from scratch. Features stateless command recording, explicit memory barrier sequencing, dynamic descriptor management, and custom buffer sub-allocators.

* **[`peel`](https://github.com/graven471/peel)** &nbsp;`c++23` `x86-64` `win32`  
  Zero-dependency binary visualizer and x86-64 machine-code disassembler. Directly decodes prefix, opcode, ModR/M, and SIB byte streams against Intel architecture manuals without external disassembly engines.

* **[`clmm-math`](https://github.com/graven471/clmm-math)** &nbsp;`rust` `solana` `fixed-point`  
  Deterministic, high-precision mathematical primitives for concentrated liquidity market makers (CLMM) on Solana. Implements exact Q64.64 fixed-point arithmetic, tick-to-sqrt-price transformations, and overflow-checked liquidity math.

* **[`wind-cooker`](https://github.com/graven471/wind-cooker)** &nbsp;`rust` `tooling` `spir-v`  
  Offline asset conditioning pipeline and packaging engine for Wind. Compiles high-level shader code to validated SPIR-V bytecode, bakes mesh geometry into memory-mappable structures, and produces packed runtime archives.

---

### engineering domains & primitives

| domain | focus & architectural primitives |
| :--- | :--- |
| **systems & runtime** | Custom memory models (slab / arena / pool allocators) · Explicit cache line padding · SIMD vectorization (AVX2) · x86-64 instruction decoding · PE & ELF binary parsers · ABI & calling convention analysis |
| **graphics & engines** | Explicit Vulkan synchronization & timeline semaphores · Custom image barrier sequencing · Shader compilation toolchains (GLSL / HLSL to SPIR-V) · Stateless render graph designs · Data-oriented ECS architecture |
| **decentralized protocols** | Deterministic fixed-point numerical schemes · Order book matching mechanics · Constant product & CLMM algorithms · Zero-copy byte deserialization · High-throughput on-chain state transitions |

---

### environment & workflow

```text
host        :: linux (arch / gentoo)
toolchains  :: clang++ / gcc · rustc / cargo · nasm · vulkan-sdk
environment :: neovim · git · tmux
debuggers   :: renderdoc · gdb · valgrind
```

<p align="center">
<code>build</code>  ·  <code>break</code>  ·  <code>inspect</code>  ·  <code>understand</code>  ·  <code>repeat</code>
</p>

