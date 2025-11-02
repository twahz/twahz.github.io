---
layout: page
icon: fas fa-info-circle
order: 4
title: "About"
description: "你好，我是 XK"
header-img: "img/post-bg-rwd.jpg"
---

你好，我是 **XK**，青椒一枚。

这个站点由 [GitHub Pages](https://pages.github.com/) 和 [Jekyll](https://jekyllrb.com/) 搭建，用来记录与分享我在学习与工作中的所思所想，沉淀可复用的知识和工具。

- GitHub 主页：[twahz](https://github.com/twahz)
- 博客源码：[twahz/twahz.github.io](https://github.com/twahz/twahz.github.io)

## 联系方式
- 通过评论区直接留言（见页面底部）
- 或在仓库提 Issue：[@twahz/twahz.github.io/issues](https://github.com/twahz/twahz.github.io/issues)

## Talks
整理中……

最后更新：{{ site.time | date: '%Y-%m-%d' }}

<!-- Gitalk 评论 start -->
{% if site.gitalk.enable %}
<link rel="stylesheet" href="https://unpkg.com/gitalk/dist/gitalk.css">
<script src="https://unpkg.com/gitalk@latest/dist/gitalk.min.js"></script>

<div id="gitalk-container"></div>
<script type="text/javascript">
  var gitalk = new Gitalk({
    clientID: '{{site.gitalk.clientID}}',
    clientSecret: '{{site.gitalk.clientSecret}}',
    repo: '{{site.gitalk.repo}}',
    owner: '{{site.gitalk.owner}}',
    admin: ['{{site.gitalk.admin}}'],
    distractionFreeMode: {{site.gitalk.distractionFreeMode}},
    id: 'about',
  });
  gitalk.render('gitalk-container');
</script>
{% endif %}
<!-- Gitalk end -->

<!-- disqus 评论框 start -->
{% if site.disqus.enable %}
<div class="comment">
  <div id="disqus_thread" class="disqus-thread"></div>
</div>

<script type="text/javascript">
  var disqus_shortname = "{{site.disqus.username}}";
  var disqus_identifier = "{{site.disqus.username}}/{{page.url}}";
  var disqus_url = "{{site.url}}{{page.url}}";

  (function() {
    var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
    dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js';
    (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
  })();
</script>
{% endif %}
<!-- disqus 评论框 end -->
