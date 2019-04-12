---
title: Mac command
author: Jay Yang
tags: command
categories:
  - computer
date: 1999-01-01 00:00:00
---

[Mac 键盘快捷键](https://support.apple.com/zh-cn/HT201236)
#### mac safeguard (外部源安装)

```bash
sudo spctl --master-disabl
```

#### mac command line shortcut

    option < 光标向前移动一个单词
    option b 光标向前移动一个单词

    option > 光标向后移动一个单词
    option f 光标向后移动一个单词

    ctrl a 将光标移至行首
    ctrl e 将光标移至行尾

    ctrl u 剪切命令行中光标所在处之前的所有字符（不包括自身）
    ctrl k 剪切命令行中光标所在处之后的所有字符（包括自身）
    ctrl w 删除你键入的最后一个单词

    ctrl v 插入特殊字符,如Ctrl+v+Tab加入Tab字符键

    ctrl (x u) 按住Ctrl的同时再先后按x和u，撤销刚才的操作

    ctrl+y 粘贴刚才所删除的字符

#### mac command

    uuidgen #生成uuid

#### mac command system

    last #命令行登录记录

    netstat #显示当前网络情况

    printenv #打印系统环境变量
    set KEY=VALUE #设置环境变量
    unuset KEY #删除环境变量

    uname -a #当前系统信息
    uname -r #当前系统内核版本
    sw_vers #当前 OSX 版本信息

    sysctl -a | grep -Eo "core_count:(.+?)$" # cpu核心数
    sysctl -n machdep.cpu.brand_string #cpu品牌

#### mac command domain

    whois HOST #查询域名的注册信息
    ping HOST #测试域名的连接延迟
    nslookup HOST #查询域名的 DNS 信息
    dig HOST #查询域名的 DNS 信息
    traceroute HOST #查询域名查找的路由信息
