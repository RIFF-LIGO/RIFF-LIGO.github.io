---
title: acm式输入输出
date: 2025-11-03 15:32:29
updated:
tags:
categories:
keywords:
description:
top_img:
comments:
cover:
toc:
toc_number:
toc_style_simple:
copyright:
copyright_author:
copyright_author_href:
copyright_url:
copyright_info:
mathjax:
katex:
aplayer:
highlight_shrink:
aside:
abcjs:
noticeOutdate:
---



# nodejs实现acm模式输入输出
模板一：
```JS
const rl = require('readline').createInterface({input:process.stdin})
const iter = rl[Symbol.asyncIterator]()
const readline = (await iter.next()).value
```


模板二：
```js

const rl = require('readline').createInterface({input:process.stdin})
rl.on('line',(line)=>{

})
```
