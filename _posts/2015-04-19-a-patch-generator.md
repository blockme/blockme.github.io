---
layout: post
title: A patch generator
categories: [linux,bash]
tags: [utils,bash]
description: here document
---

- 在开发webapps时，不可避免的需要添加某个功能或者是修改bug。而这些改动又需要向前方提交增量补丁。
	对Java而言，就是一些class之类的。这样手动拣选这些藏匿于不同目录而层次又很深的目录中比较费时间。
	曾经就因为不小心漏了一个icon而受到责备。于是写了个小脚本。方便提取补丁。

- 脚本在[这里](https://github.com/blockme/notes/blob/master/utils/x.sh)

- 在项目改动之前先执行 `x.sh i /path/to/webapp`
- 修改完成了后执行 `x.sh g`
- 到当前目录下temp找个pather及好了

如果在windows中，可以使用vagrant。把发布路径改到共享文件夹就好了


