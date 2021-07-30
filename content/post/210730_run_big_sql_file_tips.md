---
title: "MySQL 执行大 sql 文件的命令行快速解决方案"
date: 2021-07-30T10:43:16+08:00
lastmod: 2021-07-30T10:43:16+08:00
draft: false
keywords: ["mysql", "tips"]
description: "run big sql file tips"
tags: ["mysql", "tips"]
categories: ["mysql", "tips"]
author: "LeoWang"

toc: false
autoCollapseToc: false
# contentCopyright: false
reward: false
mathjax: false
---

## MySQL 执行大 sql 文件的命令行快速解决方案

<!--more-->

今天有一个 3w 行记录的 sql 文件
直接执行 sql 语句会很慢，电脑直接卡爆 3 次
遂另寻解决方案，现记录如下


```bash
mysql -u (username) -p -D(database name) < (sql file path)
mysql -u (用户名) -p -D(数据库名) < (sql 文件路径)

案例：
mysql -u root -p -Dpear-admin-pro < ./pear-admin-pro.sql
```


### 执行时间

3 万行 sql （文件大小：4.9M）语句执行时间不到 5 秒
