<div align="center">

# StuSync Patch Repository 🏫

**Over-The-Air (OTA) Update Distribution for the StuSync Desktop Application**

[![Latest Release](https://img.shields.io/github/v/release/Trehive/stusync-patches?style=for-the-badge&color=blue)](https://github.com/Trehive/stusync-patches/releases/latest)
[![License](https://img.shields.io/badge/License-Enterprise-red?style=for-the-badge)](mailto:insert@email.com)
[![Platform](https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows)](https://github.com/Trehive/stusync-patches/releases/latest)

</div>

---

> [!IMPORTANT]
> **Enterprise License Required**
> StuSync is a specialized management suite for educational institutions. Access requires a **Hardware-Linked License Key** and verified administrator credentials.
>
> To request an activation key or discuss a plan for your institution, contact the Trehive Team:
> * 📧 **Email:** [trehiveofficial@gmail.com]
> * 🌐 **Website:** [https://stusync.trehive.com]

---

## 📖 Table of Contents

- [What is StuSync?](#-what-is-stusync)
- [Current Release](#-current-release)
- [Release History](#-release-history)
- [How to Install](#-how-to-install)
- [How to Publish an Update](#️-how-to-publish-an-update)
- [Direct Access Links](#-direct-access-links)
- [Contact & Licensing](#-contact--licensing)

---

## 🏫 What is StuSync?

StuSync is an **offline-first, multi-device school management desktop application** built for educational institutions. It handles the full lifecycle of school operations — from student registration and academic management to fee collection, staff tracking, and real-time campus monitoring.

**Key Capabilities:**
- 👨‍🎓 Student & Staff Registry with full profile management
- 📚 Academic setup — subjects, class assignments, grading systems, marks entry
- 💰 Finance module — fee billing, invoicing, scholarships, expense tracking
- 📡 Cloud sync with conflict-aware multi-device support (Supabase)
- 🔒 Hardware-linked licensing with device registry security
- 📷 CCTV live feed integration and secondary dashboard
- 🚌 Transport route and GPS management

---

## 🚀 Current Release

### Beta v1.1.5+10 — "The Academic Structure Update"

> Staff assignment, subject ordering, bulk class operations, and sync engine hardening.

| Property | Value |
|---|---|
| Version | `beta_v1.1.5+10` |
| Database Schema | `v3` |
| Platform | Windows (Desktop) |
| Release Date | March 2026 |

**Highlights:**
- 👨‍🏫 Staff subject assignment with bulk select and section support
- 📚 Subject display order index for consistent sequencing across all screens
- ✅ Bulk select/delete for class subject setup
- 🔢 Typeable float credit hours (supports values like `1.25`)
- 🛡️ Conflict-aware upserts for all configuration tables in sync engine
- 🔄 Offline conflict protection on pull for `grading_systems`, `fee_categories`, `expense_categories`, `transport_stops`

[→ View Full Release Notes](https://github.com/Trehive/stusync-patches/releases/latest)

---

## 📋 Release History

| Version | Codename | Highlights |
|---|---|---|
| `beta_v1.1.5+10` | Academic Structure | Staff assignment, subject ordering, bulk operations, sync hardening |
| `beta_v1.1.4+9` | Data Integrity | Unique constraints, duplicate prevention, smart sync |
| `beta_v1.1.0+5` | Security & Oversight | CCTV integration, hardware licensing, secondary dashboard |

---

## 📥 How to Install

### Fresh Installation
1. Download `stusync_v1.1.5+10.zip` from the [latest release](https://github.com/Trehive/stusync-patches/releases/latest)
2. Extract the zip to your desired folder
3. Run `stusync.exe`
4. On first launch, enter your **Institution License Key** when prompted
5. Log in with your administrator credentials

### Upgrading from a Previous Version
1. Download the latest `update.patch` from the [latest release](https://github.com/Trehive/stusync-patches/releases/latest)
2. Run `updater.exe` — it will apply the patch automatically
3. On first launch after upgrade, the database will auto-migrate to the new schema version
4. Perform a **Full Sync** after upgrading to align with the latest cloud state

> [!WARNING]
> Always back up your database before upgrading. The app will prompt you automatically, but manual backups are recommended for large deployments.

---

## 🛠️ How to Publish an Update

> For internal Trehive team use.

1. **Generate Patch**
   Compare your new build with the previous build to produce `update.patch`

2. **Update `version.json`**
   ```json
   {
     "latest_version": "1.1.5+10",
     "changelog": "Staff assignment, subject ordering, bulk operations",
     "patch_url": "https://github.com/Trehive/stusync-patches/releases/latest/download/update.patch"
   }
   ```

3. **Create GitHub Release**
   - Go to [Releases](https://github.com/Trehive/stusync-patches/releases)
   - Click **Draft a new release**
   - Set the tag (e.g., `beta_v1.1.5+10`)
   - Upload `update.patch` and `updater.exe` as binary assets
   - Paste the release notes and publish

---

## 🔗 Direct Access Links

| Resource | URL |
|---|---|
| Version Check | `https://raw.githubusercontent.com/Trehive/stusync-patches/main/version.json` |
| Latest Patch | `https://github.com/Trehive/stusync-patches/releases/latest/download/update.patch` |
| Latest Installer | `https://github.com/Trehive/stusync-patches/releases/latest/download/updater.exe` |

---

## 📞 Contact & Licensing

StuSync is developed and maintained by **Trehive**. To activate your institution's license or get support:

| Channel | Details |
|---|---|
| 📧 Email | [trehiveofficial@gmail.com] |
| 🌐 Website |[https://stusync.trehive.com] |
| 🐛 Bug Reports | [Open an Issue](https://github.com/Trehive/stusync-patches/issues) |

> *"Offline-first apps are not about caching — they are about trust."*
> — Trehive Dev Team

---

<div align="center">
<sub>Built with ❤️ by Trehive · StuSync is proprietary software · All rights reserved</sub>
</div>
