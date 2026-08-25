# 🚀 NextMove OMS — Official Release Channel

Welcome to the official release repository for **NextMove OMS** (Modern Order & Warehouse Management System for Multi-Channel E-Commerce).

This repository distributes production Windows installers, update packages, and release changelogs.

---

## 📥 Download Latest Release

👉 **[Download NextMove OMS (Latest)](https://github.com/daksyfashion/nextmove-releases/releases/latest)**

| Package | Installer File | Size | Purpose |
| :--- | :--- | :--- | :--- |
| **Full Setup (Offline)** | [NextMove OMS.exe](https://github.com/daksyfashion/nextmove-releases/releases/latest) | Complete self-contained setup with PostgreSQL, Redis & MinIO S3 included. |
| **Update Setup (Update)** | [NextMove OMS update.exe](https://github.com/daksyfashion/nextmove-releases/releases/latest) | Fast update for systems with existing NextMove runtime installed. |

---

## 💻 System Requirements

- **Operating System**: Windows 10 / Windows 11 / Windows Server 2019+ (64-bit)
- **Processor**: Intel Core i3 / AMD Ryzen 3 or higher
- **RAM**: Minimum 4 GB (8 GB Recommended)
- **Disk Space**: 2 GB free disk space (Preferably on `D:\` drive for business data)

---

## ⚡ Installation Guide

1. Download **`NextMove OMS.exe`** from the [Releases](https://github.com/daksyfashion/nextmove-releases/releases) page.
2. Right-click the `.exe` and select **Run as Administrator**.
3. **Select Data Storage Location**:
   - By default, NextMove OMS stores all database records and files in **`D:\NextMoveData`** *(or `C:\NextMoveData` if D:\ is unavailable)*.
   - Keeping business data on `D:\` ensures your orders, inventory, and invoices remain 100% safe during Windows re-installation.
4. Click **Install**.
5. Once complete, NextMove OMS will launch automatically in your default browser at:
   - 🌐 **Web UI**: `http://localhost:3030`
   - ⚡ **API Service**: `http://localhost:4040`

---

## 🔄 In-App Automatic Updates

NextMove OMS comes with an automated update manager:
- When a new version is published to this repository, you will receive an animated **`✨ Update Available`** notification in the topbar.
- Click the notification or go to **Settings ➔ Updates** to view the changelog and update with a single click.

---

## 🛡️ Business Data Safety & Isolation

NextMove OMS separates software binaries from your business database:
- **Application Binaries**: `C:\Program Files\NextMove OMS\`
- **Database & Storage**: `D:\NextMoveData\`
  - `\postgres\` — PostgreSQL Database (Orders, Inventory, Accounts)
  - `\redis\` — Job Queue & Cache Engine
  - `\storage\` — MinIO S3 Uploaded Invoices, Labels & Documents
  - `\logs\` — Service activity logs

> 💡 *Uninstalling or updating NextMove OMS will NEVER delete or modify your data in `D:\NextMoveData`.*

---

## 📞 Support & Documentation

For setup assistance, enterprise deployment, or issue reporting:
- **Website**: 
- **Support Email**: nexera.oms@gmail.com
- **Repository Issues**: [Report an Issue](https://github.com/daksyfashion/nextmove-releases/issues)

---
© 2026 NextMove OMS. All rights reserved.
