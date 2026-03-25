# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

这是谢云龙的个人主页项目,部署在GitHub Pages上。项目使用纯HTML、CSS和JavaScript构建,内容与展示分离,所有数据存储在`data/content.json`文件中。

## 项目结构

```
xyl-muse.github.io/
├── assets/
│   ├── images/              # 图片资源
│   └── styles/
│       └── main.css         # 主样式文件
├── data/
│   └── content.json         # 内容数据文件(核心)
├── resume/
│   ├── 谢云龙_2025.pdf     # 简历PDF
│   └── 谢云龙_2025.md      # 简历Markdown版本
├── index.html               # 主页(包含JavaScript逻辑)
└── README.md               # 项目说明
```

## 核心文件说明

### data/content.json
这是最核心的数据文件,包含所有个人信息、技能、项目和经历。页面通过JavaScript动态加载此文件来渲染内容。

主要数据结构:
- `personal`: 个人基本信息(姓名、职位、描述、邮箱、位置等)
- `social`: 社交链接数组
- `skills`: 技能分类数组,每个分类包含多个技能项及熟练度
- `projects`: 项目展示数组
- `experience`: 工作经历数组
- `about`: 关于我的描述
- `education`: 教育经历

### index.html
包含所有HTML结构和JavaScript逻辑,包括:
- 主题切换(深色/浅色)
- 平滑滚动
- 滚动动画
- 动态内容渲染

## 常用命令

### 本地预览
直接在浏览器中打开 `index.html` 即可预览,无需构建工具。

### 更新内容
编辑 `data/content.json` 文件来更新所有个人信息、技能、项目和经历。

### 更新简历

#### 1. 文件位置
简历文件位于 `resume/` 目录下:
- `谢云龙_2025.pdf`: 简历PDF版本
- `谢云龙_2025.md`: 简历Markdown版本

#### 2. 如何更新简历

**步骤1: 替换PDF文件**
将新的简历PDF文件放入 `resume/` 目录中。

**步骤2: 更新配置**
编辑 `data/content.json` 文件,修改 `personal.resumePdf` 字段:
```json
"personal": {
    "name": "谢云龙",
    "title": "信息安全高级工程师 | 网络安全专家",
    // ...
    "resumePdf": "resume/你的新简历文件名.pdf"
}
```

**步骤3: 更新Markdown版本**
同时更新 `resume/谢云龙_2025.md` 文件,保持与PDF内容同步。

#### 3. 下载链接
下载链接位于页面的英雄区域(hero section),指向 `resume/谢云龙_2025.pdf`。通过配置 `data/content.json` 中的 `personal.resumePdf` 字段可以轻松修改下载链接。

#### 4. 后备机制
如果 `data/content.json` 中未配置,页面将使用硬编码的默认路径 `resume/谢云龙_2025.pdf`。

## 开发注意事项

1. **内容驱动**: 所有展示内容都在`data/content.json`中,修改HTML/CSS前先考虑是否可以通过修改数据实现。
2. **简历同步**: 更新简历时,需要同时更新`resume/`目录下的PDF和Markdown文件,并同步更新`data/content.json`中的相关内容。
3. **部署**: 推送到main分支后,GitHub Pages会自动部署。

## 重要数据映射

根据简历`resume/谢云龙_2025.md`,以下是关键信息:
- 姓名: 谢云龙
- 职位: 信息安全高级工程师
- 工作年限: 4年
- 核心技能: 信息安全体系建设、AI安全、反入侵防御、SOC、EDR、WAF、NDR、DLP、IAM/IDM
- 工作经历: 隆基绿能科技股份有限公司(2022.07至今)
- 教育背景: 西安电子科技大学 信息安全本科
