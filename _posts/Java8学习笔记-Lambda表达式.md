---
layout: post
title: Java8学习笔记-Lambda表达式
description: "Java8学习笔记-Lambda表达式"
tags: [Java]

---

> 前些天看了《编程之法》中一道字符串包含的问题，作者使用位运算方法模拟散列表，从而巧妙的解答了这个问题，大大降低了时间复杂度，小弟我再次被自己的渣渣智商打击到了。虽然笔者也在两数交换中用到过位运算，然而仅仅是用过，并没有对位运算做过更多的了解，直到……哎，痛定思痛，闲话不多说了，开始献丑，各位看官将就着看。


## 0 基本概念
Lambda的形式

Lambda存在两种形式：

    形式1：(parameters) -> expression
    形式2：(parameters) -> { statements; }

当且仅当parameters只有一个参数时，括号可省略。

    () -> {}是一个合法的Lambda表达式，与Runnable接口相匹配。



Lambda的本质

Lambda其本质是「匿名内部类」的一种「语法糖」表示，存在如下3个方面的特征：

    Anonymous Function：匿名的函数；
    Passed Around：可作为参数或返回值，可以自由地被传递或存储；
    Concise：相对于匿名内部类的样板代码(Boilerplate)，Lambda更加简洁、漂亮。




## 参考文章

- [与 Java8 有个约会：Lambda 表达式](https://codingstyle.cn/topics/149)


***

**特别说明：**

1. 本文对以上参考文章有多处引用和借鉴，如有侵权，请留言，小生必改之；文中如有错误，也请留言，小生亦改之。
2. 感谢互联网上所有秉持开源精神、愿意分享知识的前辈，致敬！
3. 文章转载请注明出处，谢谢。
