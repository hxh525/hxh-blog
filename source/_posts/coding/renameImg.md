---
author: Jay Yang
categories: coding
tags: 
  - coding
  - java
title: renameImg
date: 2019-03-31 10:10:38
img:
---

#### 修改指定文件夹下的图片名称按照序号重命名

```java
public static void main(String[] args) {
    File file = new File("/Users/x/Downloads/untitled folder");
    File[] files = file.listFiles();
    for (int i = 0; i < files.length; i++) {
        String filename = i + files[i].getName().split(".")[2]);
        //文件名除了后缀没有字符 .
        files[i].renameTo(new File(files[i].getParent(), filename);
    }
    File[] files1 = file.listFiles();

    for (File file1 : files1) {
        System.out.println("file1.getName() = " + file1.getName());
    }
}
```
