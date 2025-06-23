---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: "欢迎来到 Exxfire's Blog"
subtitle: "分享技术，记录生活"
---

# 👋 欢迎来到我的博客

你好！我是 **Exxfire**，一名热爱技术的程序员。这里是我分享技术心得、学习笔记和生活感悟的地方。

## 🚀 最新文章

{% for post in site.posts limit:5 %}
### [{{ post.title }}]({{ post.url }})
**{{ post.date | date: "%Y年%m月%d日" }}** | {{ post.categories | join: ', ' }}

{{ post.excerpt | strip_html | truncate: 80 }}

[阅读全文 →]({{ post.url }})

---
{% endfor %}

## 📚 文章分类

- **技术分享** - 编程技巧、开发经验
- **学习笔记** - 新技术学习心得
- **项目展示** - 个人项目介绍
- **生活随笔** - 日常感悟和思考

## 🛠️ 技术栈



<!-- - **前端**: HTML5, CSS3, JavaScript, React, Vue.js
- **后端**: Node.js, Python, Java, Go
- **数据库**: MySQL, MongoDB, Redis
- **云服务**: AWS, Azure, 阿里云
- **工具**: Git, Docker, Kubernetes -->

## 📫 联系我

- 📧 Email: [1009524027@qq.com](mailto:1009524027@qq.com)
- 💻 GitHub: [@Exxfire](https://github.com/Exxfire)
- 🔗 博客: [https://exxfire.github.io](https://exxfire.github.io)

<!-- ## 📡 订阅更新

想要及时获取最新文章？可以通过以下方式订阅：

- [RSS订阅](/feed.xml)
- [邮件订阅](mailto:1009524027@qq.com?subject=订阅博客更新) -->

---

*感谢你的访问！如果觉得内容有帮助，欢迎分享给更多的朋友。*
