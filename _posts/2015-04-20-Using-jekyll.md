---
layout: post
title: jekyll vagrant not so perfectly
categories: [jekyll,vagrant]
tags: [jekyll,error]
description: here document
---

# 不能编辑css js
比较郁闷的问题
在vagrant中启动本地Jekyll
通过Windows上的sublime来编辑css的时候总是出错
不管输入什么都会在_site里面编译成NUL
发现
	1. 在window上别处编辑好之后再拷贝到jekyll目录就不会出现NUL
	2. 把Jekyll文件夹转移到非virtualbox共享目录，即linux文件系统上编辑不会出错
