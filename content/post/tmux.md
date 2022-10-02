---
title: "Tmux 使用手册"
date: 2021-03-16T01:09:00+08:00
lastmod: 2021-04-17T01:09:00+08:00
draft: false
keywords: ["Tmxu"]
description: ""
tags: ["Tmux", "技术向"]
categories: ["技术向"]
author: "LeoWang"

comment: true
toc: false
autoCollapseToc: false
reward: false
mathjax: false
---

## 0x00

tmux 基础操作与快捷键

<!--more-->

# tmux 使用手册

> [Tmux 使用教程](https://www.ruanyifeng.com/blog/2019/10/tmux.html)


## command

`tmux ls `
`tmux list-sessions`   - 查看当前所有的 Tmux 会话。

`tmux attach-session` - 重新接入会话


## 窗格操作

Ctrl+b
- d: 退出
- %：划分左右两个窗格。
- "：划分上下两个窗格。
- <arrow key>：光标切换到其他窗格。<arrow key>是指向要切换到的窗格的方向键，比如切换到下方窗格，就按方向键↓。
- ;：光标切换到上一个窗格。
- o：光标切换到下一个窗格。
- {：当前窗格与上一个窗格交换位置。
- }：当前窗格与下一个窗格交换位置。
- Ctrl+o：所有窗格向前移动一个位置，第一个窗格变成最后一个窗格。
- Alt+o：所有窗格向后移动一个位置，最后一个窗格变成第一个窗格。
- x：关闭当前窗格。
- !：将当前窗格拆分为一个独立窗口。
- z：当前窗格全屏显示，再使用一次会变回原来大小。
- Ctrl+<arrow key>：按箭头方向调整窗格大小。
- q：显示窗格编号。


## 窗口快捷键

Ctrl+b
- c：创建一个新窗口，状态栏会显示多个窗口的信息。
- p：切换到上一个窗口（按照状态栏上的顺序）。
- n：切换到下一个窗口。
- <number>：切换到指定编号的窗口，其中的<number>是状态栏上的窗口编号。
- w：从列表中选择窗口。
- ,：窗口重命名。
