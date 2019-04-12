---
author: Jay Yang
categories: db
tags: mysql
title: mysql
date: 1999-01-01 00:00:00
img:
---

#### mysql 5.7 update paasword

    update user set authentication_string=password('123') where user='root'
