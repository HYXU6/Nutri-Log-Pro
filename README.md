# Nutri-Log Pro 🍎

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform: iOS](https://img.shields.io/badge/Platform-iOS-blue.svg)](https://www.apple.com/ios/)

[English](#english) | [中文说明](#chinese-description)
---
<a name="english"></a>
## English

**Nutri-Log Pro** is an intelligent dietary tracking tool based on iOS Shortcuts and the Google Gemini 3 Flash multimodal model. It analyzes food photos to calculate nutritional components and automatically synchronizes data to Apple Health and Apple Notes.

### ✨ Key Features

* **📸 Multi-channel Input**: Launch directly from the home screen (Camera) or via the "Share Sheet" in the Photos app.
* **🧠 Deep Nutritional Analysis**: Leverages Gemini 3 Flash to estimate Calories, Protein, Carbs, Fat (including Saturated Fat), Fiber, Sodium, and Sugar.
* **🏥 Health Integration**: Automatically writes recognition results into the Apple Health database.
* **📅 Visual Food Diary**: Appends a detailed log (text + original image) to a designated Apple Note for easy review.
* **🛡️ Robust Engineering**: Includes VPN connectivity pre-checks and image compression to prevent TLS handshake errors.

### 🚀 Quick Start

1. **Prerequisites**: An iPhone with the "Shortcuts" app and a **Google Gemini API Key**.
2. **Install**: Import the `.shortcut` file provided in this repo.
3. **Configure**: Enter your API Key in the "Get Contents of URL" action.
4. **Permissions**: Grant access to Camera, Photos, Health, and Notes upon first run.

### 🛡️ Disclaimer & Network Configuration 

**Network Environment & Tooling Disclaimer:**

* **Decoupled Logic**: This shortcut provides a framework for nutritional analysis. The integrated "Network Automation" steps (such as routing mode switches) are **optional implementation suggestions**. The core functionality of this project is independent of any specific third-party network tool.
* **No Bundled Tools**: This project **does not** provide, bundle, or promote any specific VPN, proxy, or circumvention applications. Any third-party app actions shown in the documentation are for demonstration of automation logic only.
* **User Responsibility**: Users are solely responsible for ensuring that their network environment and any third-party tools used comply with their local laws and regulations. The author assumes no liability for any misuse or legal consequences arising from the user's network configuration.

---
<a name="chinese-description"></a>
## 中文说明

**Nutri-Log Pro** 是一款基于 iOS 快捷指令和 Google Gemini 3 Flash 多模态大模型的智能饮食追踪工具。它能通过分析食物照片计算营养成分，并自动将数据同步至苹果“健康”与“备忘录”。

### ✨ 核心特性

* **📸 多渠道输入**：支持桌面图标直接启动（拍照）或在相册通过“共享表单”一键分享识别。
* **🧠 深度营养分析**：利用 Gemini 3 Flash 模型，精准估算热量、蛋白质、碳水、总脂肪（含饱和脂肪）、纤维素、钠及糖分。
* **🏥 健康闭环**：识别结果自动写入系统级 Apple Health 数据库，无需手动录入。
* **📅 图文饮食日志**：自动在苹果备忘录中追加详细记录（文字 + 原始图片），方便回溯。
* **🛡️ 健壮性设计**：内置 VPN 连通性预检逻辑，支持图像压缩传输，有效规避大图上传导致的 TLS 连接错误。

### 🛠️ 技术架构 (Technical Architecture)

本项目采用了典型的**端云协同**架构：

1. **Frontend (iOS Shortcuts)**: 负责图像采集、Base64 编码、JSON 构建及系统级 API 调用。
2. **Backend (Google Gemini API)**: 负责多模态视觉识别，通过结构化 Prompt 实现精准 JSON 数据输出。
3. **Regex Engine**: 使用正则表达式捕获组从 API 响应中提取核心营养数据。

### 🚀 快速开始

1. **环境要求**：安装了“快捷指令”的 iPhone，以及一个 **Google Gemini API Key**。
2. **安装步骤**：将本仓库提供的 `.shortcut` 文件导入手机。
3. **配置 Key**：在快捷指令的“获取 URL 内容”动作中填入你的 API Key。
4. **授权运行**：首次运行请允许访问相机、照片、健康与备忘录。

### 免责声明与网络配置

**网络环境与工具免责声明：**

* **逻辑解耦**：本指令的核心功能是饮食营养分析。指令中包含的“网络自动化”步骤（如路由模式切换动作）仅为**可选的自动化逻辑建议**。本项目的基础功能并不依赖于任何特定的第三方网络工具。
* **不提供工具**：本项目**不提供**、**不内置**、亦**不推广**任何特定的 VPN、代理或网络绕过类应用程序。文档中出现的任何第三方 App 动作仅用于展示自动化流程控制的技术实现。
* **用户责任**：用户需自行确保其网络环境及所使用的任何第三方工具符合其所在地（包括但不限于中国大陆地区）的法律法规。作者不对用户因网络配置不当或违反相关法律法规而产生的任何后果承担法律责任。
---

## ⚖️ License / 开源协议

This project is licensed under the [MIT License](https://www.google.com/search?q=LICENSE).
本项目采用 [MIT 开源协议](https://www.google.com/search?q=LICENSE)。
