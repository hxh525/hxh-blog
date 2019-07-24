---
author: Jaye Huang
categories: linux
tags: 
  - str-length 
  - shell
title: str-length command
date: 1999-01-01 00:00:00
img:
---

#### 字符串长度

```bash
$ str="123.?+ abc"
$ echo "$str" | wc -L
10
```

```bash
$ str="123.?+ abc"
$ echo "$str" | awk -F "" '{print NF}'
10
```

```bash
$ str="123.?+ abc"
$ echo  "$str"| awk '{print length($0)}'
10
```

```bash
$ str="123.?+ abc"
$ echo ${#str}
10
```

```bash
$ str="123.?+ abc"
$ expr "$str" : ".*"
10
```
