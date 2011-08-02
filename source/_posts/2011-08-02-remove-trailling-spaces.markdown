---
layout: post
title: "Vim: удаление trailing spaces"
date: 2011-08-02 15:31
comments: true
categories: vim
---

Для удаления trailing spaces можно воспользоваться такой командой:

```
    :%s/\s*$//g
```

Так же удобно повесить ее на горячу клавишу:

``` vim
    map <silent> <Leader>ts :%s/\s*$//g<CR>
```
