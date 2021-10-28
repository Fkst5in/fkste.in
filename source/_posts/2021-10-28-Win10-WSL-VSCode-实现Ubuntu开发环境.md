---
title: "Win10 +  WSL + VSCode 实现Ubuntu开发环境 "
categories:
  - [开发环境, WSL]
index_img: "/img/post/2021-10-28-Win10-WSL-VSCode-实现Ubuntu开发环境-index.jpg"
abbrlink: 19918
date: 2019-11-24 12:08:18
tags:
  - [WSL]
  - [Linux]
  - [Ubuntu]
banner_img: "/img/post/2021-10-28-Win10-WSL-VSCode-实现Ubuntu开发环境-banner.jpg"
---

> WSL（Windows Subsystem for Linux）是微软在 windows10 1607 之后推出的功能，让开发者可以十分方便地在 windows 环境下开发、编译 linux 程序

<!-- more -->

### 1.安装 WSL

> 可以参考[官方教程](https://docs.microsoft.com/en-us/windows/wsl/install-win10)

- 打开*启用或关闭 windows 功能*

{% asset_img features.jpg windows功能 %}

勾选 _适用于 linux 的 windows 子系统_

- 下载 Ubuntu

打开 windows 商店，搜索 ubuntu，然后下载即可

### 2.配置 VScode

- 安装 VScode

[下载连接](https://code.visualstudio.com/)，下载安装即可

- 安装 _Remote - WSL_ 插件

{% asset_img remote.jpg 插件 %}

搜索并安装插件即可

### 3.使用

安装完成后，便可以通过在 cmd 或 powershell 中使用

```
& ubuntu
```

打开 ubuntu 的终端，然后在任意目录下输入

```
$ code .
```

便可以在 VScode 内打开此目录，效果如图
{% asset_img sl.jpg sl %}

### 注

ubuntu 的根目录在 C 盘下，不过不建议直接访问

```
C:\Users\你的用户名\AppData\Local\Packages\CanonicalGroupLimited.UbuntuonWindows_79rhkp1fndgsc\LocalState\rootfs
```
