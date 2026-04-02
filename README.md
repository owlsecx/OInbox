# 📧 OInbox

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-OForensics%20%2F%20Email%20Analysis-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-None%20(Standalone)-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v2.0-cyan?style=flat-square"/>
</p>

> **OInbox** is a forensic email header analyzer specialized in detecting phishing and spoofing attempts. It parses raw email headers, evaluates SPF/DKIM/DMARC authentication, traces the hop path, calculates a risk score, and identifies suspicious indicators such as Reply-To mismatch or unusual routing.

---

## 📌 Overview

OInbox performs deep analysis of email headers to help investigators determine if an email is legitimate or a phishing/spoofing attempt. It supports interactive paste, single file (.eml/.txt), and batch folder analysis.

---

## 🖥️ Modules

| # | Module                  | Description |
|---|-------------------------|-------------|
| **[1]** | **Analyze Paste**       | Paste raw email headers interactively |
| **[2]** | **Analyze File**        | Load and analyze .eml or .txt header file |
| **[3]** | **Batch Analyze**       | Process entire folder of .eml/.txt files |
| **[4]** | **Last Results**        | View the most recent analysis output |
| **[5]** | **Export**              | Save report as JSON or CSV |
| **[6]** | **Settings**            | Configure output directory and risk scoring weights |

---

## 📊 Key Features

- **Authentication Analysis** — SPF, DKIM, DMARC, ARC with pass/fail/softfail detection
- **Hop Path Tracing** — Full Received header chain with timestamps and delays
- **Risk Scoring Engine** — Weighted scoring (0-100) with CRITICAL/HIGH/MEDIUM/LOW levels
- **Spoofing Detection** — Reply-To domain mismatch, Return-Path vs From mismatch
- **Suspicious Indicators** — X-Mailer anomalies, unusual hop count, large transit delays
- **Timing Analysis** — Transit delays between hops
- **Originating IP Extraction** — Identification of source server/IP
- **Batch Processing** — Analyze multiple emails and generate CSV summary
- **JSON/CSV Export** — Structured forensic reports

---

## ⚙️ Requirements

- **Linux or Windows**
- **No additional dependencies** — uses only Python standard library

---

## 🚀 Usage

```bash
./OInbox

📁 Output

Live Analysis — Color-coded risk level, authentication results, hop path visualization
Risk Assessment — Detailed score breakdown with contributing indicators
Hop Path — Sequential server routing with private IP detection and delays
JSON Reports — oheader_YYYYMMDD_HHMMSS.json (full structured data)
Batch CSV — oheader_batch_YYYYMMDD_HHMMSS.csv (summary of multiple emails)


📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.

AUTHORISED FORENSIC EMAIL HEADER ANALYSIS USE ONLY
