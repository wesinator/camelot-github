<div align="center">
<a href="https://camelot-os.h2lab.org">
<img alt="redpesk®" src="../images/camelot-OS.png" style="width:30%;">
<br>
</a>
</div>

# A light and secure Operating System for microcontrolers

Camelot-OS is an open-source operating system ecosystem designed to bring strong security guarantees, robust isolation, and industrial-grade engineering practices to modern IoT and embedded systems. Camelot-OS is the successor of the initial ANSSI [Wookey](https://github.com/wookey-project) project and Ledger [Outpost-OS](https://github.com/outpost-os) developments.

Built from the ground up with security in mind, Camelot-OS targets microcontroller-based devices that require more than traditional RTOSes can safely provide — without sacrificing openness, performance, or developer control.

Camelot-OS minimizes the Trusted Computing Base (TCB) using a micro-kernel architecture. Critical services are isolated, reducing the impact of vulnerabilities and making formal reasoning about security possible.

*Strong Isolation*

Applications, drivers, and services run in separated compartments with explicit communication channels, limiting lateral movement and fault propagation.

*Modular & Composable*

Camelot-OS is not a monolith. It is an ecosystem of well-defined components — kernel, SDK, tooling - designed to be assembled according to your product’s needs.

*Industry-Grade Engineering*

The project adopts modern toolchains, reproducible builds, and traceable artifacts, enabling long-term maintenance and compliance with industrial and regulatory constraints.

*Open & Auditable*

All components are developed in the open under permissive licenses, allowing independent audits, community contributions, and transparent security review.

## Camelot-OS

**Core components**

   * [sentry-kernel](https://github.com/camelot-os/sentry-kernel) The Camelot-OS Secure kernel
   * [shield](https://github.com/camelot-os/shield) The Camelot-OS runtime for C and Rust applications
   * [merlin](https://github.com/camelot-os/merlin) The userspace driver framework to help with user drivers implementations

**Camelot build tools**

   * [camelot-barbican](https://github.com/camelot-os/barbican) The one project manager for Camelot-OS
   * [camelot-builder](https://github.com/camelot-os/camelot-builder) Camelot-OS docker image to build projects easily

**Camelot SDK**

   * [camelot-sdk](https://github.com/camelot-os/camelot-sdk) The Camelot core SDK repository

**Camelot security advisories**

   * [camelot-advisories](https://github.com/camelot-os/camelot-advisories) Advisories database for all Camelot-OS components

## Camelot BSPs

Public user-space drivers for various SoCs

   * ST [USB-OTG-FS](https://github.com/camelot-os-bsp/libdrv-st-usbotg) USB "on-the-go" full-speed drivers for STM32 family
   * ST [USART](https://github.com/camelot-os-bsp/libdrv-st-usart) driver for all STM32 family

## Camelot public projects

Examples projects that can be used and modified if needed

   * [calculator](https://github.com/camelot-os/project-calculator) serial-line simple calculator shell
   * [sha2-demo](https://github.com/camelot-os/project-calculator) two task exchanging strings and their sha256 calculation using [libecc](https://github.com/libecc/libecc) cryptographic library
