---
layout: post
title: Here Document
categories: [linux,bash]
tags: [cat,bash]
description: here document
---


## Here Document 是什么

Here Document 是在Linux Shell 中的一种特殊的重定向方式，它的基本的形式如下

{% highlight bash %}
cat << delimiter
  Here Document Content
delimiter
{% endhighlight %}


{% highlight ruby %}
def he()
	puts 'hello world'
end
{% endhighlight %}



## Mannual

>  This  type of redirection instructs the shell to read input from the current source until a line containing only delimiter (with no trailing blanks) is
>   seen.  All of the lines read up to that point are then used as the standard input for a command.
>
>   The format of here-documents is:
>
>          <<[-]word
>                  here-document
>          delimiter
>
>   No parameter and variable expansion, command substitution, arithmetic expansion, or pathname expansion is performed on word.  If any characters in word
>   are  quoted, the delimiter is the result of quote removal on word, and the lines in the here-document are not expanded.  If word is unquoted, all lines
>   of the here-document are subjected to parameter expansion, command substitution,  and  arithmetic  expansion,  the  character  sequence  \<newline>  is
>   ignored, and \ must be used to quote the characters \, $, and `.
>
>   If the redirection operator is <<-, then all leading tab characters are stripped from input lines and the line containing delimiter.  This allows here-
>   documents within shell scripts to be indented in a natural fashion.

参考:[linux shell 的here document 用法 (cat << EOF)](http://my.oschina.net/u/1032146/blog/146941)
