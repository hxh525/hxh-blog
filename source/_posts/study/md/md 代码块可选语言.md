---
author: Jaye Huang
categories: md
p: daily/2019/
title: Md 文档支持的代码块引用语言高亮
date: 1999-01-01 00:00:00
img:
tags: md
---

#### Md 文档支持的代码块引用语言高亮

##### 代码

> \`\`\`css
> .bg-cover .description {
> &nbsp;&nbsp;font-weight: 300;
> &nbsp;&nbsp;line-height: 1.4em;
> &nbsp;&nbsp;color: #eee;
> &nbsp;&nbsp;cursor: default;
> }
> \`\`\`
> 注意: \`\`\` 后面填写的为下表的关键字

##### 效果

```css
.bg-cover .description {
  font-size: 1.25rem;
  font-weight: 300;
  line-height: 1.4em;
  color: #eee;
  cursor: default;
}
```

| 名称             | 关键字                    | 调用的 js             | 说明                                        |
| ---------------- | ------------------------- | --------------------- | ------------------------------------------- |
| AppleScript      | applescript               | shBrushAppleScript.js |                                             |
| ActionScript 3.0 | actionscript3 , as3       | shBrushAS3.js         |                                             |
| Shell            | bash , shell              | shBrushBash.js        |                                             |
| ColdFusion       | coldfusion , cf           | shBrushColdFusion.js  |                                             |
| C                | cpp , c                   | shBrushCpp.js         |                                             |
| C\#              | c\# , c-sharp , csharp    | shBrushCSharp.js      |                                             |
| CSS              | css                       | shBrushCss.js         |                                             |
| Delphi           | delphi , pascal , pas     | shBrushDelphi.js      |                                             |
| diff&patch       | diff patch                | shBrushDiff.js        | 用代码版本库时,遇到代码冲突,其语法就是这个. |
| Erlang           | erl , erlang              | shBrushErlang.js      |                                             |
| Groovy           | groovy                    | shBrushGroovy.js      |                                             |
| Java             | java                      | shBrushJava.js        |                                             |
| JavaFX           | jfx , javafx              | shBrushJavaFX.js      |                                             |
| JavaScript       | js , jscript , javascript | shBrushJScript.js     |                                             |
| Perl             | perl , pl , Perl          | shBrushPerl.js        |                                             |
| PHP              | php                       | shBrushPhp.js         |                                             |
| text             | text , plain              | shBrushPlain.js       | 就是普通文本.                               |
| Python           | py , python               | shBrushPython.js      |                                             |
| Ruby             | ruby , rails , ror , rb   | shBrushRuby.js        |                                             |
| SASS&SCSS        | sass , scss               | shBrushSass.js        |                                             |
| Scala            | scala                     | shBrushScala.js       |                                             |
| SQL              | sql                       | shBrushSql.js         |                                             |
| Visual Basic     | vb , vbnet                | shBrushVb.js          |                                             |
| XML              | xml , xhtml , xslt , html | shBrushXml.js         |                                             |
| Objective C      | objc , obj-c              | shBrushObjectiveC.js  |                                             |
| F\#              | f\# f-sharp , fsharp      | shBrushFSharp.js      |                                             |
|                  | xpp , dynamics-xpp        | shBrushDynamics.js    |                                             |
| R                | r , s , splus             | shBrushR.js           |                                             |
| matlab           | matlab                    | shBrushMatlab.js      |                                             |
| swift            | swift                     | shBrushSwift.js       |                                             |
| GO               | go , golang               | shBrushGo.js          |                                             |  |
