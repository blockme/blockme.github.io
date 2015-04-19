---
layout: post
title: Emulate rename on windows
categories:
tags:
description: Emulate rename on windows
---

#改名小脚本

一个迷你的改名小脚本

在windows上有时候需要批量修改文件名，可以装bulk

但是，那个还不如敲个命令快呢

- [脚本在这](https://github.com/blockme/notes/blob/master/utils/rename.sh)

- 依赖 **git-bash**

##使用
- 在windows上安装git-bash之后就可以使用了，把该脚本放在`%path%`中
{% highlight bash %}
rename 's/\.txt$//'  *		# 消除后缀
rename 's/\(\.txt\)\+$//' *	# 消除后缀
rename 's/$/\.txt/' *		# 增加后缀
find -iname '*[!.]???' -type f -exec rename 's/$/\.txt/' '{}' \; #增加后缀
{% endhighlight %}

