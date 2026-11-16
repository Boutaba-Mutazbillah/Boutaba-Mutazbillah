# Boutaba Mu'taz billah
### Low-Level Security Researcher & Reverse Engineer (`Ring 3 ➔ Ring 0`)

```assembly
; Windows x64 Bare-Metal Silicon Profile (Zero-API)
section .text
    global _start

_start:
    rdtsc                   ; Read raw CPU cycle counter
    xor rax, rdx            ; Entropy & register state mutation
    cpuid                   ; Direct silicon architectural query
    hlt                     ; Strict hardware execution halt
```

# Hi, I'm Mu'taz billah Boutaba 

I am a Computer Science Student at **Università degli Studi dell'Insubria** (Italy), deeply invested in systems programming and binary security research. My daily environment is driven by **Arch Linux** alongside isolated **Windows** setups, working closely with bare-metal execution and software isolation mechanics. 

- **Focus:** OS Internals (`Ring 3` to `Ring 0`), Reverse Engineering, and Bare-Metal Security.
- **Approach:** Speaking the CPU's native tongue—building ultra-compact, zero-API Proof-of-Concepts (PoCs) driven by pure math and raw hardware behavior.

---

## [0x01] Methodology: The Adversarial Loop & Zero-API Execution
I do not rely on high-level APIs or automated wrappers that analysts can easily hook; my approach is built from the ground up by interacting directly with the CPU and pure mathematical logic. My research operates on a strict, self-contained **Red-vs-Blue feedback loop**:

1. **Deep Hardware Exploration:** Dissecting raw CPU instructions, registers, caches, and microarchitectural behaviors down to the cycle level—turning every newly learned instruction into both an offensive and defensive primitive.
2. **Zero-API & Math-Driven Crafting:** Writing ultra-compact, high-speed Assembly payloads (`<20 lines`) driven purely by math and register manipulation—leaving zero external API calls to intercept.
3. **Self-Adversarial Testing & Documentation:** Executing custom binaries in isolated environments under debuggers (`x64dbg`, `WinDbg`) and telemetry tools to break my own logic, while rigorously mapping register and memory states with **pen and paper**.
4. **Bare-Metal Defense Engineering:** Translating discovered weaknesses into resilient, low-overhead countermeasures engineered to detect and neutralize tampering directly at the hardware level.

---

## [0x02] Low-Level Data Representation & Machine Code Expertise
- **Multi-Base Mastery:** Expert in navigating and manipulating raw architecture data across all numeral systems: **Binary (Base-2), Octal (Base-8), Decimal (Base-10), and Hexadecimal (Base-16)**.
- **Pure Binary & Hex Engineering:** Capability to analyze, write, and patch executables directly at the byte level (**Raw Bytes / Machine Code**), enabling the creation and modification of standalone software structures or payloads without relying on standard assemblers.

---

## [0x03] Core Tech Stack

```assembly
; Driven by efficiency and control
section .data
    languages:  db 'x86_64 Assembly (Zero-API / Raw CPU Primitives)', 0
    os_kernel:  db 'Windows 10 Education & Windows Internals', 0
```

- **Languages:** Pure `x86` / `x86_64` Assembly (NASM / MASM).
- **Toolchain & Disassemblers:** NASM, Make, Ghidra, x96dbg (x64dbg / x32dbg), WinDbg, GoBug.
- **Editors & IDEs:** Notepad++, SASM (Simple ASM), MASM32 Editor, AkelPad.
- **Monitoring & Auditing:** Full Sysinternals Suite, Full NirSoft Tools Suite, Wireshark (Raw socket & packet telemetry), and Pen & Paper (for register/state mapping).
- **Environments:** Custom Arch Linux environment and isolated Windows 10 Education / Enterprise Evaluation setups optimized for binary auditing and systems compilation.

---

## [0x04] Active Research Areas
- **Microarchitectural & Hardware-Level Defense:** Exploiting raw CPU instructions, timing anomalies, cache behaviors, and hardware internals to detect debuggers, sandboxes, and execution tampering without API dependencies.
- **Memory & Execution Integrity:** Implementing custom, math-driven anti-tamper mechanisms, stack protections, and user/kernel-space anomaly detection.
- **Network Telemetry:** Auditing raw network sockets and exploring dynamic packet routing behaviors.

---

## [0x05] Connect & Collaboration
If you are interested in binary security research, low-level engineering, or career opportunities, feel free to reach out:
- **Email:** mutaz.billah.revas [at] gmail.com
- **LinkedIn:** [Mu'taz billah Boutaba](https://www.linkedin.com/in/mu-taz-billah-boutaba-39ab053a1/)

---

> *"Abstractions hide the truth; registers never lie. To build a defense that cannot be bypassed, you must first become the adversary that breaks it."*
