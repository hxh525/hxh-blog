---
title: Linux command
author: Jay Yang
tags: command
categories:
  - computer
date: 2099-12-31 23:59:59
---

#### cpu 信息
    #查看物理 CPU 个数
    cat /proc/cpuinfo | grep "physical id" | sort | uniq | wc -l

    #查看每个物理 CPU 中 core 的个数(即核数)`
    cat /proc/cpuinfo | grep "cpu cores" | uniq

    #查看逻辑 CPU 的个数`
    cat /proc/cpuinfo | grep "processor" | wc -l
