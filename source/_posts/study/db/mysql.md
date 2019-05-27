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

#### mysql create schema & create user

    create schema test default character set utf8 collate utf8_general_ci;
    create user 'test'@'%' identified by '123456';
    grant all privileges on test.* to test;
    flush  privileges;
