## 🔗链接：https://markdown-practice.lhpgmc.cn/
## 📝 项目介绍

Markdown语法练习器是一个交互式Web应用，帮助用户学习和掌握Markdown语法。该应用基于Cloudflare的技术栈构建，包括Cloudflare Pages作为前端和Cloudflare Worker作为后端，并利用Cloudflare D1数据库和KV存储来保存用户练习记录和题目数据。

### ✨ 主要功能

- **多级难度题目**：提供初级、中级和高级三个难度级别的Markdown语法练习题
- **实时编辑与预览**：在编辑区输入Markdown代码，即时在预览区查看渲染效果
- **智能语法验证**：自动检查用户输入的Markdown代码是否符合题目要求
- **详细错误反馈**：当语法有误时，提供具体的错误信息和改进建议
- **练习记录保存**：记录用户的练习历史，包括题目、难度级别和完成情况
- **学习进度统计**：展示用户的学习进度和成绩统计
- **响应式设计**：适配桌面和移动设备的界面布局

## 🔍 项目预览

![Image](https://github.com/user-attachments/assets/5954fa02-5c37-4081-b56e-6e7928605bb9)

## 🛠️ 技术栈

- **前端**：HTML, CSS, JavaScript
  - Marked.js (Markdown解析)
  - Highlight.js (代码高亮)
  - DOMPurify (安全渲染)
- **后端**：Cloudflare Worker (JavaScript)
- **数据存储**：
  - Cloudflare D1 (SQL数据库)
  - Cloudflare KV (键值存储)
- **部署**：Cloudflare Pages, Cloudflare Dashboard

## 📂 项目结构

```
markdown-practice/
├── frontend/                # Cloudflare Pages前端
│   ├── index.html           # 主HTML文件
│   ├── public/              # 静态资源目录
│   └── src/                 # 源代码目录
│       ├── app.js           # 主要应用逻辑
│       ├── api-integration.js # API集成逻辑
│       └── styles.css       # 样式表
│
├── worker/                  # Cloudflare Worker后端
│   ├── index.js             # Worker主代码
│   └── wrangler.toml        # Worker配置文件
```


## 📱 使用说明

### 基本操作流程

1. **选择难度级别**：在页面顶部选择初级、中级或高级难度。
2. **生成题目**：点击"生成新题目"按钮获取一个随机的Markdown练习题。
3. **编写Markdown**：在编辑区输入你的Markdown代码，右侧会实时显示渲染效果。
4. **验证答案**：点击"验证答案"按钮检查你的代码是否符合要求。
5. **查看反馈**：系统会显示验证结果和改进建议。
6. **练习记录**：页面底部会显示你的练习历史记录。

### 学习建议

- 从初级题目开始，逐步提高难度
- 尝试不看示例自己编写Markdown代码
- 对照错误提示修改代码，直到正确
- 定期复习已完成的题目，巩固记忆
- 尝试将学到的语法应用到实际文档编写中

# 感想
其实本项目完全由manus起搞(这篇blog也是它写的），chatgpt debug现在ai真的发达多了，部署也非常简单，GitHub我还没玩透，摸清楚了我会把这个项目开源的——2025.5.24
