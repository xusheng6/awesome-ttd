# awesome-ttd

A curated list of resources related to Time Travel Debugging (TTD).

## Contents

- [TTD Solutions](#ttd-solutions)
- [Official Documentation](#official-documentation)
- [Tutorials and Guides](#tutorials-and-guides)
- [Videos](#videos)
- [CTF Write-ups](#ctf-write-ups)
- [Source Code](#source-code)

## TTD Solutions

A collection of Time Travel Debugging tools and platforms, both commercial and open-source.

### WinDbg TTD
- **Link**: [Microsoft WinDbg Preview](https://learn.microsoft.com/en-us/windows-hardware/drivers/debuggercmds/time-travel-debugging-overview)
- **Pricing**: Free
- **Description**: Microsoft's official Time Travel Debugging solution integrated into WinDbg Preview. Allows recording and replaying of Windows application execution for debugging complex issues. Features include reverse execution, memory and register queries at any point in time, and integration with the Windows debugging ecosystem.

### rr
- **Link**: [rr Project](https://rr-project.org/)
- **Pricing**: Free and Open Source
- **Description**: A lightweight recording and deterministic debugging tool for Linux. Developed by Mozilla, rr records native application execution and allows full reverse execution during replay. It's designed to be efficient with low overhead and integrates well with GDB for a familiar debugging experience.

### undo.io
- **Link**: [Undo](https://undo.io/)
- **Pricing**: Commercial (Contact for pricing)
- **Description**: Enterprise-grade reversible debugging platform for Linux and embedded systems. Built on the technology behind UDB (Undo Debugger), it provides time travel debugging capabilities for production systems, continuous integration, and development environments. Supports both live debugging and recording for later analysis.

### esReven
- **Link**: [esReven](https://www.codeproject.com/Articles/5365310/esReven-Reverse-Debugger)
- **Pricing**: Free
- **Description**: A reverse debugger for Windows that provides time travel debugging capabilities. Allows stepping backwards through program execution, setting reverse breakpoints, and analyzing program behavior in reverse. Designed for Windows applications with a focus on ease of use and minimal overhead.

### Panda-re
- **Link**: [PANDA - Platform for Architecture-Neutral Dynamic Analysis](https://github.com/panda-re/panda)
- **Pricing**: Free and Open Source
- **Description**: A platform for architecture-neutral dynamic analysis based on QEMU. PANDA enables whole-system recording and deterministic replay for various architectures. It's particularly useful for malware analysis, reverse engineering, and security research, offering extensive plugin support for custom analyses.

### GDB
- **Link**: [GDB Reverse Debugging](https://sourceware.org/gdb/current/onlinedocs/gdb.html/Reverse-Execution.html)
- **Pricing**: Free and Open Source
- **Description**: The GNU Debugger includes built-in reverse debugging capabilities. While not a full time travel debugging solution, GDB supports reverse execution through process recording, allowing reverse-continue, reverse-step, and reverse-next operations. Works with various targets and can be used with rr for enhanced TTD functionality.

### REnigma
- **Link**: [DTR Security REnigma](https://dtrsec.com/)
- **Pricing**: Commercial (Contact for pricing)
- **Description**: Advanced time travel debugging and reverse engineering platform. Provides comprehensive recording and analysis capabilities for security research, malware analysis, and vulnerability discovery. Features include full system state capture, advanced query capabilities, and integration with reverse engineering workflows.

## Official Documentation

- [Microsoft - Time Travel Debugging Overview](https://learn.microsoft.com/en-us/windows-hardware/drivers/debuggercmds/time-travel-debugging-overview) - Comprehensive overview of TTD in WinDbg, covering recording traces, replaying execution, and core debugging concepts.
- [Microsoft - Time Travel Debugging Object Model](https://learn.microsoft.com/en-us/windows-hardware/drivers/debuggercmds/time-travel-debugging-object-model) - Documentation on the TTD data model, including process objects, session objects, and LINQ-style queries for analyzing traces.
- [Microsoft - Time Travel Debugging Release Notes](https://learn.microsoft.com/en-us/windows-hardware/drivers/debuggercmds/time-travel-debugging-release-notes) - Release notes tracking TTD features, improvements, and known issues across WinDbg versions.
- [Binary Ninja - Time Travel Debugging (Windows)](https://docs.binary.ninja/guide/debugger/dbgeng-ttd.html) - Guide for using TTD with Binary Ninja on Windows through WinDbg/DbgEng integration.
- [Binary Ninja - Time Travel Debugging (Linux)](https://docs.binary.ninja/guide/debugger/gdbrsp-ttd.html) - Documentation for TTD support on Linux using the rr debugger with Binary Ninja.
- [IDA Pro - WinDbg TTD Debugging](https://docs.hex-rays.com/user-guide/debugger/local-debugging/windbg-ttd) - Documentation for using WinDbg Time Travel Debugging with IDA Pro for reverse engineering and malware analysis.

## Tutorials and Guides

- [Wikipedia - Time Travel Debugging](https://en.wikipedia.org/wiki/Time_travel_debugging) - Comprehensive overview of time travel debugging concepts, history, implementations, and use cases across different platforms and tools.
- [Next-Level Reversing: Binary Ninja+TTD](https://seeinglogic.com/posts/binary-ninja-ttd-intro/) - Hands-on tutorial demonstrating how to use TTD with Binary Ninja for reverse engineering, including setup, trace recording, and analysis workflows.
- [LRQA - Time Travel Debugging Shellcode with Binary Ninja](https://www.lrqa.com/en/cyber-labs/time-travel-debugging-shellcode-with-binary-ninja/) - Tutorial on using TTD to debug shellcode and non-PE targets with Binary Ninja, useful for malware analysis and vulnerability research.
- [Microsoft WinDbg-Samples TTD README](https://github.com/microsoft/WinDbg-Samples/blob/master/TTD/README.md) - Official Microsoft repository with TTD samples and example scripts for common debugging scenarios.

## Videos

- [Introduction to Working with Time Travel Debugging in Binary Ninja](https://www.youtube.com/watch?v=qNfCbuzdH6U) - Getting started video covering the basics of TTD in Binary Ninja, including installation and first steps.
- [Hands-on Time Travel Debugging Tutorial](https://www.youtube.com/watch?v=2v7DRyXb8_c) - Practical demonstration of TTD features and workflows for debugging complex applications.
- [Advanced Time Travel Debugging Techniques](https://www.youtube.com/watch?v=-eVyYB83hH0) - Advanced techniques and tips for effective use of TTD in reverse engineering.
- [TTD Walkthrough and Best Practices](https://www.youtube.com/watch?v=0PBV1ZFralk) - Comprehensive walkthrough of TTD capabilities and recommended approaches for various debugging scenarios, demonstrating analysis of the 7th challenge in Flare-On 2025.
- [Time Travel Debugging: Root Causing Bugs in Commercial Scale Software](https://www.youtube.com/watch?v=cwsVSTVBe0g) - Discussion of using TTD for debugging large-scale commercial software applications and finding root causes of complex bugs.
- [Time Travel Debugging - An Introduction](https://www.youtube.com/watch?v=HcyCZPNO3qI) - Introductory video covering the fundamentals of time travel debugging and its benefits for software development.
- [Reverse Engineering with Time Travel Debugging](https://www.youtube.com/watch?v=5GeO92F-wfY) - Demonstration of TTD techniques for reverse engineering applications and analyzing program behavior.
- [Debugging with Time Travel in WinDbg](https://www.youtube.com/watch?v=wpEoCC_FhUw) - Practical guide to using time travel debugging features in WinDbg for Windows application debugging.
- [Advanced TTD Workflows and Automation](https://www.youtube.com/watch?v=7WIPUzHg2-k) - Advanced workflows and automation techniques for time travel debugging in production environments.

## CTF Write-ups

- [Binary Ninja - FlareOn 11 TTD Challenge](https://binary.ninja/2024/12/16/flareon-ttd.html) - Write-up demonstrating the use of Binary Ninja's Time Travel Debugging capabilities to solve the FlareOn 11 CTF challenge, showcasing practical TTD techniques for reverse engineering.
- [Huntress CTF 2025 - Rust Tickler 1](https://github.com/Rurik/CTF/blob/master/Huntress_2025/rust_tickler_1.md) - Write-up for Huntress CTF 2025 Rust Tickler 1 challenge, demonstrating TTD techniques for analyzing Rust binaries.
- [Huntress CTF 2025 - Rust Tickler 2](https://github.com/Rurik/CTF/blob/master/Huntress_2025/rust_tickler_2.md) - Write-up for the second Rust Tickler challenge, showing advanced reverse engineering of Rust code with time travel debugging.
- [Huntress CTF 2025 - Rust Tickler 3](https://github.com/Rurik/CTF/blob/master/Huntress_2025/rust_tickler_3.md) - Write-up for the third and final Rust Tickler challenge, featuring complex Rust binary analysis using TTD.

## Source Code

- [Binary Ninja - DbgEng TTD Adapter](https://github.com/Vector35/debugger/blob/dev/core/adapters/dbgengttdadapter.cpp) - Source code for Binary Ninja's TTD adapter implementation, showing how Binary Ninja integrates with WinDbg's TTD engine.
- [ttd-bindings](https://github.com/commial/ttd-bindings) - Python bindings for Microsoft's Time Travel Debugging (TTD) engine, enabling programmatic access to TTD traces and analysis capabilities.
- [ttddbg](https://github.com/airbus-cert/ttddbg) - Python library for working with WinDbg TTD traces, providing tools for trace analysis, querying, and automation of TTD workflows.
