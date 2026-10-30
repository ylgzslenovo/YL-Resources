# 影联NFC快捷服务 / Yinglian NFC Quick Service

---

## 中文

### 📖 简介

**影联NFC快捷服务** 是一款基于 NFC 标签的安卓应用快速启动工具。通过将应用包名写入 NFC 标签，碰卡即可快速打开指定应用，无需在桌面翻找。

### ✨ 功能特性

- **应用列表选择**：自动获取手机所有已安装应用，手动选择要启动的目标
- **AAR 写入**：使用 Android Application Record 标准写入 NFC 标签
- **系统应用适配**：内置小米、华为、vivo、OPPO、三星等品牌系统应用的组件名映射
- **加密卡检测**：自动识别加密卡/非 NDEF 格式卡，提示无法写入
- **线程安全**：写入操作在子线程执行，避免主线程阻塞
- **自定义弹窗**：应用选择、写入等待均为自定义 UI
- **代码混淆**：已配置 ProGuard 规则

### 📱 使用方式

1. 打开应用，点击「选择」选择要启动的目标应用
2. 点击「📝 写入NFC标签」
3. 将空白 NFC 卡贴近手机背面
4. 写入成功后，碰卡即可打开该应用

### 🔧 技术栈

- 语言：Java
- 最低 SDK：Android 5.0 (API 21)
- 目标 SDK：Android 12 (API 31)
- 无 AndroidX 依赖
- NFC 写入基于 `NdefRecord.createApplicationRecord()`

### 📦 版本信息

| 项目 | 内容 |
|------|------|
| 应用名 | 影联NFC快捷服务 |
| 包名 | `com.ylstudio.nfcfast` |
| 版本 | `1.0.2_00014_2026.09.05_Beta` |
| 开发商 | 影联工作室 |
| 解压密码 | `ylgzs` |

### ⚠️ 注意事项

- 系统级组件（如 TEE 安全服务）可能无界面，碰卡后闪退或跳转应用商店属正常现象
- 加密卡（Mifare Classic 等）不支持 NDEF 格式，无法写入
- 写入时请保持 NFC 卡贴近手机，避免中途移动

### 🔗 反馈

Bug 反馈请前往：https://ylgzs.top

---

## English

### 📖 Introduction

**Yinglian NFC Quick Service** is an Android app launcher based on NFC tags. By writing an app package name to an NFC tag, you can launch the target app instantly by tapping the tag — no need to search through your home screen.

### ✨ Features

- **App List Selection**: Automatically retrieves all installed apps for manual selection
- **AAR Writing**: Writes NFC tags using the standard Android Application Record
- **System App Support**: Built-in component name mappings for Xiaomi, Huawei, vivo, OPPO, and Samsung system apps
- **Encrypted Card Detection**: Detects encrypted/non-NDEF cards and prevents writing
- **Thread Safety**: Write operations run on a background thread to avoid blocking the main thread
- **Custom Dialogs**: Custom UI for app selection and write waiting
- **ProGuard Enabled**: Code obfuscation configured

### 📱 Usage

1. Open the app and tap "Select" to choose the target app
2. Tap "📝 Write NFC Tag"
3. Hold a blank NFC tag against the back of your phone
4. Once written, tap the tag to launch the app

### 🔧 Tech Stack

- Language: Java
- Min SDK: Android 5.0 (API 21)
- Target SDK: Android 12 (API 31)
- No AndroidX dependency
- NFC writing based on `NdefRecord.createApplicationRecord()`

### 📦 Version Info

| Item | Content |
|------|---------|
| App Name | Yinglian NFC Quick Service |
| Package | `com.ylstudio.nfcfast` |
| Version | `1.0.2_00014_2026.09.05_Beta` |
| Developer | Yinglian Studio |
| Extraction Password | `ylgzs` |

### ⚠️ Notes

- System-level components (e.g., TEE security services) may have no UI; crashing or redirecting to the app store after tapping the tag is expected behavior
- Encrypted cards (e.g., Mifare Classic) do not support NDEF format and cannot be written
- Keep the NFC tag close to your phone during writing to avoid interruption

### 🔗 Feedback

Bug reports: https://ylgzs.top
