---
layout: post
title:  "Hello world for Jekyll"
date:   2020-09-08 +0800
categories: jekyll
---

## 前言

博客第一页，写点什么好呢？

在观摩社团大佬们搭建的 Pages 和社团中各种基于 Pages 提供的网页服务后，我终于开始试图搭建自己（以及小伙伴们）的博客了。搭建的初衷是为了更好的思想交流，毕竟每年才能聚一次，机会实在是难得。特开此博客，以便进行个人记录与思想交流。

由于本站预计是由小伙伴们共同发布文章，进行评论，所以其主题没有任何规定，可以涉及任何方面，也可以让站点内容多维化。

## 本站初步规划

1. 用户系统，用作作者区分，可能只是用 tag 实现一下

2. 标签系统

3. 评论系统

4. 讨论系统

## 功能试用

- jekyll 代码高亮

### Python

{% highlight python %}
def leet_replace(string: str, setting='sd'):  # single, digit replace
    result = ''
    for i in string.lower():
        result += choice(list(filter(
            lambda x: len(x) == 1 and x.isascii() and (47 < ord(x) < 58 or 96 < ord(x) < 123),
            alpha_replace[i])))
    return result
{% endhighlight %}

### Bash

{% highlight bash %}
sudo apt-get update
sudo apt upgrade
sudo apt autoremove
sudo apt autoclean
{% endhighlight %}

### nasm

{% highlight nasm %}
Dump of assembler code for function touch2:
  0x004017ec <+0>:     sub    rsp,0x8		# 第一方案修改eip之后跳转到这里
  0x004017f0 <+4>:     mov    edx,edi
  0x004017f2 <+6>:     mov    DWORD PTR [rip+0x202ce0],0x2    # 0x6044dc <vlevel>
  0x004017fc <+16>:    cmp    edi,DWORD PTR [rip+0x202ce2]    # 0x6044e4 <cookie>
  0x00401802 <+22>:    jne    0x401824 <touch2+56>
  0x00401804 <+24>:    mov    esi,0x4030e8 # 第二种方案修改上面的<vlevel>处的值后跳转到这里
  0x00401809 <+29>:    mov    edi,0x1
  0x0040180e <+34>:    mov    eax,0x0
  0x00401813 <+39>:    call   0x400df0 <__printf_chk@plt>
  0x00401818 <+44>:    mov    edi,0x2
  0x0040181d <+49>:    call   0x401c8d <validate>
{% endhighlight %}

- latex

$$\begin{array}{l}
  \nabla \cdot D = \rho_0\\
  \nabla \times E = - \frac{\partial B}{\partial t}\\
  \nabla \cdot B = 0\\
  \nabla \times H = j_0 + \frac{\partial D}{\partial t}
\end{array}$$
