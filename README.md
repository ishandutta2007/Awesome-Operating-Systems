# Awesome-Operating-Systems

# Top Operating Systems Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on From-Scratch Kernels, Enterprise Linux & Desktop Accessibility*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Operating Systems**. These tools provide the foundational layer between hardware and applications — managing memory, processes, filesystems, and devices — with a spectrum running from enterprise-grade Linux distributions to hobbyist kernels built from scratch for the joy of understanding every layer.

**Examples** include SerenityOS, ToaruOS, Red Hat Enterprise Linux, Ubuntu, Debian, Fedora, Arch Linux, Windows, and macOS (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, from-scratch kernels, and transparent system architecture — ideal for OS developers, systems programmers, and anyone who wants to understand or control the software running beneath their applications.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Microsoft Windows** — The dominant commercial desktop OS with the broadest hardware and software compatibility. Proprietary licensing; enterprise editions add management and security features. **Best for users needing maximum application compatibility** and commercial software support.

- **Apple macOS** — Apple's Unix-certified desktop OS tightly integrated with its hardware ecosystem. Proprietary licensing tied to Apple hardware. **Best for users committed to the Apple ecosystem** who value polish and integration.

- **Red Hat Enterprise Linux (RHEL)** — The enterprise Linux standard with long-term support, certification programs, and vendor backing. Subscription-based. **Best for enterprises needing certified hardware/software stacks** and commercial support.

## Open-Source GitHub Projects

- **[SerenityOS](https://github.com/SerenityOS/serenity)**  
  **The from-scratch graphical Unix-like OS with 1990s aesthetics** — 2-clause BSD licensed . **A love letter to '90s user interfaces with a custom Unix-like core**, built entirely in-house from kernel to web browser . **Everything is right in the repository** — modern 64-bit kernel with pre-emptive multi-threading, WindowServer, AudioServer, WebServer, a browser with JavaScript/WebAssembly, HackStudio IDE, games (Solitaire, Minesweeper, 2048, chess), and **over 300 ports of popular open-source software** . **Security features** include W^X memory, pledge & unveil, (K)ASLR, OOM-resistance, and state-of-the-art TLS algorithms . **Started by Andreas Kling in 2018** after a rehabilitation program; now **959 contributors** with 194 new people in the last year alone . **The Ladybird web browser spun out** as a cross-platform application, receiving **$100,000 from Shopify** and two anonymous $100,000 donations . **64-bit only** — the 32-bit x86 port was removed . **Best for OS developers and enthusiasts** wanting a complete, hackable, from-scratch system that runs on real hardware and QEMU.

- **[ToaruOS](https://github.com/klange/toaruos)**  
  **A completely-from-scratch hobby OS** with bootloader, kernel, drivers, C library, dynamic linker, and userspace including a composited graphical UI and network stack . **Notable components**: **Misaka** (hybrid modular kernel), **Yutani** (window compositor), **Kuroko** (dynamic bytecode-compiled language), **Bim** (Vim-inspired editor with syntax highlighting), and **ld.so** (dynamic linker/loader) . **Current goals** include improving POSIX coverage, continuing to improve the C library, and replacing third-party development tools to achieve self-hosting . **Builds via Docker** with a pre-built container image, and forks can use GitHub CI . **Best for OS development learners** wanting a complete from-scratch system with clear component boundaries and modern build tooling.

- **[Debian](https://www.debian.org/)**  
  **The "Mother of all distributions"** — created by Ian Murdock in 1993, and the base for Ubuntu and thousands of other distros . **Three release branches**: **Stable** (rigorous testing, maximum reliability for servers), **Testing** (newer packages, good for desktops), and **Unstable/Sid** (latest packages for developers) . **APT package management** is clean and reliable, and Debian supports **x86, ARM, MIPS, IBM S/390**, and more architectures — runs on nearly anything . **Famed for security and stability**; as one forum user put it: **"Need handholding? Go with Ubuntu. Want privacy? Use Debian."** **Best for production servers and long-lived deployments** where stability matters more than bleeding-edge packages.

- **[Ubuntu](https://ubuntu.com/)**  
  **The most user-friendly Debian derivative** — developed by Canonical since 2004 . **Two release tracks**: **LTS** (every two years, five years of standard security maintenance, extendable to 10 with Ubuntu Pro) and **regular** (every six months, nine months of support) . **Ships Snap by default** and **adds the default user to the sudo group** — conveniences Debian lacks out of the box . **Best for new Linux users and desktop deployments** where ease of use and hardware support matter.

- **[Fedora](https://fedoraproject.org/)**  
  **Red Hat's community-sponsored proving ground** for technologies that later appear in RHEL . **Modern software stacks before they hit enterprise distributions**, with more stability than a pure rolling release . **Editions**: **Workstation** (developer desktop with GNOME and full dev toolchain), **Server**, **CoreOS** (minimal auto-updating OS for containers), and **Silverblue** (immutable desktop for container-focused workflows) . **Best for developers** wanting current toolchains and container tooling, or those who will eventually work with RHEL.

- **[Arch Linux](https://archlinux.org/)**  
  **The control-everything rolling release** — gives you nothing by default: no graphical installer, no desktop environment, no bundled software . **You partition disks manually, install a base system, configure networking, and build from there** — and the **Arch Wiki is the most comprehensive Linux documentation anywhere** . **Rolling release** means continuous updates without version upgrades; **Pacman** is fast and minimal; the **AUR** contains tens of thousands of community-maintained packages . **Best for advanced users** who want to understand every layer of their system and control exactly what's installed.

- **[Linux Mint](https://linuxmint.com/)**  
  **The conservative, Windows-like desktop distro** — more conservative than Ubuntu, less opinionated about pushing new technologies, and uses fewer system resources on MATE or Xfce . **Three desktop editions**: **Cinnamon** (flagship, modern visuals with classic panel layout), **MATE** (lightweight and stable), and **Xfce** (most resource-efficient, runs well on older hardware) . **Best for Windows refugees and users wanting a polished desktop that works out of the box.**

- **[Kali Linux](https://www.kali.org/)**  
  **The purpose-built offensive security platform** from Offensive Security, Debian-based . **600+ pre-installed security tools** for penetration testing, vulnerability assessment, network analysis, reverse engineering, and wireless intrusion detection . **Live boot from USB** without installation, multiple desktop environments, and regular updates tracking new exploits . **Not a daily driver** — its default security model reflects its offensive focus . **Best for cybersecurity professionals and penetration testers.**

### Additional Strong Open-Source Options

- **FreeBSD** — Unix-like OS based on BSD with strong networking and storage features. 2-clause BSD licensed.
- **Haiku** — BeOS-inspired open-source OS with a focus on responsiveness and a cohesive desktop experience.
- **ReactOS** — Open-source OS aiming for binary compatibility with Windows applications and drivers.
- **seL4** — Formally verified microkernel with mathematical proofs of correctness. GPL licensed.
- **xv6** — MIT's teaching OS for operating systems courses, based on Unix V6.
- **Tilck** — Tiny Linux-compatible kernel for learning and embedded use.
- **Managarm** — Pragmatic microkernel-based OS with fully asynchronous I/O.
- **Redox** — Unix-like OS written in Rust with a focus on safety and performance.
- **Fuchsia** — Google's capability-based OS with a microkernel architecture (Zircon).

**Frameworks for building custom systems**: Combine **SerenityOS** for a complete from-scratch learning platform with real hardware support, **Debian** for production servers with rock-solid stability, **Ubuntu** or **Linux Mint** for desktop accessibility, **Fedora** for modern developer toolchains, and **Arch Linux** for full system control — to build an OS stack tailored to your need for stability, learning, or bleeding-edge software.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Operating systems differ significantly in stability, hardware support, and learning curve. **SerenityOS is a from-scratch hobby OS** — it runs on real hardware and QEMU, but it is not a production replacement for Linux, Windows, or macOS . **Debian Stable is the production server choice**; Testing is for desktops needing newer packages; Sid is for developers . **Ubuntu's Snap integration and default sudo group** are conveniences Debian lacks, at the cost of Canonical's opinions . **Arch Linux gives you nothing by default** — the learning curve is the point . **Kali Linux is not a daily driver** — its offensive security focus makes it unsuitable for general use. **Hobby OSes require cross-compilation toolchains and VM testing** — do not install them on primary hardware expecting stability.
- Self-hosted open-source solutions require proper backup strategies, hardware compatibility verification, and awareness that rolling releases can introduce breakage.

---

**Made for systems programmers, OS developers, Linux administrators, and anyone who wants to understand or control the software beneath their applications.**
Let's make operating systems more open, understandable, and hackable.
