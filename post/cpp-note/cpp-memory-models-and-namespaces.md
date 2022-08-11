---
layout: default
title: "Memory Models and Namespaces"
categories: cpp
description: This is a note of Memory Models and Namespaces
date: 2022-08-11 +0800
permalink: /post/cpp-note/cpp-memory-models-and-namespaces/
---
## 单独编译

头文件：包含结构声明和使用这些结构的函数的原型。  
源代码文件：包含与结构有关的函数的代码。  
源代码文件：包含调用与结构相关的函数的代码。  

头文件中常包含的内容。
- 函数原型
- 使用`#define`或`const`定义的符号常量
- 结构声明
- 类声明
- 模板声明
- 内联函数


在包含头文件时，使用"coordin.h"，而不是<coodin.h>。如果文件名包含在尖括号中个，则C++编译器将在存储标准头文件的主机系统的
文件系统中查找；但如果文件名包含在双引号中，则将在标准位置查找。因此在包含自己的头文件时，应使用引号而不是尖括号。




## Contact me
- Blog -> [shijiang.tk](https://shijiang.tk)
- Email -> <ssj1595329871@qq.com>
- Github -> [sunshijiang@Github](https://github.com/sunshijiang)

