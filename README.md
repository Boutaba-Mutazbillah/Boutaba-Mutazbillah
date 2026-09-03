# Boutaba Motezeballah
### Systems Architect & Reverse Engineer

```assembly
; Arch Linux Microarchitectural Initialization Profile
section .text
    global _start

_start:
    mov rax, 60         ; sys_exit syscall
    xor rdi, rdi        ; status 0
    syscall
```

# Hi, I'm Motezeballah Boutaba 

I am a Computer Science Student at **Università degli Studi dell'Insubria** (Italy), deeply invested in systems programming and binary security research. My daily environment is driven by **Arch Linux**, working closely with bare-metal execution and software isolation mechanics.

-  **Focus:** Linux Internals, Reverse Engineering, and Kernel Security Sandboxes.
-  **Approach:** Building lightweight Proof-of-Concepts (PoCs) to study anti-analysis and memory mitigation strategies.

---

###  Core Tech Stack

```assembly
; Driven by efficiency and control
section .stack
    languages:  db 'C', 0, 'C++', 0, 'x86_64 Assembly', 0
    os_kernel:  db 'Arch Linux (Custom Environment)', 0
```

- **Languages:** Pure C, Modern C++, and x86_64 Assembly (NASM / AT&T syntax).
- **Toolchain:** GCC, Clang, Make, GDB, and x64dbg.
- **Environment:** Custom Arch Linux setup optimized for binary auditing and systems compilation.

---

###  Active Research Areas
- **Anti-Debugging:** Intercepting process tracers via native `sys_ptrace` and microarchitectural timing analysis (`RDTSC`).
- **Memory Integrity:** Implementing stack smash protections (Canaries) and memory pattern matching in user-space.
- **Network Telemetry:** Auditing raw network sockets and exploring dynamic packet routing behaviors.

---

