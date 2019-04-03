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
    List<File> files = Arrays.stream(file.listFiles())
        .filter(a -> !a.getName().equals(".DS_Store")).collect(
            Collectors.toList());
    for (int i = 0; i < files.size(); i++) {
        //文件名除了后缀没有字符 .
        String filename =
            System.nanoTime() + "." + files.get(i).getName().split("\\.")[1];
        files.get(i).renameTo(new File(files.get(i).getParent(), filename));
    }

    List<File> files1 = Arrays.stream(file.listFiles())
        .filter(a -> !a.getName().equals(".DS_Store")).collect(
            Collectors.toList());
    for (int i = 0; i < files1.size(); i++) {
        //文件名除了后缀没有字符 .
        String filename = i + "." + files1.get(i).getName().split("\\.")[1];
        files1.get(i).renameTo(new File(files1.get(i).getParent(), filename));
    }
    Arrays.stream(file.listFiles())
        .forEach(f -> System.out.println(f.getName()));
}
```
