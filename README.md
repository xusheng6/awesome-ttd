# awesome-ttd

A curated list of resources related to Time Travel Debugging (TTD).

## Contents

- [Official Documentation](#official-documentation)
- [Tutorials and Guides](#tutorials-and-guides)
- [Videos](#videos)
- [CTF Write-ups](#ctf-write-ups)
- [Source Code](#source-code)

## Official Documentation

- [Microsoft - Time Travel Debugging Overview](https://learn.microsoft.com/en-us/windows-hardware/drivers/debuggercmds/time-travel-debugging-overview) - Comprehensive overview of TTD in WinDbg, covering recording traces, replaying execution, and core debugging concepts.
- [Microsoft - Time Travel Debugging Object Model](https://learn.microsoft.com/en-us/windows-hardware/drivers/debuggercmds/time-travel-debugging-object-model) - Documentation on the TTD data model, including process objects, session objects, and LINQ-style queries for analyzing traces.
- [Microsoft - Time Travel Debugging Release Notes](https://learn.microsoft.com/en-us/windows-hardware/drivers/debuggercmds/time-travel-debugging-release-notes) - Release notes tracking TTD features, improvements, and known issues across WinDbg versions.
- [Binary Ninja - Time Travel Debugging (Windows)](https://docs.binary.ninja/guide/debugger/dbgeng-ttd.html) - Guide for using TTD with Binary Ninja on Windows through WinDbg/DbgEng integration.
- [Binary Ninja - Time Travel Debugging (Linux)](https://docs.binary.ninja/guide/debugger/gdbrsp-ttd.html) - Documentation for TTD support on Linux using the rr debugger with Binary Ninja.

## Tutorials and Guides

- [Next-Level Reversing: Binary Ninja+TTD](https://seeinglogic.com/posts/binary-ninja-ttd-intro/) - Hands-on tutorial demonstrating how to use TTD with Binary Ninja for reverse engineering, including setup, trace recording, and analysis workflows.
- [LRQA - Time Travel Debugging Shellcode with Binary Ninja](https://www.lrqa.com/en/cyber-labs/time-travel-debugging-shellcode-with-binary-ninja/) - Tutorial on using TTD to debug shellcode and non-PE targets with Binary Ninja, useful for malware analysis and vulnerability research.
- [Microsoft WinDbg-Samples TTD README](https://github.com/microsoft/WinDbg-Samples/blob/master/TTD/README.md) - Official Microsoft repository with TTD samples and example scripts for common debugging scenarios.

## Videos

- [Introduction to Working with Time Travel Debugging in Binary Ninja](https://www.youtube.com/watch?v=qNfCbuzdH6U) - Getting started video covering the basics of TTD in Binary Ninja, including installation and first steps.
- [Hands-on Time Travel Debugging Tutorial](https://www.youtube.com/watch?v=2v7DRyXb8_c) - Practical demonstration of TTD features and workflows for debugging complex applications.
- [Advanced Time Travel Debugging Techniques](https://www.youtube.com/watch?v=-eVyYB83hH0) - Advanced techniques and tips for effective use of TTD in reverse engineering.
- [TTD Walkthrough and Best Practices](https://www.youtube.com/watch?v=0PBV1ZFralk) - Comprehensive walkthrough of TTD capabilities and recommended approaches for various debugging scenarios.

## CTF Write-ups

- [Huntress CTF 2025 - Rust Tickler 1](https://github.com/Rurik/CTF/blob/master/Huntress_2025/rust_tickler_1.md) - Write-up for Huntress CTF 2025 Rust Tickler 1 challenge, demonstrating TTD techniques for analyzing Rust binaries.
- [Huntress CTF 2025 - Rust Tickler 2](https://github.com/Rurik/CTF/blob/master/Huntress_2025/rust_tickler_2.md) - Write-up for the second Rust Tickler challenge, showing advanced reverse engineering of Rust code with time travel debugging.
- [Huntress CTF 2025 - Rust Tickler 3](https://github.com/Rurik/CTF/blob/master/Huntress_2025/rust_tickler_3.md) - Write-up for the third and final Rust Tickler challenge, featuring complex Rust binary analysis using TTD.

## Source Code

- [Binary Ninja - DbgEng TTD Adapter](https://github.com/Vector35/debugger/blob/dev/core/adapters/dbgengttdadapter.cpp) - Source code for Binary Ninja's TTD adapter implementation, showing how Binary Ninja integrates with WinDbg's TTD engine.
