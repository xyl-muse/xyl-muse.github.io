# 谢云龙的个人主页

这是一个现代化、专业的个人主页项目，使用HTML、CSS和JavaScript构建，部署在GitHub Pages上。

## 🌟 特性

- 🎨 **现代化设计** - 极简现代风格，玻璃态设计
- 🌓 **深色/浅色双主题** - 支持主题切换
- 📱 **响应式布局** - 完美适配各种设备
- ⚡ **高性能** - 轻量快速，无框架依赖
- 🚀 **易部署** - GitHub Pages自动部署
- 📊 **数据驱动** - 内容与展示分离，易于维护

## 📁 项目结构

```
xyl-muse.github.io/
├── assets/
│   ├── images/              # 图片资源
│   └── styles/
│       └── main.css         # 主样式文件
├── data/
│   └── content.json         # 内容数据文件
├── resume/
│   └── 谢云龙_2025.pdf     # 简历PDF
├── index.html               # 主页
├── README.md               # 项目说明
└── .gitignore              # Git忽略配置
```

## 🚀 快速开始

### 本地预览

直接在浏览器中打开 `index.html` 即可预览。

### 修改内容

所有内容都存储在 `data/content.json` 文件中，您可以直接编辑该文件来更新个人信息、技能、项目和经历。

### 添加图片

将图片放在 `assets/images/` 目录下，并在 `data/content.json` 中引用相应的路径。

## 🎯 内容模块

### 1. 英雄区域 (Hero)
- 个人姓名和职位
- 简短介绍
- 下载简历和查看项目按钮
- 社交链接

### 2. 关于我 (About)
- 个人简介
- 技能标签
- 兴趣爱好

### 3. 技术技能 (Skills)
- 技能分类展示
- 技能掌握程度图表
- 动态进度条

### 4. 精选项目 (Projects)
- 项目卡片网格
- 技术栈标签
- GitHub和演示链接

### 5. 工作经历 (Experience)
- 时间线展示
- 公司和职位信息
- 工作内容和成就

### 6. 联系方式 (Contact)
- 邮箱
- 位置
- 网站链接

## 🔧 自定义

### 修改主题颜色

在 `assets/styles/main.css` 中修改 CSS 变量：

```css
:root {
  --accent-primary: #4f46e5;    /* 主色调 */
  --accent-secondary: #3b82f6;  /* 次要色调 */
  /* ... */
}
```

### 更新个人信息

编辑 `data/content.json` 文件，修改相应字段即可。

## 📱 响应式断点

- **移动端**: < 640px
- **平板**: 640px - 1024px
- **桌面**: > 1024px

## 🚀 部署到 GitHub Pages

### 方法1：直接部署

1. 确保仓库名称为 `your-username.github.io`
2. 将代码推送到 `main` 分支
3. 在仓库设置中启用 GitHub Pages，源选择 `main` 分支

### 方法2：使用 GitHub Actions

创建 `.github/workflows/deploy.yml` 文件配置自动部署。

## 📄 许可证

MIT License - 欢迎自由使用和修改。

## 🤝 贡献

如果您发现任何问题或有改进建议，欢迎创建 Issue 或 Pull Request。

---

**用 ❤️ 和代码构建**