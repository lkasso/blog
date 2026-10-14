---
title: Portfolio
permalink: /portfolio/
---

## MetaWear SDKs

**Swift SDK for MetaWear** — Built with Claude Code. [GitHub](https://github.com/mbientlab/MetaWear-API-Swift)

Hardware SDKs for the MetaMotion wireless sensor platform. Full BLE transport layer, protocol implementation, all sensor modules (accelerometer, gyroscope, magnetometer, sensor fusion, barometer, GPS, LED, haptic, GPIO, timer, events, macros, serial passthrough, data processor chains, firmware OTA).

896 unit tests. Hardware integration tests on real iOS devices. iOS app with modern design (iOS 17+ Liquid Glass), Demo Mode (no hardware required), 3D orientation visualization. Structured as 4 SwiftPM products with SwiftData persistence and CSV export.

**Kotlin SDK for MetaWear** — Built with Claude Code. [GitHub](https://github.com/mbientlab/MetaWear-API-Kotlin)

Same feature set as Swift. Kotlin 2.1.20, minSdk 26, KMP-ready architecture separating protocol (pure JVM) from transport and persistence (Android).

1,275+ JVM tests. 43 BLE + 13 persistence instrumented tests, hardware-verified on Pixel 7 with MetaMotion S. Jetpack Compose app with feature parity to iOS. Includes `DemoBleTransport` — a protocol-level emulator for testing without hardware.

Both shipping, in active use at scale.

---

## Gradle Strategic Work

**Gradle Is Going Agentic** — [blog.gradle.org](https://blog.gradle.org/gradle-is-going-agentic), August 2026

Co-authored with Tom Tresansky. Lays out why build tools need to serve agents (developers increasingly have AI agents run builds, read failures, make fixes) and Gradle's three-part approach: official skills, benchmarks, and removal of friction.

**Introducing Gradle Skills** — [blog.gradle.org](https://blog.gradle.org/introducing-gradle-skills), September 2026

Co-authored with Tom Tresansky. Announces `gradle-best-practices` and `gradle-wrapper-upgrade` skills, benchmarked across 7 LLM vendors. Every model scored higher with the skill. Claude Sonnet 5 rose from 30 to 50 of 51 checks on best practices.

---

## DPE University

[dpeuniversity.gradle.com](https://dpeuniversity.gradle.com/app)

Gradle's hands-on training platform. Built course automation pipeline: Claude generates presentation + project + script; speech synthesis produces narration; assembled in Camtasia/DaVinci Resolve.

Course creation: 1 week → 1–2 days (5–7x faster).

---

## Support Systems

**Beacon Support Skill** — 1,624 Discord threads + 402 email threads. Safety policies baked in.

**MbientLab Support Skill** — Multi-language API support (Swift, Kotlin, C++, Python). 520+ real support messages.
