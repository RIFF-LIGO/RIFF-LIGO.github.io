---
title: 音乐
date: 2025-11-01 16:47:41
aplayer: true
---

<!-- 简单示例 (id, server, type)  -->
{% meting "60198" "netease" "playlist" %}

<!-- 进阶示例 -->
{% meting "60198" "netease" "playlist" "autoplay" "mutex:false" "listmaxheight:340px" "preload:none" "theme:#ad7a86"%}

```text
{% aplayer 那些花儿 朴树 url [picture_url, narrow, autoplay, width:xxx, lrc:xxx] %}
```