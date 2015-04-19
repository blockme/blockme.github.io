---
layout: post
title: Update brightness on ubuntu
categories:
tags:
description: update brightness on ubuntu
---

Acer 笔记本安装ubuntu后，若不能调整亮度

{% highlight bash %}
sudo sed -i 's/GRUB_CMDLINE_LINUX=""/GRUB_CMDLINE_LINUX="acpi_osi=Linux acpi_backlight=video"/' /etc/default/grub
sudo sed -i '$i echo 50 >/sys/class/backlight/intel_backlight/brightness' /etc/rc.local
sudo update-grub
{% endhighlight %}
