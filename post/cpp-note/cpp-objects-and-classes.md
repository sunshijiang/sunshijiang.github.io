---
layout: default
title: "Objects and Classed"
categories: c++
description: This is a note of Objects and Classes
permalink: /post/cpp-note/cpp-objects-and-classes/
---
## 过程性编程和面向对象编程
## 类概念
## 如何定义和实现类
## 公有类访问和私有类访问
## 类的数据成员
## 类方法（类函数成员）
## 创建和使用类对象
## 类的构造函数和析构函数
## const成员函数
## this指针
## 创建对象数组
## 类作用域

#### 要调用公有成员函数，必须通过对象
<details><summary>调用公有成员函数</summary>
<pre><code>

Stock sleeper("Exclusive Ore", 100, 0.25);
sleeper.show();
show();
</code></pre>
</details>

#### 在定义成员函数时，必须使用作用域解析运算符
<details><summary>解析运算符</summary>
<pre><code>
void Stock::update(doubele price)
{
    ...
}
</code></pre>
</details>

### 作用域为类的常量

#### 在类中声明一个枚举

<details><summary>声明的枚举的作用域为整个类</summary>
<pre><code>
class Bakery
{
private:
    enum {Months = 12};
    double costs[Months];
    ...
}
</code></pre>
</details>

#### 使用关键字static

<details><summary>使用关键字static</summary>
<pre><code>
class Bakery
{
private:
    static const int Months = 12;
    double costs[Months];
    ...
}
</code></pre>
</details>

### 作用域内枚举


## 抽象数据类型

## Contact me
- Blog -> [shijiang.tk](https://shijiang.tk)
- Email -> <ssj1595329871@qq.com>
- Github -> [sunshijiang@Github](https://github.com/sunshijiang)
