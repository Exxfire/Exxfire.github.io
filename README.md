# Exxfire's Blog

[![Build Status](https://github.com/Exxfire/exxfire.github.io/workflows/Build%20and%20Deploy/badge.svg)](https://github.com/Exxfire/exxfire.github.io/actions)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Exxfire.github.io-blue.svg)](https://exxfire.github.io)
[![Jekyll](https://img.shields.io/badge/Jekyll-4.2+-red.svg)](https://jekyllrb.com/)

## 📝 关于

这是我的个人技术博客，使用 [Jekyll](https://jekyllrb.com/) 构建，托管在 [GitHub Pages](https://pages.github.com/) 上。

博客地址：[https://exxfire.github.io](https://exxfire.github.io)

## ✨ 功能特性

- 📱 响应式设计，支持移动端
- 🎨 现代化UI设计
- 🔍 SEO优化
- 📊 支持Google Analytics
- 💬 支持评论系统（Disqus/GitHub Discussions）
- 📱 社交媒体分享
- 📚 文章分类和标签
- 🔍 搜索功能
- 📄 分页功能
- 📂 归档页面
- 📡 RSS订阅

## 🛠️ 技术栈

- **静态站点生成器**: Jekyll 4.2+
- **主题**: Minima + Jekyll-YAMT
- **部署**: GitHub Pages
- **评论系统**: Disqus / GitHub Discussions
- **分析工具**: Google Analytics
- **CDN**: GitHub Pages CDN

## 🚀 本地开发

### 环境要求

- Ruby 2.6.0 或更高版本
- RubyGems
- GCC 和 Make

### 安装步骤

1. **克隆仓库**
   ```bash
   git clone https://github.com/Exxfire/exxfire.github.io.git
   cd exxfire.github.io
   ```

2. **安装依赖**
   ```bash
   bundle install
   ```

3. **启动本地服务器**
   ```bash
   bundle exec jekyll serve
   ```

4. **访问本地站点**
   打开浏览器访问 [http://localhost:4000](http://localhost:4000)

### 开发命令

```bash
# 启动开发服务器（带实时重载）
bundle exec jekyll serve --livereload

# 构建生产版本
bundle exec jekyll build

# 检查构建结果
bundle exec jekyll build --profile

# 清理缓存
bundle exec jekyll clean
```

## 📁 项目结构

```
exxfire.github.io/
├── _config.yml          # Jekyll配置文件
├── _posts/              # 博客文章
├── _pages/              # 静态页面
├── _data/               # 数据文件
├── _layouts/            # 布局模板
├── _includes/           # 包含文件
├── _sass/               # Sass样式文件
├── assets/              # 静态资源
├── images/              # 图片文件
├── Gemfile              # Ruby依赖
├── README.md            # 项目说明
└── index.markdown       # 首页
```

## 📝 写作指南

### 创建新文章

1. 在 `_posts/` 目录下创建新文件
2. 文件名格式：`YYYY-MM-DD-title.md`
3. 添加Front Matter：

```yaml
---
layout: post
title: "文章标题"
date: 2024-01-01 12:00:00 +0800
categories: [技术, 编程]
tags: [Jekyll, GitHub Pages, 博客]
author: Exxfire
comments: true
share: true
---
```

### 文章格式

- 使用Markdown语法
- 支持代码高亮
- 支持数学公式（LaTeX）
- 支持图片和视频嵌入
- 支持表格和列表

## 🎨 自定义主题

### 修改样式

1. 在 `_sass/` 目录下创建自定义样式文件
2. 在 `assets/css/` 目录下创建主样式文件
3. 在 `_config.yml` 中配置Sass选项

### 添加新页面

1. 在根目录或 `_pages/` 目录下创建 `.md` 文件
2. 添加Front Matter：

```yaml
---
layout: page
title: "页面标题"
permalink: /page-url/
---
```

## 🔧 配置说明

### 主要配置项

- `title`: 网站标题
- `description`: 网站描述
- `url`: 网站URL
- `author`: 作者信息
- `social`: 社交媒体链接
- `plugins`: 启用的插件
- `theme`: 使用的主题

### 插件配置

- `jekyll-feed`: RSS订阅
- `jekyll-seo-tag`: SEO优化
- `jekyll-sitemap`: 站点地图
- `jekyll-paginate`: 分页功能
- `jekyll-archives`: 归档功能

## 📊 部署

### GitHub Pages

1. 推送代码到GitHub
2. 在仓库设置中启用GitHub Pages
3. 选择部署分支（通常是 `main` 或 `gh-pages`）

### 自定义域名

1. 在 `_config.yml` 中设置 `url`
2. 在GitHub Pages设置中添加自定义域名
3. 创建 `CNAME` 文件

## 🤝 贡献

欢迎提交Issue和Pull Request！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 📞 联系方式

- 📧 Email: 1009524027@qq.com
- 💻 GitHub: [@Exxfire](https://github.com/Exxfire)
- 🔗 博客: [https://exxfire.github.io](https://exxfire.github.io)

## 🙏 致谢

- [Jekyll](https://jekyllrb.com/) - 静态站点生成器
- [Minima](https://github.com/jekyll/minima) - Jekyll默认主题
- [Jekyll-YAMT](https://github.com/PandaSekh/Jekyll-YAMT) - 现代化主题
- [GitHub Pages](https://pages.github.com/) - 免费托管服务

---

⭐ 如果这个项目对你有帮助，请给它一个星标！