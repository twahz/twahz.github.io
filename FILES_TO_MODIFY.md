# 需要修改的文件清单 / Files to Modify Checklist

本文档提供了创建个人博客时需要修改的所有文件的快速概览。  
This document provides a quick overview of all files that need to be modified when creating your personal blog.

---

## 📋 文件修改清单 / File Modification Checklist

### 🔴 必须修改的文件 / Must Modify Files

#### 1. `_config.yml` 
**重要程度 / Priority:** ⭐⭐⭐ 最高 / Highest

**需要修改的内容 / What to modify:**
- 第 17 行：`title:` - 博客标题 / Blog title
- 第 19 行：`tagline:` - 副标题 / Tagline
- 第 21 行：`description:` - 网站描述 / Site description
- 第 27 行：`url:` - 网站地址 / Site URL
- 第 30 行：`github.username:` - GitHub 用户名 / GitHub username
- 第 33 行：`twitter.username:` - Twitter 用户名（可选）/ Twitter username (optional)
- 第 38 行：`social.name:` - 你的姓名 / Your name
- 第 39 行：`social.email:` - 你的邮箱 / Your email
- 第 40-43 行：`social.links:` - 社交媒体链接 / Social media links
- 第 102 行：`avatar:` - 头像路径 / Avatar path

**为什么重要 / Why important:**  
这个文件包含了博客的所有核心配置信息，是整个网站的"大脑"。如果不修改，网站会显示原作者的信息。  
This file contains all core configuration of the blog. It's the "brain" of the website. Without modification, it will show the original author's information.

---

#### 2. `_data/contact.yml`
**重要程度 / Priority:** ⭐⭐ 高 / High

**需要修改的内容 / What to modify:**
- 第 5 行：GitHub 链接 / GitHub link
- 第 9 行：Twitter/X 链接 / Twitter/X link
- 第 13 行：邮箱地址 / Email address
- 第 22-45 行：其他社交媒体链接（可选）/ Other social links (optional)

**为什么重要 / Why important:**  
控制侧边栏底部显示的联系方式图标。  
Controls contact icons displayed at the bottom of the sidebar.

---

#### 3. `_tabs/about.md`
**重要程度 / Priority:** ⭐⭐ 高 / High

**需要修改的内容 / What to modify:**
- 第 6 行：`description:` - 页面描述 / Page description
- 第 9-22 行：整个关于页面的内容 / Entire about page content

**为什么重要 / Why important:**  
这是访客了解你的主要页面，应该包含你的个人介绍、背景、兴趣等。  
This is the main page where visitors learn about you. Should contain your introduction, background, interests, etc.

---

### 🟡 建议修改的文件 / Recommended to Modify Files

#### 4. `_posts/` 目录 / Directory
**重要程度 / Priority:** ⭐⭐⭐ 最高 / Highest

**需要做什么 / What to do:**
- 创建新文件：`YYYY-MM-DD-标题.md` / Create new files: `YYYY-MM-DD-title.md`
- 每个文件开头需要包含 YAML Front Matter / Each file must start with YAML Front Matter

**文章模板 / Post template:**
```markdown
---
title: 文章标题 / Post Title
date: 2024-11-03 14:30:00 +0800
categories: [分类1, 分类2] / [Category1, Category2]
tags: [标签1, 标签2] / [tag1, tag2]
---

文章内容... / Post content...
```

**为什么重要 / Why important:**  
这是博客的核心内容！没有文章的博客就不是真正的博客。  
This is the core content of your blog! A blog without posts is not really a blog.

---

#### 5. `assets/img/` 目录 / Directory
**重要程度 / Priority:** ⭐⭐ 高 / High

**需要做什么 / What to do:**
- 如果目录不存在，先创建：`mkdir -p assets/img` / If directory doesn't exist, create it first: `mkdir -p assets/img`
- 添加你的头像图片 / Add your avatar image
- 建议尺寸：512x512 像素或更大，正方形 / Recommended size: 512x512px or larger, square
- 在 `_config.yml` 中配置路径 / Configure path in `_config.yml`

**为什么重要 / Why important:**  
头像让你的博客更具个性化和专业感。  
An avatar makes your blog more personalized and professional.

---

### 🟢 可选修改的文件 / Optional Files to Modify

#### 6. `assets/img/favicons/` 目录（如果存在）
**重要程度 / Priority:** ⭐ 低 / Low

**需要做什么 / What to do:**
- 替换网站图标文件 / Replace favicon files

**为什么重要 / Why important:**  
自定义网站图标让博客在浏览器标签页中更易识别。  
Custom favicon makes your blog more recognizable in browser tabs.

---

#### 7. 其他标签页 / Other Tab Pages
- `_tabs/archives.md` - 归档页 / Archives page
- `_tabs/categories.md` - 分类页 / Categories page  
- `_tabs/tags.md` - 标签页 / Tags page

**重要程度 / Priority:** ⭐ 低 / Low

**需要做什么 / What to do:**
- 通常保持默认即可 / Usually keep defaults
- 可选：修改页面标题或描述 / Optional: modify page title or description

---

## 📊 修改优先级总结 / Priority Summary

### 🔴 立即修改（第一优先级）/ Immediate (First Priority)
1. `_config.yml` - 个人信息部分 / Personal information section
2. `_data/contact.yml` - 联系方式 / Contact information
3. `_tabs/about.md` - 关于页面 / About page

### 🟡 尽快修改（第二优先级）/ Soon (Second Priority)
4. 添加头像图片 / Add avatar image
5. 创建第一篇博客文章 / Create first blog post
6. 修改博客标题和描述 / Modify blog title and description

### 🟢 可选修改（第三优先级）/ Optional (Third Priority)
7. 配置评论系统 / Configure comment system
8. 配置网站分析 / Configure web analytics
9. 自定义网站图标 / Customize favicon
10. 添加更多社交媒体链接 / Add more social links

---

## 🚫 不要修改的文件 / Files NOT to Modify

❌ **请勿修改以下文件（除非你知道自己在做什么）:**  
❌ **Do NOT modify the following files (unless you know what you're doing):**

- `.nojekyll` - 告诉 GitHub Pages 不要使用 Jekyll / Tells GitHub Pages not to use Jekyll
- `index.html` - 博客首页模板 / Blog homepage template
- `_plugins/` 目录 - Jekyll 插件 / Jekyll plugins
- `Gemfile` - Ruby 依赖配置 / Ruby dependencies
- `.github/` 目录 - GitHub Actions 配置 / GitHub Actions configuration

---

## 📚 更多详细信息 / More Detailed Information

查看完整指南 / See complete guides:
- [个人博客定制指南.md](个人博客定制指南.md) - 详细中文指南 / Detailed Chinese guide
- [CUSTOMIZATION_GUIDE.md](CUSTOMIZATION_GUIDE.md) - Comprehensive English guide
- [QUICK_START_CHECKLIST.md](QUICK_START_CHECKLIST.md) - 快速检查清单 / Quick checklist

---

## ✅ 验证清单 / Verification Checklist

在提交修改之前，请确认 / Before committing, please verify:

- [ ] 所有个人信息已更新 / All personal information updated
- [ ] 邮箱、用户名、链接都是正确的 / Email, username, links are correct
- [ ] 至少创建了一篇博客文章 / At least one blog post created
- [ ] 添加了头像图片 / Avatar image added
- [ ] 本地预览正常 / Local preview works correctly
- [ ] `_config.yml` 语法正确（YAML 对缩进敏感）/ `_config.yml` syntax is correct (YAML is indentation-sensitive)

---

最后更新 / Last Updated: 2024-11-03
