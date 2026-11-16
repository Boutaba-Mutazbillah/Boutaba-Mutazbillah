# Boutaba Mu'taz billah
### Low-Level Security Researcher & Reverse Engineer (`Ring 3 ➔ Ring 0`)

```assembly
section .text
    global _start

_start:
    rdtsc                  
    xor rax, rdx           
    cpuid                   
    hlt                     
```

# Hi, I'm Mu'taz billah Boutaba 

I am a Computer Science Student at **Università degli Studi dell'Insubria** (Italy), deeply invested in systems programming and binary security research. My primary daily environment is **Windows 10 Education**, complemented by lightweight **Arch Linux** setups for cross-platform systems exploration, working closely with bare-metal execution and software isolation mechanics.

- **Focus:** OS Internals (`Ring 3` to `Ring 0`), Reverse Engineering, and Bare-Metal Security.
- **Approach:** Speaking the CPU's native tongue—building ultra-compact, zero-API Proof-of-Concepts (PoCs) driven by pure math and raw hardware behavior.

---

## [0x01] Methodology
I do not rely on high-level APIs or automated wrappers that analysts can easily hook; my approach is built from the ground up by interacting directly with the CPU and pure mathematical logic. My research operates on a strict, self-contained **Red-vs-Blue feedback loop**:

1. **Deep Hardware Exploration:** Dissecting raw CPU instructions, registers, caches, and microarchitectural behaviors down to the cycle level—turning every newly learned instruction into both an offensive and defensive primitive.
2. **Zero-API & Math-Driven Crafting:** Writing ultra-compact, high-speed Assembly payloads driven purely by math and register manipulation—leaving zero external API calls to intercept.
3. **Self-Adversarial Testing & Documentation:** Executing custom binaries in isolated environments under debuggers (`x64dbg`, `WinDbg`) and telemetry tools to break my own logic, while rigorously mapping register and memory states with **pen and paper**.
4. **Bare-Metal Defense Engineering:** Translating discovered weaknesses into resilient, low-overhead countermeasures engineered to detect and neutralize tampering directly at the hardware level.

---

## [0x02] Core Tech Stack

```assembly

section .data
    languages:  db 'x86_64 Assembly (Zero-API / Raw CPU Primitives)', 0
    os_kernel:  db 'Windows 10 Education & Windows Internals', 0
```

- **Languages:** `x86` / `x86_64` Assembly (NASM / MASM).
- **Toolchain & Disassemblers:** NASM, Ghidra, x96dbg (x64dbg / x32dbg), WinDbg, GoBug.
- **Editors & IDEs:** Notepad++, SASM (Simple ASM), MASM32 Editor, AkelPad.
- **Monitoring & Auditing:** Full Sysinternals Suite, Full NirSoft Tools Suite, Wireshark (Raw socket & packet telemetry), and Pen & Paper (for register/state mapping).
- **Environments:** Windows 10 Education & Enterprise Evaluation setups for binary auditing, plus Arch Linux environments.
---

## [0x03] Active Research Areas
- **Microarchitectural & Hardware-Level Defense:** Exploiting raw CPU instructions, timing anomalies, cache behaviors, and hardware internals to detect debuggers, sandboxes, and execution tampering without API dependencies.
- **Memory & Execution Integrity:** Implementing custom, math-driven anti-tamper mechanisms, stack protections, and user/kernel-space anomaly detection.
- **Network Telemetry:** Auditing raw network sockets and exploring dynamic packet routing behaviors.

---

## [0x04] Connect 

- **Email:** mutaz.billah.revas [at] gmail.com
- **LinkedIn:** [Mu'taz billah Boutaba](https://www.linkedin.com/in/mu-taz-billah-boutaba-39ab053a1/)

---
