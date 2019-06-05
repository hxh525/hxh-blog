---
author: Jay Yang
categories: db
tags: mysql
title: mysql
date: 1999-01-01 00:00:00
img:
---

#### mac mysql 5.7 no paasword login

    mysql.server start
    mysql.server restart

    mysql.server stop
    mysqld_safe --skip-grant-tables
    mysql -uroot

#### mysql commond

    show databases;
    show tables;
    flush privileges;

#### mysql 5.7 update paasword & host

    update mysql.user set authentication_string=password('123456') where user='root'
    update mysql.user set host='%' where user='root'

#### mysql create schema & create user

    create schema test default character set utf8 collate utf8_general_ci;
    create user 'test'@'%' identified by '123456';
    grant all privileges on test.* to test;
    flush  privileges;
