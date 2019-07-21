---
author: Jay Yang
categories: java
tags: 
    - java
    - fastjson 
title: fastjson SerializerFeature
date: 1999-01-01 00:00:00
img:
toc: false
---

|                                |                                                                                                                            |
| ------------------------------ | -------------------------------------------------------------------------------------------------------------------------- |
| QuoteFieldNames                | 输出 key 时是否使用双引号,默认为 true                                                                                      |
| UseSingleQuotes                | 使用单引号而不是双引号,默认为 false                                                                                        |
| WriteMapNullValue              | 是否输出值为 null 的字段,默认为 false                                                                                      |
| WriteEnumUsingToString         | Enum 输出 name()或者 original,默认为 false                                                                                 |
| UseISO8601DateFormat           | Date 使用 ISO8601 格式输出，默认为 false                                                                                   |
| WriteNullListAsEmpty           | List 字段如果为 null,输出为[],而非 null                                                                                    |
| WriteNullStringAsEmpty         | 字符类型字段如果为 null,输出为”“,而非 null                                                                                 |
| WriteNullNumberAsZero          | 数值字段如果为 null,输出为 0,而非 null                                                                                     |
| WriteNullBooleanAsFalse        | Boolean 字段如果为 null,输出为 false,而非 null                                                                             |
| SkipTransientField             | 如果是 true，类中的 Get 方法对应的 Field 是 transient，序列化时将会被忽略。默认为 true                                     |
| SortField                      | 按字段名称排序后输出。默认为 false                                                                                         |
| WriteTabAsSpecial              | 把\\t 做转义输出，默认为 false `不推荐`                                                                                    |
| PrettyFormat                   | 结果是否格式化,默认为 false                                                                                                |
| WriteClassName                 | 序列化时写入类型信息，默认为 false。反序列化是需用到                                                                       |
| DisableCircularReferenceDetect | 消除对同一对象循环引用的问题，默认为 false                                                                                 |
| WriteSlashAsSpecial            | 对斜杠’/’进行转义                                                                                                          |
| BrowserCompatible              | 将中文都会序列化为\\uXXXX 格式，字节数会多一些，但是能兼容 IE 6，默认为 false                                              |
| WriteDateUseDateFormat         | 默认为 false。JSON.DEFFAULT_DATE_FORMAT = “yyyy-MM-dd”;JSON.toJSONString(obj, SerializerFeature.WriteDateUseDateFormat);   |
| DisableCheckSpecialChar        | 一个对象的字符串属性中如果有特殊字符如双引号 默认为 false                                                                  |
| NotWriteRootClassName          | 含义                                                                                                                       |
| BeanToArray                    | 将对象转为 array 输出                                                                                                      |
| WriteNonStringKeyAsString      | 含义                                                                                                                       |
| NotWriteDefaultValue           | 含义                                                                                                                       |
| BrowserSecure                  | 含义                                                                                                                       |
| IgnoreNonFieldGetter           | 含义                                                                                                                       |
| WriteEnumUsingName             | 含义                                                                                                                       |
