---
author: Jay Yang
categories: linux
tags: 
    - apt-get 
    - shell
title: apt-get command
date: 2019-03-29 14:24:33
img:
---

#### apt-get

    apt-get [选项] 命令

##### 选项：

    -h 本帮助文件。
    -q 输出到日志 - 无进展指示
    -qq 不输出信息，错误除外
    -d 仅下载 - 不安装或解压归档文件
    -s 不实际安装。模拟执行命令
    -y 假定对所有的询问选是，不提示
    -f 尝试修正系统依赖损坏处
    -m 如果归档无法定位，尝试继续
    -u 同时显示更新软件包的列表
    -b 获取源码包后编译 -V 显示详细的版本号
    -c=? 阅读此配置文件
    -o=? 设置自定的配置选项，如 -o dir::cache=/tmp

##### 命令：

    update - 重新获取软件包列表
    upgrade - 进行更新
    install - 安装新的软件包
    remove - 移除软件包
    autoremove - 自动移除全部不使用的软件包
    purge - 移除软件包和配置文件
    source - 下载源码档案
    build-dep - 为源码包配置编译依赖
    dist-upgrade - 发行版升级
    dselect-upgrade - 依照 dselect 的选择更新
    clean - 清除下载的归档文件
    autoclean - 清除旧的的已下载的归档文件
    check - 检验是否有损坏的依赖

##### 常用示例

    apt-cache searchpackagename #搜索包
    apt-cache show packagename #获取包的相关信息，如说明、大小、版本等
    apt-get install packagename #安装包
    apt-get install packagename --reinstall #重新安装包
    apt-get -f install #修复安装”-f = –fix-missing”
    apt-get remove packagename #删除包
    apt-get remove packagename --purge #删除包，包括删除配置文件等
    apt-get update #更新源
    apt-get upgrade #更新已安装的包
    apt-get dist-upgrade #升级系统
    apt-get dselect-upgrade #使用 dselect 升级
    apt-cache depends packagename #了解使用依赖
    apt-cache rdepends packagename #是查看该包被哪些包依赖
    apt-get build-dep packagename #安装相关的编译环境
    apt-get source packagename #下载该包的源代码
    apt-get clean apt-get autoclean #清理无用的包
    apt-get check #检查是否有损坏的依赖
