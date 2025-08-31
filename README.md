# 提莫VPN - 动态跳转引导页 (Teemo VPN - Dynamic Redirect Landing Page)

这是一个现代化、带有丰富动态效果的网站跳转引导页。它被设计用于在用户访问主页前，提供一个视觉吸引力强、信息清晰的过渡界面。页面包含一个可配置时长的倒计时，结束后会自动跳转到目标网站，同时用户也可以选择手动立即跳转。


**[在线演示链接(https://www.timo.pp.ua)**

<img width="1914" height="910" alt="image" src="https://github.com/user-attachments/assets/c7d0200f-5103-4cea-aaac-5bb3b20d226d" />


---

## ✨ 主要特点 (Features)

本引导页不仅仅是一个简单的倒计时页面，它融合了多种现代网页技术，以提供卓越的用户体验。

### 视觉效果
* **🚀 3D粒子背景:** 基于 `Three.js` 创建的互动式星空粒子背景，会随着鼠标的移动而细腻地变换视角，营造出置身于宇宙空间的沉浸感。
* **🎨 动态渐变背景:** 流畅变换的四色渐变背景，为整个页面提供了富有科技感和高级感的基调。
* **💎 玻璃拟态 (Glassmorphism) 卡片:** 中心的内容区域采用流行的“毛玻璃”效果，搭配半透明边框，在复杂的背景上也能保证信息的清晰可读性。

### 交互与动画
* **🎬 优雅的入场动画:** 页面加载时，所有文本和控件元素均采用自下而上的淡入动画，使内容呈现过程流畅自然。
* **⏳ 动态SVG倒计时:** 倒计时器以SVG圆环进度条的形式动态展示时间流逝，直观且美观。
* **⚡️ 加速“跃迁”效果:** 随着倒计时临近结束，背景中的粒子会显著加速飞行，为即将发生的页面跳转营造出一种“时空穿梭”前的紧张感和期待感。

### 功能与易用性
* **🔧 **极其简单的配置**: 打开文件即可在最顶部找到配置区域，修改一处网址即可同步所有链接，无需任何编程知识。**
* **🌐 双语支持:** 内置 **中文/English** 一键切换功能，无需刷新页面即可更改所有文本内容。
* **💾 语言记忆:** 用户的语言偏好会自动保存在浏览器的 `localStorage` 中，下次访问时将自动应用。
* **📱 响应式设计:** 基于 `Tailwind CSS` 构建，确保页面在桌面、平板和手机等不同尺寸的设备上都能获得完美的显示效果。

---

## 🛠️ 技术栈 (Technology Stack)

* **HTML5:** 页面结构
* **JavaScript (ES6):** 核心交互逻辑与动画控制
* **Tailwind CSS:** 快速、高效的原子化CSS框架
* **Three.js:** 驱动3D粒子背景

---

## 🚀 如何使用 (How to Use)

这是一个纯前端的单文件项目，无需复杂的构建或安装过程。

1.  克隆本仓库或直接下载 `index.html` 文件。
2.  使用任意文本编辑器（如记事本、VS Code等）打开 `index.html` 文件，根据下一节的指南进行修改。
3.  保存文件，用浏览器打开即可查看您的定制效果。

---

## ☁️ 部署到 Vercel (Deploy to Vercel)

您可以将此项目免费部署到 Vercel 平台，以获得一个公开、高速的网址。

### 一键部署 (推荐)

1.  **前提**: 您需要先将此项目上传到您自己的 **公开** GitHub 仓库。
2.  **修改链接**: **编辑本 README 文件**，将下方按钮链接中的 `https://github.com/YOUR_USERNAME/YOUR_REPO_NAME` 替换为您自己的仓库地址。
3.  **点击部署**: 保存并提交文件，然后点击下方的部署按钮：

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/YOUR_USERNAME/YOUR_REPO_NAME)

4.  Vercel 将会引导您完成账户创建和项目部署，全程通常无需任何额外配置，点击几下即可完成。

### 手动部署

1.  注册并登录您的 [Vercel](https://vercel.com/) 账户。
2.  点击 "Add New..." -> "Project"。
3.  选择 "Import Git Repository" 并导入您存放此项目的 GitHub 仓库。
4.  Vercel 会自动识别这是一个无框架的静态网站。您无需更改任何设置，直接点击 "Deploy" 即可成功部署。

---

## ⚙️ 自定义指南 (Customization)

您可以非常轻松地将此模板用于您自己的项目。**打开 `index.html` 文件，您将在最上方看到一个清晰的配置区域**。

```html
<script>
    // --- 1. 核心网址设置 (***最重要***) ---
    const SITE_CONFIG = {
        url: '[https://www.your-website.com](https://www.your-website.com)',      // 最终要跳转到的完整网址
        name: 'your-website.com'              // 显示在页面底部的网址文本
    };

    // --- 2. 其他参数与文本设置 ---
    const CONFIG = {
        // ...
        countdownSeconds: 10,
        // ...
        translations: {
            zh: {
                page_title: '您的网站标题',
                main_title: '您的项目名称',
                // ...
            },
            en: {
                // ...
            }
        }
    };
</script>

