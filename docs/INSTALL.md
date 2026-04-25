# StuSync Installation Guide

## System Requirements

| Requirement | Minimum | Recommended |
|--------------|---------|-------------|
| OS | Windows 10 (64-bit) | Windows 11 |
| RAM | 4 GB | 8 GB |
| Storage | 10 GB free | 20 GB free |
| Display | 1280x720 | 1920x1080 |
| Internet | Optional | 10 Mbps+ for sync |

---

## Installation Steps

### 1. Download

Download the latest release from:
- **GitHub:** https://github.com/Trehive/stusync-patches/releases/latest
- **Website:** https://stusync.trehive.com/downloads

### 2. Extract

```
Download: stusync_v2.0.2.zip
Extract to: C:\Program Files\StuSync  (recommended)
```

### 3. First Launch

1. Open the StuSync folder
2. Double-click `stusync.exe`
3. The app will initialize for first launch

### 4. Activation

1. **Enter License Key** — Contact Trehive to obtain your institutional license
2. **Device Registration** — Automatically bound to your machine
3. **Set Admin Credentials** — Create administrator username/password
4. **Configure School** — Enter school name, code, academic year

### 5. Initial Setup

- Configure grades and sections
- Set up fee structure
- Add staff and students
- (Optional) Connect to cloud sync

---

## Upgrading

### Auto-Update (Recommended)

1. The app will prompt when an update is available
2. Click **Update Now**
3. The app downloads and applies the patch automatically
4. On first launch, database migrations run automatically

### Manual Update

1. Download the latest `stusync_vx.x.x.zip`
2. Back up your database: `Settings → Backup → Create Backup`
3. Close the app completely
4. Extract new files, overwrite existing
5. Run `stusync.exe`
6. Database migrates automatically

---

## Running the App

### Command Line (Optional)

```batch
:: Run with custom data folder
stusync.exe --data-path="D:\MySchoolData"

:: Run with debug logging
stusync.exe --debug
```

### Quick Launch

Create a shortcut:
1. Right-click `stusync.exe`
2. Send to Desktop (create shortcut)
3. Double-click shortcut to launch

---

## Data Backup

### Manual Backup

**Settings → Backup → Create Backup**

Creates an encrypted `.stusync` backup file with:
- Full database (AES-256 encrypted)
- All media files
- Automatic rotation (keeps last 3 backups)

### Auto-Backup

The app automatically creates backups:
- Daily (if connected)
- Before every update

### Restore from Backup

**Settings → Backup → Restore**

1. Select backup file
2. Confirm restore
3. App restarts with restored data

---

## Troubleshooting

### "License Not Found"

- Verify your license key is correct
- Contact Trehive if license is lost

### "Device Not Registered"

- Contact Trehive to register your device
- Provide your machine ID (shown in error)

### "Database Corrupted"

- Restore from backup
- If no backup, contact Trehive support

### "Sync Failed"

- Check internet connection
- Verify Supabase credentials
- Try manual sync later

---

## Uninstallation

1. **Back up your data** (very important!)
2. Delete the StuSync folder
3. Delete `%APPDATA%\StuSync` (optional)
4. Remove any shortcuts

> [!WARNING]
> Uninstalling without backing up your data will result in permanent data loss. Always create a backup before uninstalling.

---

## Support

| Channel | Details |
|---------|---------|
| Email | trehiveofficial@gmail.com |
| Phone | +977-9741802381 |
| Website | https://stusync.trehive.com/support |

---

*© 2024–2026 Trehive*