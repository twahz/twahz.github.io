# 博客定制快速检查清单 / Quick Start Checklist

## 🔴 必须修改 / Must Modify

- [ ] **_config.yml**
  - [ ] `title:` 博客标题
  - [ ] `tagline:` 副标题/座右铭
  - [ ] `description:` 网站描述
  - [ ] `url:` 你的 GitHub Pages 地址
  - [ ] `github.username:` 你的 GitHub 用户名
  - [ ] `social.name:` 你的姓名
  - [ ] `social.email:` 你的邮箱
  - [ ] `social.links:` 你的社交媒体链接

- [ ] **_data/contact.yml**
  - [ ] GitHub 链接
  - [ ] Email 地址
  - [ ] Twitter/X 链接（如有）
  - [ ] 其他社交媒体链接（可选）

- [ ] **_tabs/about.md**
  - [ ] 修改个人介绍内容
  - [ ] 更新联系方式

## 🟡 建议修改 / Recommended

- [ ] 创建 img 目录：`mkdir -p assets/img` (如不存在)
- [ ] 添加头像图片到 `assets/img/`
- [ ] 在 `_config.yml` 中设置 `avatar:` 路径
- [ ] 创建第一篇博客文章在 `_posts/`
- [ ] 检查语言设置 `lang:` (zh-CN 或 en)
- [ ] 检查时区设置 `timezone:`

## 🟢 可选配置 / Optional

- [ ] 配置评论系统（Disqus/Utterances/Giscus）
- [ ] 配置网站分析（Google Analytics 等）
- [ ] 添加网站图标 (favicon)
- [ ] 配置搜索引擎验证码
- [ ] 添加更多社交媒体链接

## 📝 创建第一篇文章 / Create First Post

在 `_posts/` 目录创建文件: `YYYY-MM-DD-your-title.md`

```markdown
---
title: 文章标题
date: 2024-11-03 14:30:00 +0800
categories: [分类1, 分类2]
tags: [标签1, 标签2]
---

文章内容...
```

## 🚀 本地测试 / Local Testing

```bash
bundle install
bundle exec jekyll serve
# 访问 http://127.0.0.1:4000
```

## ✅ 部署检查 / Deployment Check

- [ ] 所有个人信息已更新
- [ ] 本地预览正常
- [ ] 提交所有修改到 GitHub
- [ ] GitHub Actions 构建成功
- [ ] 访问网站确认显示正确

---

完成以上步骤后，你的个人博客就配置完成了！🎉
After completing the above steps, your personal blog is ready! 🎉
