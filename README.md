# Boutaba Mu'taz billah
### Systems Architect & Reverse Engineer
![إحصائيات جيتهاب](https://vercel.app)

```assembly
; Arch Linux Microarchitectural Initialization Profile
section .text
    global _start

_start:
    mov rax, 60         ; sys_exit syscall
    xor rdi, rdi        ; status 0
    syscall
```

# Hi, I'm Mu'taz billah Boutaba 

I am a Computer Science Student at **Università degli Studi dell'Insubria** (Italy), deeply invested in systems programming and binary security research. My daily environment is driven by **Arch Linux**, working closely with bare-metal execution and software isolation mechanics. 

-  **Focus:** Linux Internals, Reverse Engineering, and Kernel Security Sandboxes.
-  **Approach:** Building lightweight Proof-of-Concepts (PoCs) to study anti-analysis and memory mitigation strategies.

---

## [0x01] My Philosophy: Bottom-Up Execution & Behavioral Research
I do not rely on high-level APIs or automated wrappers; my approach is built from the ground up by interacting directly with the CPU and native syscalls to avoid unnecessary abstractions. My rigorous learning and research loop follows three strict phases:
1. **Instruction Sequencing & Simulation:** Mastering single assembly commands to their microarchitectural core, analyzing how their specific execution order affects execution speed, and using them to simulate malware behaviors.
2. **Behavioral Telemetry:** Executing custom binaries within isolated sandboxes, dynamically tracking memory and kernel states, and performing rigorous physical documentation of every transition.
3. **Focused Mitigation:** Intercepting the execution pipeline mid-process to engineer target-specific, hardened countermeasures to neutralize the exact vector threat.

---

## [0x02] Low-Level Data Representation & Machine Code Expertise
- **Multi-Base Mastery:** Expert in navigating and manipulating raw architecture data across all numeral systems: **Binary (Base-2), Octal (Base-8), Decimal (Base-10), and Hexadecimal (Base-16)**.
- **Pure Binary & Hex Engineering:** Capability to analyze, write, and patch executables directly at the byte level (**Raw Bytes / Machine Code**), enabling the creation and modification of standalone software structures or payloads without relying on standard assemblers.

---

## [0x03] Core Tech Stack

```assembly
; Driven by efficiency and control
section .stack
    languages:  db 'x86_64 Assembly', 0
    os_kernel:  db 'Arch Linux (Custom Environment)', 0
```

- **Languages:** x86_64 Assembly (NASM / MASM / AT&T syntax).
- **Toolchain & Disassemblers:** NASM, Make, Ghidra, Radare2 / Rizin, x64dbg, WinDbg.
- **Editors & IDEs:** Notepad++, SASM (Simple ASM), MASM32 Editor.
- **Monitoring & Auditing:** Full Sysinternals Suite, Full NirSoft Tools Suite, and Wireshark (Raw socket & packet telemetry).
- **Environments:** Custom Arch Linux environment and isolated Windows Enterprise Evaluation setups optimized for binary auditing and systems compilation.

---

## [0x04] Active Research Areas
- **Anti-Debugging:** Intercepting process tracers via native `sys_ptrace` and microarchitectural timing analysis (`RDTSC` / `RDTSCP`).
- **Memory Integrity:** Implementing stack smash protections (Canaries) and memory pattern matching in user-space.
- **Network Telemetry:** Auditing raw network sockets and exploring dynamic packet routing behaviors.

---

## [0x05] Connect & Collaboration
If you are interested in binary security research, low-level engineering, or career opportunities, feel free to reach out:
- **Email:** mutaz.billah.revas [at] gmail.com
- **LinkedIn:** [Mu'taz billah Boutaba]( https://www.linkedin.com/in/mu-taz-billah-boutaba-39ab053a1/ )
