# StuSync Patch Repository 🚀

This repository hosts the Over-The-Air (OTA) update files for the StuSync Desktop Application.

## 🛠 How to Publish an Update

1. **Generate Patch:** Compare your new build with the old build to create `update.patch`.
2. **Update version.json:** - Increment `latest_version`.
   - Update the `changelog`.
3. **Create GitHub Release:**
   - Go to [Releases](https://github.com/Trehive/stusync-patches/releases).
   - Click **Draft a new release**.
   - Set the Tag (e.g., `v1.0.1`).
   - **Upload** `update.patch` and `updater.exe` as binary assets.
   - Publish.

## 🔗 Direct Access Links
- **Version Check:** `https://raw.githubusercontent.com/Trehive/stusync-patches/main/version.json`
- **Latest Patch:** `https://github.com/Trehive/stusync-patches/releases/latest/download/update.patch`