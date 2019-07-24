---
author: Jaye Huang
categories: gitlab
tags: gitlab
title: gitlab command
date: 1999-01-01 00:00:00
img:
---

#### Gitlab

##### Install

[https://about.gitlab.com/install/](https://about.gitlab.com/install/)

##### Gitlab 默认路径

    #配置路径
    /etc/gitlab/gitlab.rb
    #备份路径
    /var/opt/gitlab/backups

##### Gitlab 数据备份

    sudo gitlab-rake gitlab:backup:create

##### Gitlab 数据恢复

    sudo  ./gitlab-ctl stop unicorn
    sudo  ./gitlab-ctl stop sidekiq
    sudo  ./gitlab-rake gitlab:backup:restore BACKUP='备份的identity'
    sudo  ./gitlab-ctl start

##### 安装完 gitlab 后的运维操作

    sudo gitlab-ctl status
    sudo gitlab-ctl reconfigure
    sudo gitlab-ctl start
    sudo gitlab-ctl stop
    sudo gitlab-ctl restart
    sudo gitlab-ctl tail

##### 检查 redis 的日志

    sudo gitlab-ctl tail redis

##### 检查 postgresql 的日志

    sudo gitlab-ctl tail postgresql

##### 检查 gitlab-workhorse 的日志

    sudo gitlab-ctl tail gitlab-workhorse

##### 检查 logrotate 的日志

    sudo gitlab-ctl tail logrotate

##### 检查 nginx 的日志

    sudo gitlab-ctl tail nginx

##### 检查 sidekiq 的日志

    sudo gitlab-ctl tail sidekiq

##### 检查 unicorn 的日志

    sudo gitlab-ctl tail unicorn

##### Gitlab 修改 root 用户密码

    sudo gitlab-rails console production

    user = User.where(id: 1).first
    user.password = ‘新密码‘
    user.password_confirmation = ‘新密码‘
    user.save!

##### gitlab setting

    Guest：可以创建issue、发表评论，不能读写版本库
    Reporter：可以克隆代码，不能提交，QA、PM可以赋予这个权限
    Developer：可以克隆代码、开发、提交、push，RD可以赋予这个权限
    Master：可以创建项目、添加tag、保护分支、添加项目成员、编辑项目，核心RD负责人可以赋予这个权限
    Owner：可以设置项目访问权限 - Visibility Level、删除项目、迁移项目、管理组成员，开发组leader可以赋予这个权限

    Private：只有组成员才能看到
    Internal：只要登录的用户就能看到
    Public：所有人都能看到

> ps:开源项目和组设置的是 Internal
