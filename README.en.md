# Vault App
#English


[![Flutter](https://img.shields.io/badge/Flutter-3.41.4-blue)](https://flutter.dev)

[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

[![Platform](https://img.shields.io/badge/Platform-Android-brightgreen)](https://www.android.com)

[![Release](https://img.shields.io/github/v/release/ySyndevL/vault-app-dist?label=Latest%20Release)](https://github.com/ySyndevL/vault-app-dist/releases)



「🔐 A secure local password manager for Android with AES-256 encryption, multi-language support & backup features」



<div align="center">

<img width="500" alt="image" src="https://github.com/user-attachments/assets/3d914615-31b3-4621-a2bb-5afde23b18f0" />

</div>



---

```

**Password Tips**:
- ✅ Use at least 12 characters.
- ✅ Include uppercase, lowercase, numbers, and symbols.
- ✅ Avoid personal info (names, birthdays).

### 2. Adding a Password
1. Go to the **Passwords** tab.
2. Tap the **+** button in the bottom right.
3. Fill in the details (Website, Username, Password, Notes).
4. Tap **Save**.

### 3. Managing Entries
- **Search**: Use the search bar at the top for real-time filtering.
- **Edit**: Tap any entry to modify and save.
- **Delete**: Long-press or swipe an entry to delete.
- **Copy**: Tap the icon next to the password field for instant clipboard copy.

### 4. Backing Up Data
**Backups are essential!** To create one:
1. Open the sidebar (☰ menu).
2. Tap **Backup**.
3. Choose your format:
   - **.vault**: Most secure, encrypted format.
   - **CSV/Excel**: For external viewing.
4. Save the file to a safe location (External drive, encrypted cloud, etc.).

---

## ⚙️ Settings & Customization

- **Change Master Password**: Sidebar → Settings → Change Master Password. (Requires current password).
- **Switch Language**: Sidebar → Settings → Language. Changes apply instantly.
- **Clear All Data**: ⚠️ **Warning**: This action is irreversible. Sidebar → Settings → Clear All Data.

---

## 🐛 Troubleshooting

### Q: I forgot my Master Password!
**A**: Unfortunately, there is no recovery option. For security reasons, the app does not support password resets. You must reinstall the app and start over.

### Q: APK installation failed?
- Check if you have Android 5.0+.
- Ensure "Install Unknown Apps" is enabled.
- Check if you have at least 100MB of free storage.

### Q: Permission Issues?
Vault requires storage permissions only for the Import/Export feature. It does not scan other files or photos.

---

## 📊 App Info

| Item | Details |
|------|------|
| **Version** | 1.0.0 |
| **Release Date** | 2026-05-04 |
| **Size** | ~45-50 MB |
| **Min Android** | 5.0 (API 21) |
| **Encryption** | AES-256-GCM |
| **License** | MIT |

---

## 🤝 Support & Feedback

- **Report Bugs**: Open a [GitHub Issue](https://github.com/ySyndevL/vault-app-dist/issues).
- **Suggestions**: Join the [GitHub Discussions](https://github.com/ySyndevL/vault-app-dist/discussions).

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 🔮 Roadmap

- [ ] 📱 iOS Support
- [ ] 🎐 Play Store / F-Droid distribution
- [ ] 👆 Biometric Unlock (Fingerprint/Face ID)
- [ ] 🔐 Password Strength Analyzer
- [ ] 🌙 Auto-lock timer

---

<div align="center">

**❤️ If Vault App helps you, please give it a ⭐ Star!Sure thing! Here is the English version of your **Vault App** GitHub README. I've polished the phrasing to sound professional and clear for an international audience.

---

# Vault App

[![Flutter](https://img.shields.io/badge/Flutter-3.41.4-blue)](https://flutter.dev)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Android-brightgreen)](https://www.android.com)
[![Release](https://img.shields.io/github/v/release/ySyndevL/vault-app-dist?label=Latest%20Release)](https://github.com/ySyndevL/vault-app-dist/releases)

「🔐 A secure local password manager for Android with AES-256 encryption, multi-language support & backup features」

A secure, lightweight local password manager for Android devices. All data is stored locally with no cloud synchronization.

<div align="center">
<img width="500" alt="Vault App UI" src="https://github.com/user-attachments/assets/3d914615-31b3-4621-a2bb-5afde23b18f0" />
</div>

---

## ✨ Core Features

### 🔐 Password Management
- **AES-256-GCM Encryption**: Military-grade protection for your data.
- **Argon2id Key Derivation**: Industry-standard strong key derivation.
- **Custom Fields**: Manage Website, Username, Password, and Notes.
- **Quick Search**: Real-time filtering for instant access.
- **One-Tap Copy**: Easily copy passwords to your clipboard.

### 📍 Address Management
- Securely store frequently used addresses.
- Categorization and tagging support.
- Fully encrypted storage.

### 💾 Backup & Restore
- 📦 **Export as `.vault`**: Encrypted binary format (Recommended).
- 📊 **Export as CSV**: Compatible with spreadsheet software like Excel.
- 📈 **Export as Excel**: Native `.xlsx` format support.
- 📥 **Universal Import**: Supports importing from all the above formats.

### 🌐 Multi-Language Support
- 🇬🇧 English
- 🇹🇼 Traditional Chinese (繁體中文)

### 🎨 Modern UI
- Material Design 3 implementation.
- Intuitive tabbed navigation.
- Dark Mode optimized.
- Fully responsive design.

---

## 📋 System Requirements

| Item | Requirement |
|------|------|
| **Android Version** | 5.0+ (API 21+) |
| **Storage** | ~50 MB |
| **RAM** | ≥ 2 GB (Recommended) |
| **Network** | Not Required (100% Offline) |

---

## 📥 Installation

### Method 1: Install APK directly (Recommended)

1. **Download** the APK file:
   - Get the latest `vault_app-releasev1.0.0.apk` from the [Releases](https://github.com/ySyndevL/vault-app-dist/releases) page.

2. **Allow Unknown Apps**:
   ```
   Settings → Apps → Special app access → Install unknown apps → Select File Manager → Allow
   ```

3. **Install**:
   - Open the downloaded APK and follow the prompts to "Install".

4. **Launch**:
   - Once installed, tap "Open" or find "Vault" in your app drawer.

### Method 2: ADB Installation (Developers)
```bash
# Ensure your Android device is connected
adb devices

# Install the APK
adb install vault_app-releasev1.0.0.apk

# Launch the app
adb shell am start -n com.ysyn_devl.vault_app/.MainActivity
```

### Method 3: Google Drive (Alternative)

If GitHub download speeds are slow, you can use this Google Drive link:
[vault_app v1.0.0 - Google Drive](https://drive.google.com/file/d/1UWhVrGc5Z4uxsqhZt9X84EpnOUHHgO48/view?usp=sharing)

---

## 🔒 Security Features

### Offline First
✅ **Local Storage Only**
- No Cloud Sync.
- No remote servers.
- No data transmission over the internet.
- Works 100% offline.

### Encryption Standards
- **AES-256-GCM**: NIST-standard authenticated encryption.
- **Argon2id**: Modern, password-cracking resistant hashing.
- **PBKDF2**: For legacy compatibility.

### Privacy Protection
✅ **No Tracking, No Ads, No Data Collection**
- Zero personal information gathered.
- No analytics or telemetry code.
- No data uploads.
- Open source (Plan in progress).

### Minimal Permissions
The app only requests the following:
- 📂 **Read/Write External Storage**: To save and load backup files.
- 🔌 **Network Access** (Optional): To check for app updates.

---

## 🚀 Quick Start

### 1. Initial Setup - Set Your Master Password

```
Launch App → "Create Vault" Page
↓
Enter Master Password (Min. 8 characters)
↓
Confirm Password
↓
Tap "Set Master Password"
↓
Access Main Dashboard
```

**Password Tips**:
- ✅ Use at least 12 characters.
- ✅ Include uppercase, lowercase, numbers, and symbols.
- ✅ Avoid personal info (names, birthdays).

### 2. Adding a Password
1. Go to the **Passwords** tab.
2. Tap the **+** button in the bottom right.
3. Fill in the details (Website, Username, Password, Notes).
4. Tap **Save**.

### 3. Managing Entries
- **Search**: Use the search bar at the top for real-time filtering.
- **Edit**: Tap any entry to modify and save.
- **Delete**: Long-press or swipe an entry to delete.
- **Copy**: Tap the icon next to the password field for instant clipboard copy.

### 4. Backing Up Data
**Backups are essential!** To create one:
1. Open the sidebar (☰ menu).
2. Tap **Backup**.
3. Choose your format:
   - **.vault**: Most secure, encrypted format.
   - **CSV/Excel**: For external viewing.
4. Save the file to a safe location (External drive, encrypted cloud, etc.).

---

## ⚙️ Settings & Customization

- **Change Master Password**: Sidebar → Settings → Change Master Password. (Requires current password).
- **Switch Language**: Sidebar → Settings → Language. Changes apply instantly.
- **Clear All Data**: ⚠️ **Warning**: This action is irreversible. Sidebar → Settings → Clear All Data.

---

## 🐛 Troubleshooting

### Q: I forgot my Master Password!
**A**: Unfortunately, there is no recovery option. For security reasons, the app does not support password resets. You must reinstall the app and start over.

### Q: APK installation failed?
- Check if you have Android 5.0+.
- Ensure "Install Unknown Apps" is enabled.
- Check if you have at least 100MB of free storage.

### Q: Permission Issues?
Vault requires storage permissions only for the Import/Export feature. It does not scan other files or photos.

---

## 📊 App Info

| Item | Details |
|------|------|
| **Version** | 1.0.0 |
| **Release Date** | 2026-05-04 |
| **Size** | ~45-50 MB |
| **Min Android** | 5.0 (API 21) |
| **Encryption** | AES-256-GCM |
| **License** | MIT |

---

## 🤝 Support & Feedback

- **Report Bugs**: Open a [GitHub Issue](https://github.com/ySyndevL/vault-app-dist/issues).
- **Suggestions**: Join the [GitHub Discussions](https://github.com/ySyndevL/vault-app-dist/discussions).

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 🔮 Roadmap

- [ ] 📱 iOS Support
- [ ] 🎐 Play Store / F-Droid distribution
- [ ] 👆 Biometric Unlock (Fingerprint/Face ID)
- [ ] 🔐 Password Strength Analyzer
- [ ] 🌙 Auto-lock timer

---

<div align="center">

**❤️ If Vault App helps you, please give it a ⭐ Star!**

🔐 Keep Your Passwords Safe, Keep Your Data Private.

</div>
```
