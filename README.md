# 🦉 OMem

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OForensics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.1-cyan?style=flat-square"/>
</p>

> **OMem** — Volatile Memory Forensic Analyser

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OMem is a volatile memory forensic analyser for Debian-based Linux. It supports live RAM inspection (root required) and offline analysis of saved `.raw` dumps for strings, entropy, and IOC scanning, with dump listing under `~/.omem/dumps`. Reports and chain-of-custody style logging are available from the interactive workflow.

---

## ✨ Features

- Live memory forensics on Debian-based systems (root / privileged access required)
- Offline analysis of saved `.raw` dumps without live PID attachment
- Modes: strings (ASCII/UTF-16 mining), entropy analysis, and IOC scanning
- List previously saved dumps under `~/.omem/dumps`
- Pattern search, heap inspection, network artefact extraction, and YARA-lite style matching in the interactive tool
- Integrity hashing (SHA-256 / MD5) and JSON/CSV/TXT report paths from the full workflow

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OMem --offline ~/mem.raw --mode strings
./OMem --offline dump.raw --mode ioc
./OMem --list-dumps
./OMem --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled.s.Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
