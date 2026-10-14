---
title: Portfolio
permalink: /portfolio/
---

## Claude Code

**Swift SDK for MetaWear** — Built with Claude Code. [GitHub](https://github.com/mbientlab/MetaWear-API-Swift)

Hardware SDKs for the MetaMotion wireless sensor platform. Full BLE transport layer, protocol implementation, all sensor modules (accelerometer, gyroscope, magnetometer, sensor fusion, barometer, GPS, LED, haptic, GPIO, timer, events, macros, serial passthrough, data processor chains, firmware OTA).

896 unit tests. Hardware integration tests on real iOS devices. iOS app with modern design (iOS 17+ Liquid Glass), Demo Mode (no hardware required), 3D orientation visualization. Structured as 4 SwiftPM products with SwiftData persistence and CSV export.

**Kotlin SDK for MetaWear** — Built with Claude Code. [GitHub](https://github.com/mbientlab/MetaWear-API-Kotlin)

Same feature set as Swift. Kotlin 2.1.20, minSdk 26, KMP-ready architecture separating protocol (pure JVM) from transport and persistence (Android).

1,275+ JVM tests. 43 BLE + 13 persistence instrumented tests, hardware-verified on Pixel 7 with MetaMotion S. Jetpack Compose app with feature parity to iOS. Includes `DemoBleTransport` — a protocol-level emulator for testing without hardware.

Both shipping, in active use at scale.

---

## Claude Ecosystem

**MCP Server: Career Timeline & Posts** — [mcp.laura.kassovic.com](https://mcp.laura.kassovic.com/)

Static site MCP server exposing career data via standard MCP tools. Schemas for `get_career_timeline` (all roles), `get_role` (by company), `list_posts` (all posts), `list_posts_for_era` (posts by era), `get_about` (bio). Runs on Jekyll; data sourced from `_data/journey.json` and `_posts/`. Tool discovery via `/mcp.json` manifest. Enables Claude or any MCP client to programmatically query structured career information.

---

## Agent Skills

**Beacon Support Skill** — 1,624 Discord threads + 402 email threads. Safety policies baked in.

**MbientLab Support Skill** — Multi-language API support (Swift, Kotlin, C++, Python). 520+ real support messages indexed and searchable.

**Introducing Gradle Skills** — [blog.gradle.org](https://blog.gradle.org/introducing-gradle-skills), September 2026

Co-authored with Tom Tresansky. `gradle-best-practices` audits builds against official best practices, proposes or applies fixes. `gradle-wrapper-upgrade` handles wrapper upgrades, pins checksums, verifies builds, rolls back on failure. Benchmarked across 7 LLM vendors. Claude Sonnet 5 rose from 30 to 50 of 51 checks with the skill enabled.

---

## Strategic Work

**Gradle Is Going Agentic** — [blog.gradle.org](https://blog.gradle.org/gradle-is-going-agentic), August 2026

Co-authored with Tom Tresansky. Positions Gradle for agents as first-class users. Agents increasingly run builds, read failures, propose fixes. Gradle's approach: official skills (teach agents the right patterns), benchmarks (measure whether skills work), friction removal (clearer errors, less token waste).

**AI Policy** — [github.com/gradle/gradle](https://github.com/gradle/gradle/blob/master/AI_POLICY.md)

Co-authored. Guidelines for AI-assisted contributions to Gradle. Requires contributors to understand and justify their submissions. Disclosure of significant AI involvement. Human review and judgment as final gate on all contributions. Enforcement against low-effort AI-generated content and non-engagement in review.

---

## Training & Enablement

**DPE University** — [dpeuniversity.gradle.com](https://dpeuniversity.gradle.com/app) | [YouTube Playlist](https://www.youtube.com/watch?v=QHb8nUQzw2s&list=PLLQbIfXVLZqHM_0cKVezM9vNoNzN_orfr)

Gradle's hands-on training platform. Built course automation pipeline: Claude generates presentation slides + hands-on project + instructor script. `moss-tts-8b` synthesizes narration with voice cloning (your voice, not generic TTS). Assembled in Camtasia/DaVinci Resolve.

Course creation: 1 week → 1–2 days (5–7x faster). Covers Gradle fundamentals, build optimization, enterprise patterns.

---

## Public Speaking & Advocacy

**Sensors Expo & Conference 2018** — [Speaker Schedule](https://sensorsexpoconference2018.sched.com/speaker/laura_kassovic.1y39etiq)

Spoke on MetaWear wearable sensor platform capabilities, wireless protocols, real-world IoT applications.

**Medical Sensors Design Conference 2018** — [Speaker Schedule](https://medicalsensorsdesignconfere2018.sched.com/speaker/laura_kassovic.1y0nliqc)

Presented on miniaturized wearable sensors, medical-grade BLE design, data accuracy in motion sensing for health applications.

**Arm Innovator Series** — [Hackster.io Video](https://www.hackster.io/videos/197)

Interview on MetaWear platform: size and washability improvements, Bluetooth 5 capabilities for long-range wireless sensors, power efficiency gains, real-world deployment in health and fitness.

**AEC Business Interview: "Sensors for Smarter Construction"** — [Podcast](https://aec-business.com/sensors-smarter-construction-interview-laura-kassovic-mbientlab/), November 2016

Discussed three areas where wearables improve construction sites: worker safety monitoring (real-time health signals), insurance (accident data collection), workflow efficiency (hands-free data entry). MbientLab manufacturing model and sensor reliability at scale.

---
