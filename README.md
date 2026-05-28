# 智课件 - AI智能PPT生成器

> 🎓 中小学教师的智能课件生成助手，输入教案 → AI生成 → 直接上课

## 功能特点

- ✅ **四种输入方式**：文本粘贴 / 大纲粘贴 / 课程目标 / 拍照OCR识别
- ✅ **语数英全覆盖**：语文/数学/英语各4套专业模板
- ✅ **AI智能生成**：基于SiliconFlow API理解教案结构
- ✅ **在线预览编辑**：生成后实时预览，支持修改标题/内容/换模板
- ✅ **导出.pptx**：下载标准PowerPoint格式文件

## 快速开始

### 方式一：在线使用（推荐）
👉 **https://lxztry.github.io/aicourse/**

### 方式二：本地运行
```bash
# 直接用浏览器打开 index.html
open index.html
# 或使用 Python 简易服务器
python -m http.server 8080
# 访问 http://localhost:8080
```

## 使用流程

1. 输入 SiliconFlow API Key（首次使用时填写）
2. 选择学科（语文📖 / 数学📐 / 英语🔤）
3. 选择输入方式并粘贴/上传教案内容
4. 点击「开始生成PPT」，等待10-30秒
5. 预览并编辑，满意后导出 .pptx

## 技术栈

- **前端**：HTML5 + CSS3 + Vanilla JS（单文件，零依赖安装）
- **AI服务**：SiliconFlow API（Qwen2.5-7B）
- **PPT生成**：PptxGenJS
- **OCR识别**：Tesseract.js（本地离线识别）
- **Markdown渲染**：Marked.js

## 获取 API Key

1. 访问 [SiliconFlow](https://www.siliconflow.cn/) 注册账号
2. 进入控制台 → API Keys → 创建新密钥
3. 填入应用即可使用

## 模板说明

| 学科 | 模板名称 | 适用场景 |
|------|---------|---------|
| 语文 | 诗词赏析 | 古诗词教学 |
| 语文 | 阅读理解 | 课文精读 |
| 语文 | 作文指导 | 写作教学 |
| 语文 | 综合课件 | 一般语文课 |
| 数学 | 概念引入 | 新知讲解 |
| 数学 | 计算练习 | 练习课 |
| 数学 | 应用题 | 应用题教学 |
| 数学 | 复习课 | 单元复习 |
| 英语 | 听说训练 | 听说课 |
| 英语 | 读写练习 | 读写课 |
| 英语 | 语法讲解 | 语法课 |
| 英语 | 复习课 | 单元复习 |

## 项目结构

```
aicourse/
├── index.html          # 主应用（单文件）
├── marked.min.js       # Markdown渲染
├── pptxgen.bundle.js  # PPT生成库
└── tesseract.min.js    # OCR识别库
```

## License

MIT License - 欢迎改进和二次开发