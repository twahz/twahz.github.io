# Personal Blog Customization Guide

This is a comprehensive guide to help you customize this Jekyll + Chirpy theme blog into your own personal blog.

## Essential Files to Modify

### 1. `_config.yml` - Core Site Configuration ⭐⭐⭐

This is the most important configuration file containing all basic information about your blog.

**Key sections to modify:**

```yaml
# Line 17: Blog title
title: XK Blog  # Change to your blog name

# Line 19: Tagline/Motto
tagline: 天行健，君子以自强不息；地势坤，君子以厚德载物！  # Change to your motto or tagline

# Lines 21-23: Site description (for SEO)
description: >-
  分享关于数学、编程与科研的思考与记录。  # Change to a brief description of your blog

# Line 27: Site URL
url: "https://twahz.github.io"  # Change to your GitHub Pages URL, e.g., https://yourusername.github.io

# Line 30: GitHub username
github:
  username: twahz  # Change to your GitHub username

# Line 33: Twitter/X username (optional)
twitter:
  username: GraphsGuru  # Change to your Twitter username or remove this section

# Lines 38-46: Social information
social:
  name: Xingkun Song  # Change to your real name or nickname
  email: sxkmath@outlook.com  # Change to your email address
  links:
    - https://x.com/GraphsGuru  # Change to your Twitter profile
    - https://github.com/twahz  # Change to your GitHub profile
    # Uncomment and add more social links as needed

# Line 102: Avatar setting
avatar:  # Add your avatar image path, e.g., /assets/img/avatar.jpg

# Line 9: Language setting
lang: zh-CN  # Change to 'en' for English blog

# Line 12: Timezone
timezone: Asia/Shanghai  # Change to your timezone
```

**Optional advanced configurations:**

- **Lines 49-55: Webmaster verifications** (for Google, Bing, etc.)
- **Lines 61-75: Web analytics** (Google Analytics, GoatCounter, etc.)
- **Lines 111-131: Comment system** (Disqus, Utterances, Giscus)

### 2. `_data/contact.yml` - Contact Information ⭐⭐

Defines social media icons and links displayed at the bottom of the sidebar.

**Sections to modify:**

```yaml
# Line 5: GitHub link
- type: github
  icon: "fab fa-github"
  url: "https://github.com/twahz"  # Change to your GitHub profile

# Line 9: Twitter/X link
- type: x
  icon: "fa-brands fa-x-twitter"
  url: "https://x.com/GraphsGuru"  # Change to your Twitter profile or remove

# Line 13: Email
- type: email
  icon: "fas fa-envelope"
  url: "mailto:sxkmath@outlook.com"  # Change to your email address
```

**Optional contact methods:**
- Uncomment lines 23-45 to add Mastodon, LinkedIn, Stack Overflow, Bluesky, Reddit, Threads, etc.

### 3. `_tabs/about.md` - About Page ⭐⭐

This is your "About Me" page where visitors can learn about you.

**Content to modify:**

```markdown
# Line 6: Page description
description: "你好，我是 XK"  # Change to your brief self-introduction

# Lines 9-22: Entire about page content
你好，我是 **XK**，青椒一枚。

这个站点由 [GitHub Pages](https://pages.github.com/) 和 [Jekyll](https://jekyllrb.com/) 搭建...

# Replace entirely with your own personal introduction, background, interests, etc.
```

### 4. `_posts/` Directory - Blog Posts ⭐⭐⭐

This is where you place all your blog posts.

**Steps to create a new post:**

1. Create a new file in the `_posts/` directory
2. File naming format: `YYYY-MM-DD-title.md`
   - Example: `2024-11-03-my-first-post.md`

3. Posts must start with YAML Front Matter:

```markdown
---
title: Your Post Title
date: 2024-11-03 10:00:00 +0800
categories: [Category1, Category2]
tags: [tag1, tag2, tag3]
---

Start writing your post content here...
```

**Example post:**

```markdown
---
title: My First Blog Post
date: 2024-11-03 14:30:00 +0800
categories: [Life, Journal]
tags: [beginning, personal-blog]
---

# Welcome to My Blog

This is my first blog post...
```

## Optional Files to Modify

### 5. Avatar Image

**Step 1: Create the img directory**

If the `assets/img/` directory doesn't exist, create it first:

```bash
mkdir -p assets/img
```

**Step 2: Add your avatar image**

Copy your avatar image file to the `assets/img/` directory.

**Step 3: Configure in settings**

Then configure the avatar path in `_config.yml`:

```yaml
avatar: /assets/img/your-avatar-filename.jpg
```

Recommended size: 512x512 pixels or larger, square format

### 6. Site Favicon

Replace icon files in the `assets/img/favicons/` directory (if it exists)

### 7. Other Tab Pages

Other files in the `_tabs/` directory:
- `archives.md` - Archives page (usually no modification needed)
- `categories.md` - Categories page (usually no modification needed)
- `tags.md` - Tags page (usually no modification needed)

These files typically work fine with defaults unless you want to customize page titles or descriptions.

## Modification Priority Summary

### 🔴 Must Modify Immediately (or will show someone else's information)

1. Personal information in `_config.yml` (name, email, username, URL)
2. Contact links in `_data/contact.yml`
3. Personal introduction in `_tabs/about.md`

### 🟡 Recommended to Modify Soon

4. Add your own avatar image
5. Modify title, tagline, and description in `_config.yml`
6. Start creating your own posts in `_posts/`

### 🟢 Optional Modifications

7. Configure comment system (if needed)
8. Configure web analytics (if needed)
9. Add more social media links
10. Customize site favicon

## Preview Blog Locally

After making modifications, you can preview your blog locally:

```bash
# Install dependencies
bundle install

# Start local server
bundle exec jekyll serve

# Then visit http://127.0.0.1:4000 in your browser
```

## Deploy to GitHub Pages

1. Commit all modifications to your GitHub repository
2. GitHub Actions will automatically build and deploy
3. Wait a few minutes, then visit `https://yourusername.github.io`

## Important Notes

⚠️ **Important Reminders:**

1. **Do NOT delete** the `.nojekyll` file
2. **Do NOT modify** files like `_plugins/`, `index.html` (unless you know what you're doing)
3. **Follow naming conventions**: Blog posts must use `YYYY-MM-DD-title.md` format
4. **Check before committing**: Ensure `_config.yml` syntax is correct (YAML is indentation-sensitive)
5. **Image paths**: Use relative paths or absolute paths starting with `/`

## Getting Help

- Chirpy Theme Documentation: https://github.com/cotes2020/jekyll-theme-chirpy/wiki
- Jekyll Official Documentation: https://jekyllrb.com/docs/
- Submit Issues: https://github.com/twahz/twahz.github.io/issues

---

Last Updated: 2024-11-03
