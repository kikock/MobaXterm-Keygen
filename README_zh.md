# MobaXterm Keygen & Customizer 🚀

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Version](https://img.shields.io/badge/Version-v2.7-green.svg)
![Compatibility](https://img.shields.io/badge/Compatible-v20.X%20|%20v25.4%20|%20v26.0-orange)

> ⭐ **如果您觉得有用，请给这个仓库点个星！** ⭐

## 概述

这是一个现代、用户友好的 Web 工具，用于生成 MobaXterm 的激活密钥并对其进行自定义。MobaXterm 是 Windows 上终极的终端模拟器，集成了 X11 服务器、SSH 客户端和全面的网络工具集。

## 功能特性

- **✨ 简洁现代的 UI** - 响应式设计，针对桌面和移动设备进行了优化
- **🌓 深色/浅色模式** - 一键切换主题
- **🔒 支持多个版本** - 为不同的 MobaXterm 版本生成密钥
- **👥 自定义用户数** - 指定并发用户数量
- **💾 一键下载** - 即时下载您的自定义激活文件
- **🔧 完整的自定义器** - 无需官方自定义工具即可创建个性化设置
- **🖼️ 支持自定义 Logo** - 使用您自己的图片替换默认的 MobaXterm Logo
- **📑 书签管理器** - 预定义 SSH、FTP 和其他连接配置文件
- **🔌 插件集成** - 在您的自定义配置中包含插件

## 兼容性

- 适用于 **MobaXterm 版本 20.X、25.4 和 26.0**
- 支持便携版和安装版

## 使用方法

### 密钥生成器 (Key Generator)

1. **访问生成器**：前往 [MobaXterm Key Generator](https://moba-xterm-keygen.vercel.app/)
2. **填写表单**：
   - 选择所需的 MobaXterm 版本 (Edition)
   - 输入用户名（仅限字母）
   - 选择您的 MobaXterm 版本号（20.X 或 26.X）
   - 指定用户数量
3. **下载**：点击 "Download Key" 获取您的 `Custom.mxtpro` 文件
4. **激活**：将生成的文件放入您的 MobaXterm 安装目录：
   ```
   C:\Program Files (x86)\Mobatek\MobaXterm
   ```

### 自定义器 (Customizer)

1. **转到 Customizer 标签页**
2. **配置您的设置**：
   - **Banner**：创建个性化的欢迎信息
   - **Profile**：配置自定义 bash profile（类似于 Linux 中的 /etc/profile）
   - **Settings**：开启/关闭 MobaXterm 功能
   - **Logo**：上传您的自定义 Logo 图片
   - **Bookmarks**：为您的用户创建预定义连接
   - **Plugins**：添加可选的 MobaXterm 插件 (.mxt3 文件)
3. **生成设置**：点击 "Generate Configuration File" 下载您的设置
4. **应用设置**：使用下文介绍的方法之一应用您的自定义设置

### 设置合并器 (Settings Merger)

1. **转到 Custom Settings Merger 标签页**
2. **上传文件**：
   - 您的许可证密钥文件 (`Custom.mxtpro`)
   - 您的自定义设置文件 (`MobaXterm customization.custom`)
3. **合并**：创建一个包含许可证和自定义设置的单一文件
4. **部署**：将合并后的 `Custom.mxtpro` 复制到您的 MobaXterm 安装目录

## Cloudflare Pages 部署教程

您可以轻松将此项目部署到 Cloudflare Pages，只需几个步骤：

### 准备工作
1. 拥有一个 [Cloudflare](https://www.cloudflare.com/) 账户。
2. 将本项目 Fork 到您的 GitHub 账户。

### 方法一：通过 Cloudflare Dashboard (推荐)
1. 登录 Cloudflare Dashboard。
2. 进入 **Compute (Workers & Pages)** -> **Overview**。
3. 点击 **Create application** -> **Pages** -> **Connect to Git**。
4. 选择您 Fork 的 `MobaXterm-Keygen` 仓库。
5. 在 **Set up builds and deployments** 页面：
   - **Project name**: 保持默认或自定义
   - **Production branch**: `main` (或 `master`)
   - **Framework preset**: `None`
   - **Build command**: (留空)
   - **Build output directory**: `.` (输入一个点，代表根目录)
6. 点击 **Save and Deploy**。

### 方法二：使用 GitHub Actions 自动部署
如果您希望通过 GitHub Actions 推送代码时自动部署，请按照以下步骤操作：

1. **获取 Cloudflare API Token**:
   - 访问 [Cloudflare Profile API Tokens](https://dash.cloudflare.com/profile/api-tokens)。
   - 点击 **Create Token** -> 使用 **Edit Cloudflare Workers** 模板。
   - 确保包含 `Account | Cloudflare Pages | Edit` 权限。

2. **获取 Account ID**:
   - 在 Cloudflare Dashboard 的任意页面右下角或 URL 中可以找到 `Account ID`。

3. **配置 GitHub Secrets**:
   - 在您的 GitHub 仓库中，进入 **Settings** -> **Secrets and variables** -> **Actions**。
   - 点击 **New repository secret**。
   - 添加 `CLOUDFLARE_API_TOKEN`。
   - 添加 `CLOUDFLARE_ACCOUNT_ID`。

4. **推送代码**:
   - 本项目已包含 `.github/workflows/deploy.yml`。
   - 只要您向 `main` 分支推送代码，GitHub Actions 就会自动触发并将最新版本部署到 Cloudflare Pages。

## 安装指南

### 步骤 1：下载 MobaXterm
从 [MobaXterm 官方网站](https://mobaxterm.mobatek.net/download-home-edition.html) 下载最新版本。

### 步骤 2：生成您的密钥和自定义设置
使用我们的工具：
1. 创建您的激活密钥
2. 自定义您的设置（可选）
3. 合并您的许可证与自定义设置（可选）

### 步骤 3：激活 MobaXterm
1. 找到您的 MobaXterm 安装文件夹：
   - **默认路径**：`C:\Program Files (x86)\Mobatek\MobaXterm`
   - 或者右键点击 MobaXterm 快捷方式并选择“打开文件所在位置”
2. 将 `Custom.mxtpro` 文件复制到此目录
3. 启动 MobaXterm - 您的许可证和自定义设置现在应该已应用！

### 替代自定义方法

MobaXterm.exe 有一个自定义器模式，您可以通过添加参数 `-customizer` 来访问：

```powershell
.\MobaXterm.exe -customizer
```

这个官方工具也允许您导出设置到名为 `MobaXterm customization.custom` 的文件。我们的基于 Web 的自定义器提供了类似的功能，但可以直接在浏览器中访问。

## 故障排除

1. **激活无效？**
   - 确认您使用的是兼容版本（20.X, 25.4, 或 26.0）
   - 确保文件在正确的位置
   - 检查文件是否确切命名为 `Custom.mxtpro`

2. **生成密钥时出错？**
   - 确保所有表单字段填写正确
   - 用户名必须仅包含字母（无空格、数字或特殊字符）
   - 尝试刷新页面并重新生成

3. **自定义未应用？**
   - 确认您已将自定义设置与许可证文件合并
   - 确保合并后的文件确切命名为 `Custom.mxtpro`
   - 将文件放入安装目录后，尝试重启 MobaXterm

## 技术细节

此工具使用客户端处理来根据您的输入生成有效的许可证密钥和自定义文件。所有内容直接在您的浏览器中生成——没有任何数据发送到任何服务器，确保您的隐私和安全。

## 免责声明

此工具仅供教育目的使用。请通过购买许可证支持开发人员以进行商业用途。

## 开发

### 构建技术栈
- Vue.js
- Tailwind CSS
- Modern JavaScript

### 版本历史
- **v2.7** - 增加对版本 26.0 的支持
- **v2.6** - 增加对版本 25.4 的支持
- **v2.5** - 增加对版本 25.3 的支持
- **v2.4** - 增加完整的 MobaXterm 自定义器功能
- **v2.3** - 增加自定义设置合并器
- **v2.2** - 深色模式和移动端优化
- **v2.1** - 增加对版本 25.2 的支持
- **v2.0** - 重大 UI 重设计
- **v1.0** - 初始发布

---

Created with ❤️ by Zarfala

---

⭐ [Star this repository on GitHub!](https://github.com/zarfadev/MobaXterm-Keygen) ⭐
