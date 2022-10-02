---
title: "Reinstall Macos"
date: 2022-09-30T00:44:30+08:00
lastmod: 2022-09-30T00:44:30+08:00
draft: true
keywords: []
description: ""
tags: []
categories: []
author: "LeoWang"

toc: false
autoCollapseToc: false
# contentCopyright: false
reward: false
mathjax: false
---

## 起因

我的 MacOS 磁盘空间不够用了，已经删除过一些东西了，仍然只有 20 GB 左右的磁盘空间可用；并且磁盘中还有很多大量的不必要的文件，
如：
- 开发过程中的 `node_modules`（没有及时清理）
- `docker` 产生的镜像包和
- 虚拟机（文件、镜像）
- 许多冗余的软件

<!--more-->

## 前置操作

- 备份安装软件列表
	- `/Library`
	- `~/Library`
	- `brew list`
	- `npm list --global`
- 确定需要安装的软件和安装方式
- 确定需求
  > 可以，但没必要
  - 不需要 `docker`  
    `Arm` 平台的 `docker` 使用效果有点不尽人意，主要原因还是因为开发者对 `Arm` 平台的适配不够所导致，遂弃用，改为在个人服务器上使用
  - 不需要虚拟机  
    同样，和弃用 `docker` 的原因一致，`Arm` 平台跑虚拟机的效果也还是不尽人意，虽然有 [UTM](#)、[QMENU](#) 这类软件去适配 `Arm` 平台。


## 开始

