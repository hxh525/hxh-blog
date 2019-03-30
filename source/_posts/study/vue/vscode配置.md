---
author: Jay Yang
categories: js
tags: vscode
title: vscode配置
date: 2019-03-29 13:57:58
img:
---

#### vscode config

```json
{
  // vue eslint设置
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    {
      "language": "html",
      "autoFix": true
    },
    {
      "language": "vue",
      "autoFix": true
    }
  ],
  // 保存自动修复
  "eslint.autoFixOnSave": true,
  // tab锁紧
  "editor.tabSize": 2,
  // 保存格式化
  "editor.formatOnSave": true,
  // html格式化
  "html.format.enable": false,
  // css 校验
  "css.validate": false,
  // eslint 集成
  "prettier.eslintIntegration": true,
  // 自动保存
  "files.autoSave": "afterDelay",
  // vue 格式化js关闭
  "vetur.format.defaultFormatter.js": "none"
}
```
