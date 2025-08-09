# 發票計數應用程式 (Invoice Counter App)

一個輕量級的發票管理和計數工具，支援跨不同系統進行發票統計和管理。這是一個使用現代技術堆疊建構的演示專案。

## 📋 功能特性

- **智慧發票掃描**: 使用AI技術自動識別和提取發票信息
- **發票管理**: 建立、編輯、刪除和檢視發票記錄
- **計數統計**: 即時統計發票數量和金額
- **歷史記錄**: 查看發票操作歷史
- **資料視覺化**: 提供統計圖表和資料分析
- **設定管理**: 自訂應用程式配置和偏好設定

## 🛠️ 技術堆疊

- **前端框架**: React Native with Expo
- **狀態管理**: Zustand
- **類型檢查**: TypeScript
- **UI元件**: React Native元件庫
- **AI整合**: 智慧發票識別API
- **物件偵測**: 電腦視覺技術
- **代碼格式化**: Prettier

## 📁 專案結構

```
project/
├── app/ # 應用主目錄
│ ├── (tabs)/ # 標籤頁路由
│ │ ├── counter/ # 計數功能
│ │ ├── create.tsx # 建立發票
│ │ ├── index.tsx # 首頁
│ │ └── settings.tsx # 設定頁面
│ ├── _layout.tsx # 主佈局
│ └── +not-found.tsx # 404頁面
├── components/ # 可重複使用組件
│ ├── AIInvoiceScanner.tsx
│ ├── InvoiceForm.tsx
│ ├── ObjectMarker.tsx
│ └── SettingsModal.tsx
├── store/ # 狀態管理
│ ├── countStore.ts
│ └── invoiceStore.ts
├── types/ # TypeScript類型定義
│ ├── counting.ts
│ └── invoice.ts
├── utils/ # 工具函數
│ ├── ai.ts
│ └── objectDetection.ts
├── hooks/ # 自訂Hooks
│ └── useFrameworkReady.ts
└── config/ # 設定文件
 └── config.json
```

## 🚀 快速開始

### 環境需求

- Node.js (版本 16 或更高)
- npm 或 yarn
- Expo CLI
- iOS Simulator (可選) 或 Android Emulator (可選)

### 安裝步驟

1. **克隆倉庫**
 『`bash
 git clone https://github.com/fengguihao890/invoice-count-.git
 cd invoice-count-
 ```

2. **安裝依賴**
 『`bash
 npm install
 # 或
 yarn install
 ```

3. **啟動開發伺服器**
 『`bash
 npx expo start
 ```

4. **運行應用程式**
 - 在iOS模擬器上運行: 按 `i`
 - 在Android模擬器上運行: 按 `a`
 - 在真機上運作: 掃描二維碼

## 📱 使用指南

### 主要功能

1. **發票掃描**
 - 點擊相機按鈕拍攝發票
 - AI自動識別發票訊息
 - 手動編輯和確認訊息

2. **發票管理**
 - 查看所有發票列表
 - 搜尋和篩選發票
 - 編輯發票詳情

3. **統計功能**
 - 查看發票總數和總金額
 - 按時間範圍統計
 - 數據視覺化圖表

4. **設定**
 - 配置應用偏好
 - 管理用戶設定
 - 資料備份與復原

## 🔧 配置

### 環境變數

在專案根目錄建立 `.env` 檔案：

```env
# AI服務配置
AI_API_KEY=your_ai_api_key
AI_ENDPOINT=https://api.example.com/ai

# 應用程式配置
APP_NAME=發票計數應用
APP_VERSION=1.0.0
```

### 設定文件

編輯 `config/config.json` 來自訂應用程式設定：

```json
{
 "app": {
 "name": "發票計數應用程式",
 "version": "1.0.0"
 },
 "features": {
 "aiScanning": true,
 "objectDetection": true,
 "dataExport": true
 }
}
```

## 🧪 開發

### 程式碼規範

專案使用 Prettier 進行程式碼格式化：

『`bash
# 格式化程式碼
npm run format

# 檢查程式碼格式
npm run lint
```

### 構建

『`bash
# 建構Android APK
npx expo build:android

# 建構iOS應用
npx expo build:ios
```

## 🤝 貢獻

歡迎投稿 Issue 和 Pull Request！

1. Fork 項目
2. 建立功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 開啟 Pull Request

## 📄 許可證

本專案採用 MIT 授權 - 查看 [LICENSE](LICENSE) 文件以了解詳情。

## 🙏 致謝

- [Expo](https://expo.dev/) - React Native開發平台
- [Zustand](https://github.com/pmndrs/zustand) - 狀態管理函式庫
- [React Native](https://reactnative.dev/) - 行動應用開發框架

## 📞 聯絡方式

- 專案連結: [https://github.com/fengguihao890/invoice-count-](https://github.com/fengguihao890/invoice-count-)
- 問題回饋: [Issues](https://github.com/fengguihao890/invoice-count-/issues)

---

⭐ 如果這個項目對您有幫助，請給我們一個星標！
