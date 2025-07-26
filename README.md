# 发票计数应用 (Invoice Counter App)

一个轻量级的发票管理和计数工具，支持跨不同系统进行发票统计和管理。这是一个使用现代技术栈构建的演示项目。

## 📋 功能特性

- **智能发票扫描**: 使用AI技术自动识别和提取发票信息
- **发票管理**: 创建、编辑、删除和查看发票记录
- **计数统计**: 实时统计发票数量和金额
- **历史记录**: 查看发票操作历史
- **数据可视化**: 提供统计图表和数据分析
- **设置管理**: 自定义应用配置和偏好设置

## 🛠️ 技术栈

- **前端框架**: React Native with Expo
- **状态管理**: Zustand
- **类型检查**: TypeScript
- **UI组件**: React Native组件库
- **AI集成**: 智能发票识别API
- **对象检测**: 计算机视觉技术
- **代码格式化**: Prettier

## 📁 项目结构

```
project/
├── app/                    # 应用主目录
│   ├── (tabs)/            # 标签页路由
│   │   ├── counter/       # 计数功能
│   │   ├── create.tsx     # 创建发票
│   │   ├── index.tsx      # 主页
│   │   └── settings.tsx   # 设置页面
│   ├── _layout.tsx        # 主布局
│   └── +not-found.tsx     # 404页面
├── components/            # 可复用组件
│   ├── AIInvoiceScanner.tsx
│   ├── InvoiceForm.tsx
│   ├── ObjectMarker.tsx
│   └── SettingsModal.tsx
├── store/                 # 状态管理
│   ├── countStore.ts
│   └── invoiceStore.ts
├── types/                 # TypeScript类型定义
│   ├── counting.ts
│   └── invoice.ts
├── utils/                 # 工具函数
│   ├── ai.ts
│   └── objectDetection.ts
├── hooks/                 # 自定义Hooks
│   └── useFrameworkReady.ts
└── config/               # 配置文件
    └── config.json
```

## 🚀 快速开始

### 环境要求

- Node.js (版本 16 或更高)
- npm 或 yarn
- Expo CLI
- iOS Simulator (可选) 或 Android Emulator (可选)

### 安装步骤

1. **克隆仓库**
   ```bash
   git clone https://github.com/fengguihao890/invoice-count-.git
   cd invoice-count-
   ```

2. **安装依赖**
   ```bash
   npm install
   # 或
   yarn install
   ```

3. **启动开发服务器**
   ```bash
   npx expo start
   ```

4. **运行应用**
   - 在iOS模拟器上运行: 按 `i`
   - 在Android模拟器上运行: 按 `a`
   - 在真机上运行: 扫描二维码

## 📱 使用指南

### 主要功能

1. **发票扫描**
   - 点击相机按钮拍摄发票
   - AI自动识别发票信息
   - 手动编辑和确认信息

2. **发票管理**
   - 查看所有发票列表
   - 搜索和筛选发票
   - 编辑发票详情

3. **统计功能**
   - 查看发票总数和总金额
   - 按时间范围统计
   - 数据可视化图表

4. **设置**
   - 配置应用偏好
   - 管理用户设置
   - 数据备份和恢复

## 🔧 配置

### 环境变量

在项目根目录创建 `.env` 文件：

```env
# AI服务配置
AI_API_KEY=your_ai_api_key
AI_ENDPOINT=https://api.example.com/ai

# 应用配置
APP_NAME=发票计数应用
APP_VERSION=1.0.0
```

### 配置文件

编辑 `config/config.json` 来自定义应用设置：

```json
{
  "app": {
    "name": "发票计数应用",
    "version": "1.0.0"
  },
  "features": {
    "aiScanning": true,
    "objectDetection": true,
    "dataExport": true
  }
}
```

## 🧪 开发

### 代码规范

项目使用 Prettier 进行代码格式化：

```bash
# 格式化代码
npm run format

# 检查代码格式
npm run lint
```

### 构建

```bash
# 构建Android APK
npx expo build:android

# 构建iOS应用
npx expo build:ios
```

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

1. Fork 项目
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开 Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 🙏 致谢

- [Expo](https://expo.dev/) - React Native开发平台
- [Zustand](https://github.com/pmndrs/zustand) - 状态管理库
- [React Native](https://reactnative.dev/) - 移动应用开发框架

## 📞 联系方式

- 项目链接: [https://github.com/fengguihao890/invoice-count-](https://github.com/fengguihao890/invoice-count-)
- 问题反馈: [Issues](https://github.com/fengguihao890/invoice-count-/issues)

---

⭐ 如果这个项目对您有帮助，请给我们一个星标！ 