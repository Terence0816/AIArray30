# ⌨️ AI 行列30 for Windows

[![Downloads](https://img.shields.io/github/downloads/Terence0816/AIArray30/total?label=Downloads&color=success)](https://github.com/Terence0816/AIArray30/releases)
![Version](https://img.shields.io/github/v/release/Terence0816/AIArray30?label=Version&color=blue)
![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-0078D6?logo=windows&logoColor=white)
![Architecture](https://img.shields.io/badge/Architecture-x64-6f42c1)
![IME](https://img.shields.io/badge/Windows-TSF-0A84FF)

<p align="center">
  <img src="assets/AIArray30_Cover.png" alt="AI 行列30 for Windows" width="100%">
</p>

**保留熟悉的行列30輸入方式，加入 NexaCore 連續輸入、個人化學習與更現代的 Windows 輸入體驗。**

AI 行列30 for Windows 是一套以 **Windows TSF（Text Services Framework）** 為基礎的行列30輸入法。

除了傳統逐字輸入外，也加入 **NexaCore 連續輸入引擎**，可將連續輸入的行列碼組合成較合理的中文字句，並透過本機個人學習逐步適應使用者的輸入習慣。

> 本 Repository 目前僅提供程式介紹、畫面與正式安裝版下載，**不公開原始碼**。

---

## 🎬 操作示範

YouTube：

👉 **[AI 行列30 Windows 版｜連續輸入實測與操作示範](https://youtu.be/0_sohVOYjJQ)**

---

## 🖼️ 介面預覽

### 一般設定

可設定 Shift／Ctrl + Space 中英文切換、NexaCore 連續輸入、多組連續候選、背景詞組學習、候選視窗字型與碼字對應色彩提示。

![AI 行列30 一般設定](assets/screenshots/general-settings.png)

### NexaCore 連續輸入

輸入一整串行列碼後，由 NexaCore 依照合法候選與中文上下文進行組句與排序；可選擇只顯示最優候選，或最多顯示 3 組自動候選。

上方行列碼可依第一候選句的實際切碼結果顯示對應色彩，方便辨識每一段碼所對應的中文字。

![AI 行列30 NexaCore 連續輸入](assets/screenshots/continuous-input.png)

### 連續輸入詞彙共用學習中心

共用學習為選用功能，預設關閉。開啟後，可將必要的新增、修改與刪除／拒絕候選事件匿名送入共用學習流程，協助改善正式共用資料庫。

一般打字內容與本機背景詞組學習不會因為這個功能而全部上傳。

![AI 行列30 共用學習中心](assets/screenshots/shared-learning-center.png)

---

## ✨ 主要功能

- Windows 原生 **TSF 輸入法**
- 支援標準行列30輸入
- **NexaCore 連續輸入**
- 自動候選可選擇 **Top1 / Top3** 顯示
- 自動產生的連續候選最多保留 3 組，降低雜訊與長期負擔
- 手動新增／修改的個人候選不受 Top3 限制
- 一般逐字輸入也可進行 **背景詞組學習**
- 背景學習會記錄常用的 2～10 字詞組，協助之後的連續輸入排序
- 個人本機學習優先於正式共用資料庫與核心預設排序
- 候選可自行新增、編輯與刪除
- 支援第一候選的 **碼字對應色彩提示**
- 支援單按 Shift 切換中／英文
- 支援按住 Shift 暫時輸入英文／符號，放開後自動回到原中文模式
- 支援 `Ctrl + Space` 切換中／英文
- 可在游標附近顯示「中／英」狀態提示
- 支援 Windows 11「進階鍵盤設定 → 覆寫預設輸入法」
- 可選擇參與匿名共用學習
- 正式共用資料庫可獨立更新，不影響個人本機學習
- 單一 Setup EXE 安裝／更新／移除

---

## 🧠 NexaCore 連續輸入

傳統行列30通常以逐字輸入為主。

AI 行列30加入 NexaCore 後，可以將一段連續輸入的行列碼先建立合法候選，再依中文上下文進行組句與排序。

例如同一串碼可能同時存在多種合法組合，NexaCore 會依照：

- 行列碼合法性
- 字詞搭配
- 中文上下文
- 個人本機學習
- 背景詞組習慣
- 正式共用資料庫

綜合決定較適合的候選順序。

### Top1 / Top3

設定中可選擇是否顯示多組連續候選：

- **關閉**：只顯示最優 1 組
- **開啟**：最多顯示 3 組自動候選

如果某組候選被使用者刪除，不會再拿原本第 4 名自動補回來。

使用者自己手動新增的候選，則不受自動 Top3 限制。

---

## 📚 背景詞組學習

除了明確新增或修改候選外，AI 行列30也可以從一般逐字輸入中學習常用詞組。

例如平常逐字輸入：

```text
我要回家喝咖啡
```

系統可以在本機逐步記住常用的 2～10 字組合，例如：

```text
我要
我要回家
回家喝咖啡
我要回家喝咖啡
```

之後使用連續輸入時，即使核心原本沒有把某個組合排在前面，也可以因為你的實際使用習慣提高順位。

背景詞組學習為 **本機個人資料**，不會直接當成共用資料上傳。

---

## 🎨 碼字對應色彩提示

連續輸入候選視窗可以依照第一候選句的實際切碼方式，將：

- 上方行列碼
- 第一候選句中的中文字

以相同顏色分組顯示。

如果一個字由多個行列碼組成，整組碼會使用相同顏色，讓使用者更容易看出：

```text
哪一段碼 → 對應哪一個字
```

此功能可於設定中開啟或關閉。

---

## ⌨️ 中英文切換

### 單按 Shift

可設定：

- 所有 Shift
- 左 Shift
- 右 Shift

單獨按一下 Shift 再放開，即可切換中文／英文輸入模式。

### 按住 Shift 暫時輸入英文

在中文模式中，可以：

```text
按住 Shift → 輸入 ABC / 數字符號 → 放開 Shift → 繼續中文輸入
```

只要 Shift 期間有搭配其他按鍵，就不會被判定成「切換中英文模式」。

### Ctrl + Space

仍支援傳統 `Ctrl + Space` 切換中／英文。

---

## ☁️ 匿名共用學習

AI 行列30提供選用的「連續輸入詞彙共用學習中心」。

此功能預設關閉。

啟用後，只有與候選改善有關的必要事件才會進入共用學習流程，例如：

- 新增候選
- 修改候選
- 刪除／拒絕不適合的候選

一般正常選字不會因為共用學習而全部送出；本機背景詞組與個人習慣仍保存在本機。

正式共用資料庫與個人學習互相獨立，個人本機學習具有較高優先權。

---

## 📦 下載

### 最新版本

👉 **[下載最新版本 / Latest Release](https://github.com/Terence0816/AIArray30/releases/latest)**

👉 **[查看所有 Releases / 發行版本](https://github.com/Terence0816/AIArray30/releases)**

正式版本僅提供 Windows 安裝程式，不提供原始碼。

Release 安裝檔名稱會類似：

```text
AIArray30_Setup_vX.X.X.exe
```

---

## 🚀 安裝、更新與移除

下載最新版 Setup 後直接執行即可。

### 第一次執行

若電腦尚未安裝 AI 行列30，Setup 會詢問是否安裝目前版本。

### 已安裝舊版本

若偵測到較舊版本，Setup 會提示更新。

### 已安裝相同版本

再次執行同版本 Setup 時，可選擇移除 AI 行列30。

### 已安裝較新版本

較舊的 Setup 不會直接覆蓋較新的已安裝版本。

安裝完成後，可在 Windows 的輸入法清單中選擇：

```text
繁體中文（台灣）－ AI 行列30
```

---

## 🔐 數位簽章與安全性

正式 Release 的安裝程式可使用 Windows Authenticode 數位簽章。

NexaCore 核心模型會以加密封裝方式隨安裝程式提供，執行時由輸入法在本機載入。

建議只從本專案的 GitHub Releases 頁面下載正式版本。

---

## 💻 系統需求

| 項目 | 需求 |
| --- | --- |
| 作業系統 | Windows 10 / Windows 11 |
| 架構 | 64-bit x64 |
| 輸入法架構 | Windows TSF |
| 安裝方式 | 單一 Setup EXE |
| 網路 | 一般輸入不需要；共用資料庫／共用學習功能需要 |
| 權限 | 安裝時依 Windows 提示取得必要權限 |

---

## 📁 Repository 說明

此 GitHub Repository 主要提供：

```text
README.md
assets/
├─ AIArray30_Cover.png
└─ screenshots/
   ├─ general-settings.png
   ├─ continuous-input.png
   └─ shared-learning-center.png
```

正式安裝程式統一透過 **GitHub Releases** 發布。

**本 Repository 不公開 AI 行列30原始碼。**

---

## 🔎 搜尋關鍵字

`AIArray30`, `Array30`, `行列30`, `行列輸入法`, `中文輸入法`, `Windows輸入法`, `TSF`, `NexaCore`, `連續輸入`, `AI輸入法`, `智慧輸入`, `中文打字`, `Traditional Chinese IME`, `Windows IME`, `Array input method`

---

## ⚠️ 使用說明

AI 行列30目前仍持續測試與改善 NexaCore 連續輸入、個人學習、候選排序及共用資料庫內容。

不同使用者的輸入習慣不同，連續輸入候選不一定每次都與使用者預期完全相同；可透過個人學習、新增／修改／刪除候選持續調整。

---

## 👤 Author

**Terence0816**

---

## English

**AI Array30 for Windows** is a native Windows TSF Traditional Chinese input method based on the Array30 input method.

It adds **NexaCore continuous input**, local personalization, background phrase learning, Top1/Top3 candidate display, candidate editing, Shift/Ctrl+Space language switching, and optional anonymous shared learning.

### Highlights

- Native Windows TSF IME
- Array30 input method
- NexaCore continuous Chinese input
- Top1 / Top3 candidate display
- Local personalized learning
- Background 2–10 character phrase learning
- Candidate add / edit / delete
- Color-coded code-to-character hints
- Single Shift language switching
- Hold Shift for temporary English input
- Ctrl + Space support
- Optional anonymous shared learning
- Single Setup EXE installer

### Download

👉 **[Latest Release](https://github.com/Terence0816/AIArray30/releases/latest)**

This repository provides documentation, screenshots and official release installers only. **Source code is not published.**
