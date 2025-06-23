# Exxfire's Blog

[![Build Status](https://github.com/Exxfire/exxfire.github.io/workflows/Build%20and%20Deploy/badge.svg)](https://github.com/Exxfire/exxfire.github.io/actions)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Exxfire.github.io-blue.svg)](https://exxfire.github.io)
[![Jekyll](https://img.shields.io/badge/Jekyll-4.4.1-red.svg)](https://jekyllrb.com/)

## 📝 关于

这是我的个人技术博客，使用 [Jekyll](https://jekyllrb.com/) 构建，托管在 [GitHub Pages](https://pages.github.com/) 上。

博客地址：[https://exxfire.github.io](https://exxfire.github.io)

## ✨ 功能特性

- 📱 响应式设计，支持移动端
- 🎨 现代化UI设计，自定义样式
- 🔍 SEO优化
- 📊 支持Google Analytics
- 💬 支持评论系统（Disqus/GitHub Discussions）
- 📱 社交媒体分享
- 📚 文章分类和标签
- 🔍 搜索功能
- 📄 分页功能
- 📂 归档页面
- 📡 RSS订阅
- 🚀 GitHub Actions自动部署
- 🎯 自定义布局和主题

## 🛠️ 技术栈

- **静态站点生成器**: Jekyll 4.4.1
- **主题**: Minima 2.5 + 自定义样式
- **部署**: GitHub Pages + GitHub Actions
- **评论系统**: Disqus / GitHub Discussions
- **分析工具**: Google Analytics
- **CDN**: GitHub Pages CDN

## 🚀 本地开发

### 环境要求

- Ruby 3.2+ 或更高版本
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

# 添加Linux平台支持（用于GitHub Actions）
bundle lock --add-platform x86_64-linux
```

## 📁 项目结构

```
exxfire.github.io/
├── _config.yml              # Jekyll配置文件
├── _layouts/                # 自定义布局文件
│   ├── default.html         # 默认布局
│   ├── page.html            # 页面布局
│   ├── post.html            # 文章布局
│   └── home.html            # 首页布局
├── _posts/                  # 博客文章
├── _data/                   # 数据文件
│   └── navigation.yml       # 导航配置
├── assets/                  # 静态资源
│   └── main.scss            # 自定义样式文件
├── .github/                 # GitHub配置
│   └── workflows/           # GitHub Actions工作流
│       └── jekyll.yml       # 自动部署配置
├── _404.html               # 404错误页面
├── about.markdown          # 关于页面
├── index.markdown          # 首页
├── Gemfile                 # Ruby依赖
├── Gemfile.lock            # 依赖锁定文件
├── README.md               # 项目说明
├── LICENSE                 # 许可证文件
└── .gitignore              # Git忽略文件
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

### 样式自定义

项目使用自定义的SCSS样式文件 `assets/main.scss`，包含：

- 响应式布局设计
- 现代化UI组件
- 自定义颜色方案
- 移动端优化
- 动画效果

### 布局自定义

在 `_layouts/` 目录下包含以下自定义布局：

- `default.html` - 基础布局模板
- `page.html` - 静态页面布局
- `post.html` - 文章页面布局
- `home.html` - 首页布局

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

### 自定义配置

- `show_excerpts`: 显示文章摘要
- `show_post_meta`: 显示文章元信息
- `show_related_posts`: 显示相关文章
- `show_reading_time`: 显示阅读时间
- `show_social_share`: 显示社交分享

## 📊 部署

### GitHub Pages

项目使用GitHub Actions进行自动部署：

1. 推送代码到GitHub
2. GitHub Actions自动构建和部署
3. 部署到GitHub Pages

### GitHub Actions工作流

`.github/workflows/jekyll.yml` 包含：

- 自动构建Jekyll站点
- 部署到GitHub Pages
- 支持多平台构建（Windows/Linux）

### 自定义域名

1. 在 `_config.yml` 中设置 `url`
2. 在GitHub Pages设置中添加自定义域名
3. 创建 `CNAME` 文件

## 🐛 故障排除

### 常见问题

1. **平台兼容性问题**
   ```bash
   bundle lock --add-platform x86_64-linux
   ```

2. **依赖安装问题**
   ```bash
   bundle install --path vendor/bundle
   ```

3. **构建错误**
   ```bash
   bundle exec jekyll clean
   bundle exec jekyll build
   ```

### 调试技巧

- 使用 `--verbose` 参数查看详细错误信息
- 检查 `_site` 目录的生成内容
- 查看浏览器开发者工具的网络和控制台

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
- [GitHub Pages](https://pages.github.com/) - 免费托管服务
- [GitHub Actions](https://github.com/features/actions) - 自动化部署

## 📈 更新日志

### v2.0.0 (2024-06-23)
- ✨ 添加自定义布局文件
- 🎨 实现响应式设计
- 🚀 集成GitHub Actions自动部署
- 📱 优化移动端体验
- 🔧 修复GitHub Pages兼容性问题

### v1.0.0 (2024-06-23)
- 🎉 初始版本发布
- 📝 基础博客功能
- 📚 文章管理系统
- 🔍 SEO优化

---

⭐ 如果这个项目对你有帮助，请给它一个星标！