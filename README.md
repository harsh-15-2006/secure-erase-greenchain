# 🔒 GreenChain - Secure Data Wiping with Blockchain Verification

![License](https://img.shields.io/badge/license-MIT-green)
![Python](https://img.shields.io/badge/python-3.8+-blue)
![Blockchain](https://img.shields.io/badge/blockchain-Polygon-purple)

> **Smart India Hackathon 2025 - Problem Statement SIH25070**

---

## 🎯 Problem Statement

Data breaches from discarded IT assets cost companies millions. Over **40% of used hard drives** sold online contain recoverable sensitive data. Current solutions lack:
- ❌ Verifiable proof of data destruction
- ❌ Trustworthy audit trails
- ❌ Eco-friendly recycling integration

---

## 💡 Our Solution: GreenChain

GreenChain is a **blockchain-verified secure data wiping platform** that:

1. 🔍 **Intelligently detects** drive type (HDD/SSD)
2. 🔒 **Applies appropriate wiping method** (ATA Secure Erase for SSDs, DoD/NIST for HDDs)
3. 📄 **Generates tamper-proof certificates** with unique cryptographic hashes
4. 🔗 **Anchors proof on Polygon blockchain** for immutable verification
5. 📱 **Creates QR "GreenPass"** for physical asset verification
6. ♻️ **Promotes eco-friendly recycling** of IT assets

---

## ✨ Key Features

### 🔐 Intelligent Wiping
- **Auto-detects** drive type (HDD vs SSD)
- **SSD:** Uses ATA Secure Erase (hardware-level, fastest)
- **HDD:** Uses DoD 5220.22-M, NIST 800-88, or Quick Wipe

### 🔗 Blockchain Verification
- Certificate **hash stored on Polygon Mumbai testnet**
- **Immutable, public, verifiable proof** of wipe
- Perfect for **GDPR, HIPAA, and audit compliance**

### 📱 GreenPass QR Code
- **Physical verification** for recycled drives
- Scan with any phone to instantly verify
- Shows wipe certificate, time, and blockchain proof

### 🌐 Web Dashboard
- Clean, professional **user interface**
- **Real-time progress** tracking
- **Instant certificate** generation and QR code display

---

## 🏗️ Architecture
┌─────────────────────────────────────────────────────────────┐
│ GreenChain System │
├─────────────────────────────────────────────────────────────┤
│ │
│ ┌─────────────┐ ┌──────────────────────────────────┐ │
│ │ Web UI │ │ Python Backend (Flask) │ │
│ │ Dashboard │◄──►│ • Drive Detection (psutil) │ │
│ │ │ │ • Wipe Engine │ │
│ │ • Drive │ │ • Certificate Generation │ │
│ │ Selection │ │ • QR Code Creation │ │
│ │ • Progress │ └───────────────┬──────────────────┘ │
│ │ • Results │ │ │
│ └─────────────┘ │ │
│ ▼ │
│ ┌──────────────────────────────────┐ │
│ │ Blockchain Layer │ │
│ │ • Polygon Mumbai Testnet │ │
│ │ • SHA-256 Hash Storage │ │
│ │ • Immutable Verification │ │
│ └──────────────────────────────────┘ │
│ │
└─────────────────────────────────────────────────────────────┘
