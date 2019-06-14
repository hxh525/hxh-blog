# 命令

## 启动命令

hexo clean && hexo server -p 525

## 发布命令

hexo clean && hexo d && git add . && git commit -m 'update diary' && git push

## 生成日记

hexo new 'x' -p daily/2019/

## 同步图片至 7 牛云

hexo qiniu sync

## page title

top: true
toc: false
