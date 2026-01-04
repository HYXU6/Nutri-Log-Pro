# Nutri-Log Pro 🍎

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform: iOS](https://img.shields.io/badge/Platform-iOS-blue.svg)](https://www.apple.com/ios/)

[English](#english) | [中文说明](#chinese-description)

---

<a name="english"></a>
## English

**Nutri-Log Pro** is an intelligent dietary tracking tool based on iOS Shortcuts and the Google Gemini 3 Flash multimodal model. It analyzes food photos to calculate nutritional components and automatically synchronizes data to multiple platforms.

### ✨ Key Features
- **📸 Multi-channel Input**: Launch directly from the home screen (Camera) or via the "Share Sheet" in the Photos app.
- **🧠 Deep Nutritional Analysis**: Leverages Gemini 3 Flash to estimate Calories, Protein, Carbs, Fat, Fiber, Sodium, and Sugar.
- **🏥 Health Integration**: Automatically writes recognition results into the Apple Health database.
- **📅 Dual-Channel Logging (Highly Customizable)**:
  - **Apple Journal**: Creates a native entry with original photos and detailed logs (Requires iOS 19.1+).
  - **Apple Notes**: Appends the same data to a continuous "Diet Log" note for easy batch review.
  - *Users can freely keep or delete either module based on personal preference.*
- **🛡️ Robust Engineering**: Includes automated network environment switching and image compression.

### 🚀 Quick Start
1. **Prerequisites**: An iPhone, the "Shortcuts" app, and a **Google Gemini API Key**.
2. **Install**: Download the `.shortcut` file from the [Releases](#) page.
3. **Configure**: Enter your API Key in the "Get Contents of URL" action.
4. **Customization**: 
   - If you only need **Journal**, delete the "Append to Note" action.
   - If you only need **Notes**, delete the "Create Journal Entry" action.

---

<a name="en-disclaimer"></a>
### 🛡️ Disclaimer & Network Configuration
**Network Environment & Tooling Disclaimer:**
* **Decoupled Logic**: This shortcut provides a framework for nutritional analysis. The integrated "Network Automation" steps (such as routing mode switches) are **optional implementation suggestions**. The core functionality of this project is independent of any specific third-party network tool.
* **No Bundled Tools**: This project **does not** provide, bundle, or promote any specific VPN, proxy, or circumvention applications. Any third-party app actions shown in the documentation are for demonstration of automation logic only.
* **User Responsibility**: Users are solely responsible for ensuring that their network environment and any third-party tools used comply with their local laws and regulations. The author assumes no liability for any misuse or legal consequences arising from the user's network configuration.

---

<a name="chinese-description"></a>
## 中文说明

**Nutri-Log Pro** 是一款基于 iOS 快捷指令和 Google Gemini 3 Flash 多模态大模型的智能饮食追踪工具。它能通过分析食物照片计算营养成分，并自动将数据同步至多个平台。

### ✨ 核心特性
- **📸 多渠道输入**：支持桌面图标直接启动或在相册通过“共享表单”一键分享识别。
- **🧠 深度营养分析**：利用 Gemini 3 Flash 模型，精准估算热量、蛋白质、碳水、脂肪、纤维素、钠及糖分。
- **🏥 健康闭环**：识别结果自动写入系统级 Apple Health 数据库。
- **📅 双渠道记录（高度可定制）**：
  - **原生手记 (Journal)**：创建包含原始照片及营养日志的精美分录（需 iOS 19.1+）。
  - **备忘录 (Notes)**：在指定的“饮食记录”文档中追加文字，方便批量查看。
  - *用户可以根据个人喜好，自由保留或删除其中任何一个记录模块。*
- **🛡️ 健壮性设计**：内置网络环境自动切换逻辑，支持图像压缩传输。

### 🚀 快速开始
1. **环境要求**：安装了“快捷指令”的 iPhone，以及一个 **Google Gemini API Key**。
2. **安装步骤**：从 [Releases](#) 页面下载本仓库提供的 `.shortcut` 文件。
3. **配置 Key**：在快捷指令的“获取 URL 内容”动作中填入你的 API Key。
4. **个性化定制**：
   - 如果您只需要**手记**功能，请在快捷指令中删除“追加到备忘录”动作。
   - 如果您只需要**备忘录**功能，请在快捷指令中删除“创建手记分录”动作。

---

<a name="cn-disclaimer"></a>
### 🛡️ 免责声明与网络配置说明
**网络环境与工具免责声明：**
* **逻辑解耦**：本指令的核心功能是饮食营养分析。指令中包含的“网络自动化”步骤（如路由模式切换动作）仅为**可选的自动化逻辑建议**。本项目的基础功能并不依赖于任何特定的第三方网络工具。
* **不提供工具**：本项目**不提供**、**不内置**、亦**不推广**任何特定的 VPN、代理或网络绕过类应用程序。文档中出现的任何第三方 App 动作仅用于展示自动化流程控制的技术实现。
* **用户责任**：用户需自行确保其网络环境及所使用的任何第三方工具符合其所在地（包括但不限于中国大陆地区）的法律法规。作者不对用户因网络配置不当或违反相关法律法规而产生的任何后果承担法律责任。

---

## ⚖️ License / 开源协议
This project is licensed under the [MIT License](LICENSE).
本项目采用 [MIT 开源协议](LICENSE)。
