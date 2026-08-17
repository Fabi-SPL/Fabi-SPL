# Fabi

**Software engineer. Backend, data pipelines and automation.**

TypeScript, Python, PostgreSQL, self-hosted infrastructure. I build systems that run unattended and the deployment around them.

### What I work on

- Backend services and REST APIs in TypeScript and Python
- Data pipelines: scraping, extraction, validation, scheduled jobs on `pg_cron`
- Self-hosted Postgres and Supabase: RLS, partitioning, PostGIS, pgvector
- Native iOS apps in SwiftUI, CI/CD on GitHub Actions
- Undocumented protocols and vendor APIs: BLE, SOAP, WebRTC, packet captures when there are no docs
- MCP servers and LLM API integration where it solves a real problem

### Stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat&logo=swift&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat&logo=playwright&logoColor=white)

### Public work

**TypeScript and Node**

- **[argus](https://github.com/Fabi-SPL/argus)** · One control plane over four vendor APIs that share nothing: devolo powerline on OpenWrt, NETGEAR over SOAP, Telekom Speedport on Sercomm firmware, and Tailscale over REST. A driver registry normalises them, and a `guard` layer refuses writes to protected bands before the driver is ever called. A survey of 31 comparable projects turned up none doing all four.
- **[kontist-mcp](https://github.com/Fabi-SPL/kontist-mcp)** · Typed GraphQL layer over a German business bank. The hard part is the auth chain: the long-lived refresh token sits behind interactive consent plus an MFA push, so it has to be captured once through a local callback server and then treated as the only credential worth persisting. Transfers are deliberately not exposed.
- **[uiverse-mcp](https://github.com/Fabi-SPL/uiverse-mcp)** · 3,800 UI components indexed and searchable from any MCP client, with a cache layer so a cold start does not hit the upstream repo.

**Swift**

- **[whoop-ble-swift](https://github.com/Fabi-SPL/whoop-ble-swift)** · The BLE protocol for a WHOOP 4.0 strap, worked out from packet captures and implemented as a standalone package. Framing, CRC, command encoding, historical-record parsing. 42 tests, green CI.
- **[lucid-health](https://github.com/Fabi-SPL/lucid-health)** · iOS app plus a correlation server and a BLE bridge to that strap. Deliberately keeps every scoring decision off the device.
- **[lucid-ride](https://github.com/Fabi-SPL/lucid-ride)** · SwiftUI, distributed through AltStore PAL. The telemetry comes off a tracker I built and bolted to the bike: a hand soldered ESP8266 and BNO085 IMU in a 3D printed enclosure I modelled around those components, logging at 25 Hz to onboard flash in its own binary format, joining my phone hotspot on the road for an NTP clock and live upload. The app joins that against health data by ride window. Firmware stays private, it is written against one board and one wiring diagram.

**Python**

- **[remote-desktop](https://github.com/Fabi-SPL/remote-desktop)** · Screen streaming to a plain browser tab over WebRTC, with NVENC swapped in for libx264 and a NAL-aware bitstream splitter replacing one that corrupted every keyframe. Worth reading for the bug I got wrong: I wrote an RTP send pacer, measured 50 consecutive 3.2 ms sleeps consuming 756 ms of wall clock against Windows' 15.6 ms timer granularity, and deleted it. The README documents the deletion rather than hiding it.

If you only open one, open **remote-desktop** for the debugging or **argus** for the architecture.

Most of my work lives in private client and product repos.

---

I use AI where it solves a problem. The work itself is engineering: error handling, measurement, deployment, operations.

📍 Germany · 🌐 [lucidailabs.com](https://lucidailabs.com) · ✉️ Fabi@lucidailabs.com
