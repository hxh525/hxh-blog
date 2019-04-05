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
  "workbench.startupEditor": "welcomePage",
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "window.zoomLevel": 0,
  "gitlens.advanced.messages": {
    "suppressCommitHasNoPreviousCommitWarning": false,
    "suppressCommitNotFoundWarning": false,
    "suppressFileNotUnderSourceControlWarning": false,
    "suppressGitVersionWarning": false,
    "suppressLineUncommittedWarning": false,
    "suppressNoRepositoryWarning": false,
    "suppressResultsExplorerNotice": true,
    "suppressShowKeyBindingsNotice": true,
    "suppressUpdateNotice": false,
    "suppressWelcomeNotice": true
  },
  "workbench.colorTheme": "Visual Studio Dark",
  "gitlens.keymap": "alternate",
  "git.autofetch": true,
  "git.confirmSync": false,
  "git.enableSmartCommit": true,
  "gitlens.views.repositories.files.layout": "tree",
  "gitlens.views.fileHistory.enabled": true,
  "gitlens.views.lineHistory.enabled": true,
  "editor.suggestSelection": "first",

  // eslint设置
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
  "vetur.format.defaultFormatter.js": "none",
  "javascript.updateImportsOnFileMove.enabled": "always",
  "editor.minimap.enabled": true,
  "editor.renderWhitespace": "none",
  "workbench.activityBar.visible": true,
  "workbench.statusBar.visible": true,
  "git.autoStash": true
}
```
