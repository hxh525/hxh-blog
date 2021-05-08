---
title: https配置
author: Jaye Huang
date: 1999-01-01 00:00:00
categories: hexo
tags:
  - hexo
  - https
---

#### blog 域名解析

<https://console.dnspod.cn/dns/jayehuang.com/record?source=cloud>

|          |          |          |                                 |      |     |     |                 |
| -------- | -------- | -------- | ------------------------------- | ---- | --- | --- | --------------- |
| 主机记录 | 记录类型 | 线路类型 | 记录值                          | 权重 | MX  | TTL | 最后操作时间    |
| @        | CNAME    | 默认     | hxh525.github.io.               | -    | -   | 600 | 2021/5/8 14:59  |
| res      | CNAME    | 默认     | res.jayehuang.com.qiniudns.com. | -    | -   | 600 | 2019/9/25 16:58 |
| www      | CNAME    | 默认     | jayehuang.com.                  | -    | -   | 600 | 2019/8/19 01:36 |

#### 腾讯云申请 ssl 证书

<https://console.cloud.tencent.com/ssl>

|                    |                   |                            |                     |          |          |        |      |
| ------------------ | ----------------- | -------------------------- | ------------------- | -------- | -------- | ------ | ---- |
| ID                 | 绑定域名          | 证书类型                   | 到期时间            | 所属项目 | 关联资源 | 状态   | 操作 |
| mUtGXGgm blog 图片 | res.jayehuang.com | TrustAsia TLS RSA CA(1 年) | 2022-05-08 07:59:59 | 默认项目 |          | 已签发 | 更多 |

#### 七牛云 cdn 服务申请域名加速

<https://portal.qiniu.com/cdn/domain>

#### 七牛云 实时消费明细

<https://portal.qiniu.com/financial/bills/estimated-consume>

#### 切换 https - http

<!--
##### 开启 https 步骤

打开 [blog 域名解析](#blog 域名解析) res 解析记录
关闭 [blog 域名解析](#blog 域名解析) \* 解析记录
启用 [七牛云 cdn 服务申请域名加速](#七牛云 cdn 服务申请域名加速) res.jayehuang.com
关闭 [七牛云 cdn 服务申请域名加速](#七牛云 cdn 服务申请域名加速) .jayehuang.com
HXH_BLOG 全局替换 `https://res -> http://test`

##### 关闭 https 步骤

关闭 [blog 域名解析](#blog 域名解析) res 解析记录
打开 [blog 域名解析](#blog 域名解析) \* 解析记录
停用 [七牛云 cdn 服务申请域名加速](#七牛云 cdn 服务申请域名加速) res.jayehuang.com
启用 [七牛云 cdn 服务申请域名加速](#七牛云 cdn 服务申请域名加速) .jayehuang.com
HXH_BLOG 全局替换 `http://test -> https://res` -->
