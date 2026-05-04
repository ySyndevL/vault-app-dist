# Vault App

[![Flutter](https://img.shields.io/badge/Flutter-3.41.4-blue)](https://flutter.dev)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Android-brightgreen)](https://www.android.com)
[![Release](https://img.shields.io/github/v/release/ySyndevL/vault-app-dist?label=Latest%20Release)](https://github.com/ySyndevL/vault-app-dist/releases)

A simple offline password manager

一個安全、輕量級的本地密碼管理器，支持 Android 設備。所有資料本地儲存，無雲同步。

<div align="center">
<img width="500" alt="image" src="https://github.com/user-attachments/assets/3d914615-31b3-4621-a2bb-5afde23b18f0" />
</div>

---

## ✨ 核心功能

### 🔐 密碼管理
- **AES-256-GCM 加密**：軍事級加密保護
- **Argon2id 密鑰導出**：強力的密鑰衍生
- **自訂欄位**：網站、用戶名、密碼、備註
- **快速搜尋**：即時篩選功能
- **複製到剪貼板**：一鍵複製密碼

### 📍 位址管理
- 保存常用位址
- 位址分類和標籤
- 加密存儲

### 💾 備份 & 還原
- 📦 匯出為 `.vault`（加密格式，推薦）
- 📊 匯出為 CSV（可在 Excel 中開啟）
- 📈 匯出為 Excel（.xlsx 格式）
- 📥 支援匯入上述所有格式

### 🌐 多語言支持
- 🇬🇧 English
- 🇹🇼 繁體中文

### 🎨 現代化 UI
- Material Design 3
- 直觀的標籤頁面
- 深色模式友好
- 響應式設計

---

## 📋 系統需求

| 項目 | 要求 |
|------|------|
| **Android 版本** | 5.0+ (API 21+) |
| **儲存空間** | ~50 MB |
| **記憶體** | ≥ 2 GB（推薦） |
| **網路** | 不需要（完全離線） |

---

## 📥 安裝方式

### 方式 1：直接安裝 APK（推薦）

1. **下載** APK 檔案
   - 從 [Releases](https://github.com/ySyndevL/vault-app-dist/releases) 頁面下載 `vault_app-releasev1.0.0.apk`

2. **允許安裝未知應用**
   ```
   設定 → 應用 → 特殊應用存取權限 → 安裝未知應用 → 選擇檔案管理器 → 允許
   ```

3. **安裝應用**
   - 開啟下載的 APK 檔案
   - 按照提示點擊「安裝」

4. **啟動應用**
   - 安裝完成後點擊「開啟」
   - 或從應用列表中找到 "Vault" 並點擊

### 方式 2：ADB 安裝（開發者）

```bash
# 確保已連接 Android 設備
adb devices

# 安裝 APK
adb install vault_app-releasev1.0.0.apk

# 啟動應用
adb shell am start -n com.ysyn_devl.vault_app/.MainActivity
```

### 方式 3：Google Drive 下載（備用）

如果 GitHub 下載較慢，可使用 Google Drive 連結：
[vault_app v1.0.0 - Google Drive](https://drive.google.com/file/d/1UWhVrGc5Z4uxsqhZ9X84EpnOUHHgQ48/view)

---

## 🔒 安全特性

### 本地優先
✅ **所有資料儲存在設備本地**
- 無雲同步
- 無遠程服務器
- 無網路傳輸
- 完全離線工作

### 加密標準
- **AES-256-GCM**：NIST 標準加密算法
- **Argon2id**：現代密碼雜湊算法
- **PBKDF2**：備用相容性算法

### 隱私保護
✅ **無追蹤、無廣告、無數據收集**
- 不收集個人信息
- 不包含分析代碼
- 不上傳任何數據
- 開源代碼（計劃中）

### 權限最小化
應用僅要求以下權限：
- 📂 **讀取/寫入外部儲存**：用於備份檔案
- 🔌 **網路存取**（可選）：檢查應用更新

---

## 🚀 快速開始

### 1️⃣ 首次啟動 - 建立主密碼

```
應用開啟 → 看到「建立保險箱」頁面
↓
輸入主密碼（至少 8 字元）
↓
再次確認密碼
↓
點擊「設定主密碼」按鈕
↓
進入應用主頁面
```

**密碼建議**：
- ✅ 至少 12 字元
- ✅ 包含大小寫字母、數字、符號
- ✅ 不使用個人信息（名字、生日等）

### 2️⃣ 新增密碼

1. 進入「密碼」標籤
2. 點擊右下角 **+** 按鈕
3. 填寫以下資訊：
   - **網站**：如 `example.com` 或 `GitHub`
   - **用戶名**：登入名或郵箱
   - **密碼**：複雜的強密碼
   - **備註**：安全問題、恢復郵箱等（可選）
4. 點擊「儲存」

### 3️⃣ 管理密碼

**搜尋密碼**：
- 在列表頂部搜尋框輸入網站名稱或用戶名
- 即時篩選結果

**編輯密碼**：
- 點擊任何密碼條目 → 修改資訊 → 儲存

**刪除密碼**：
- 長按條目或滑動 → 刪除確認

**複製密碼**：
- 點擊密碼欄右側的圖標自動複製到剪貼板

### 4️⃣ 備份重要資料

**定期備份**很重要！步驟：

1. 開啟側邊欄（點擊左上角☰）
2. 點擊「備份」選項
3. 選擇匯出格式：
   - 📦 `.vault`（推薦）：加密格式，安全性最高
   - 📊 `CSV`：可用 Excel 開啟
   - 📈 `Excel`：.xlsx 格式

4. 將備份檔案保存到安全位置：
   - 外接硬碟
   - 雲端儲存（已加密的檔案）
   - 另一台設備

### 5️⃣ 還原備份

1. 開啟側邊欄
2. 點擊「還原」選項
3. 選擇要匯入的檔案（`.vault`、`.csv`、`.xlsx`）
4. 確認匯入
5. 應用會自動添加新的密碼條目

---

## ⚙️ 設定和自訂

### 更改主密碼

1. 側邊欄 → 設定
2. 點擊「更改主密碼」
3. 輸入舊密碼驗證
4. 設置新密碼
5. 確認

### 切換語言

1. 側邊欄 → 設定
2. 選擇「語言」
3. 選擇英文或繁體中文
4. 應用立即生效（無需重啟）

### 清除所有資料

⚠️ **警告**：此操作無法撤銷！

1. 側邊欄 → 設定
2. 點擊「清除所有資料」
3. 雙次確認
4. 應用重啟，回到首次啟動狀態

---

## 🐛 故障排除

### Q: 忘記了主密碼怎麼辦？

**A**: 很遺憾，沒有恢復選項。為了安全性，應用不支持密碼重置。

**解決方案**：
1. 卸載應用（設定 → 應用 → Vault → 卸載）
2. 重新安裝應用
3. 重新建立主密碼

**預防**：
- 定期備份資料
- 使用易記但強力的密碼

---

### Q: 無法安裝 APK？

**A**: 嘗試以下步驟：

1. **檢查 Android 版本**
   ```
   設定 → 關於手機 → Android 版本
   ```
   需要 5.0 或更高版本

2. **允許安裝未知應用**
   ```
   設定 → 應用 → 特殊應用存取權限 → 安裝未知應用 → 檔案管理器 → 允許
   ```

3. **清除快取並重試**
   ```
   設定 → 應用 → 檔案管理器 → 儲存 → 清除快取
   ```

4. **檢查儲存空間**
   - 至少預留 100 MB 空間

---

### Q: 無法匯入備份檔案？

**A**: 檢查以下項目：

- ✅ 檔案格式正確（`.vault`、`.csv` 或 `.xlsx`）
- ✅ 檔案完整未損壞
- ✅ 檔案存儲在可訪問的位置
- ✅ 嘗試用新生成的測試檔案

**如還有問題**：
- 清除應用資料（設定 → 應用 → Vault → 儲存 → 清除資料）
- 重新安裝應用
- 在 [Issues](https://github.com/ySyndevL/vault-app-dist/issues) 報告

---

### Q: 應用閃退或無法啟動？

**A**: 嘗試以下步驟：

1. **清除應用資料**
   ```
   設定 → 應用 → Vault → 儲存 → 清除資料
   ```

2. **清除應用快取**
   ```
   設定 → 應用 → Vault → 儲存 → 清除快取
   ```

3. **重新啟動設備**

4. **卸載並重新安裝**
   - 先備份資料！
   - 卸載應用
   - 重新安裝最新版本

---

### Q: 為什麼需要外部儲存權限？

**A**: 僅用於以下目的：
- 🔄 匯出備份檔案
- 📥 匯入備份檔案
- 📂 訪問下載資料夾

**隱私保證**：
- 不會掃描或訪問其他檔案
- 不會上傳任何資料

---

## 📊 應用信息

| 項目 | 詳情 |
|------|------|
| **版本** | 1.0.0 |
| **發布日期** | 2026-05-04 |
| **大小** | ~45-50 MB |
| **最低 Android** | 5.0 (API 21) |
| **推薦 Android** | 10+ |
| **語言** | English, 繁體中文 |
| **加密方式** | AES-256-GCM |
| **許可證** | MIT |

---

## 🤝 報告問題和建議

### 報告 Bug

發現問題？請在 [GitHub Issues](https://github.com/ySyndevL/vault-app-dist/issues) 中報告。

**包括以下信息**：
- 設備型號和 Android 版本
- 應用版本號
- 詳細的錯誤描述
- 重現步驟
- 截圖或日誌（如有）

### 功能建議

有新想法？在 [GitHub Discussions](https://github.com/ySyndevL/vault-app-dist/discussions) 中分享。

---

## 📄 許可證

本項目採用 **MIT 許可證**。詳見 [LICENSE](LICENSE) 檔案。

---

## 🙏 致謝

感謝以下開源項目和社區：

- [Flutter](https://flutter.dev) - 跨平台開發框架
- [Riverpod](https://riverpod.dev) - 狀態管理
- [intl](https://pub.dev/packages/intl) - 國際化支持
- [Pointycastle](https://pub.dev/packages/pointycastle) - 加密算法
- Android 開發社區

---

## 🔮 未來計劃

- [ ] 📱 iOS 版本支持
- [ ] 🎐 Google Play Store 上架或其他平台
- [ ] 👆 生物識別解鎖（指紋/面孔）
- [ ] 🔐 密碼強度分析工具
- [ ] 🌙 自動鎖定功能

---

## 📧 聯繫方式

- **GitHub**：[@ySyndevL](https://github.com/ySyndevL)
- **倉庫**：[vault-app-dist](https://github.com/ySyndevL/vault-app-dist)
- **報告問題**：[Issues](https://github.com/ySyndevL/vault-app-dist/issues)

---

## ⚖️ 免責聲明

本應用以「按原樣」提供，不附帶任何擔保。

- 應用開發者對因使用本應用而導致的任何直接或間接損害不承擔責任
- 定期備份你的重要資料
- 不要忘記你的主密碼
- 遵守當地法律法規使用本應用

---

<div align="center">

**❤️ 如果 Vault App 對你有幫助，請給個 ⭐ Star！**

🔐 Keep Your Passwords Safe, Keep Your Data Private.

</div>


