# 🦉 OInbox

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OForensics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.1-cyan?style=flat-square"/>
</p>

> **OInbox** — Phishing Email Header Analyzer

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OInbox analyses phishing and suspicious email headers with SPF, DKIM, DMARC, ARC, hop-path, and spoofing checks. It scores risk, flags lookalike domains, and can optionally enrich with GeoIP. Single-file and batch folder modes plus JSON output support SOC triage of .eml evidence.

---

## ✨ Features

- Parse raw .eml/.txt headers for authentication results
- SPF, DKIM, DMARC, and ARC oriented validation signals
- Hop-path reconstruction and spoofing/lookalike detection
- Risk scoring with attachment-aware context
- Optional GeoIP lookup (off by default)
- Batch folder analysis and JSON stdout for pipelines

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OInbox --file suspicious.eml
./OInbox --batch ./eml_inbox --json
./OInbox --file note.eml --geoip
./OInbox --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

Proprietary — © 2026 Owlsec LLC. All rights reserved.

*Tools are distributed as pre-built executables. Source code is proprietary.*
