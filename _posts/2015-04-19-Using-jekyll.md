---
layout: post
title: Jekyll in vagrant
categories: [jekyll,vagrant]
tags: [polling]
description: jekyll vagrant polling fresh
---



### **不能编辑css js**

> 	在vagrant中启动本地Jekyll
	通过Windows上的sublime来编辑css的时候总是出错
	不管输入什么都会在_site里面编译成NUL

几番尝试后

- 在window上别处编辑好之后再拷贝到jekyll目录就不会出现NUL
- 把Jekyll文件夹转移到非virtualbox共享目录，即linux文件系统上编辑不会出错

>	对于一般的新建post没什么问题
	只是修改js，css的时候就麻烦一些

### **不能自动更新**
- 发现在Windows上编辑vagrant上的jekyll并不会自动生成，应该是没有通知到系统吧。而在vagrant内用你vim编辑是会自动生成新的网页的。

>	原来需要使用 `jekyll serve  --watch --force_polling`



