---
layout: default
title: "C++ Learn Note"
description: This is C++ learning note
categories: cpp
permalink: /post/2022-08-04-cpp-learn-note/
---

## 函数重载

```
#include <iostream>
unsigned long left(unsigned long num, unsigned ct); //调用left函数，left为long型，其中left函数有两个参数，一个是整型，一个是unsigned
char * left(const char * str, int n = 1);   //  调用left函数，left为char型，其中left有两个参数，一个是常量char，一个是整型

int main()
{
    using namespace std;
    char * trip = "Hawaii!!";   //  char型，常量
    unsigned long n = 12345678; //  long型
    int i;      //  整型
    char * temp;    //  char型

    for (i = 1; i < 10 ; i++)
    {
        cout << left(n, i) << endl; //  调用long left函数
        temp = left(trip, i);   //  调用 char left函数，i递增
        cout << temp << endl;   //  输出temp
        delete[] temp;  // 解除指针

    }
    return 0;
}

unsigned long left(unsigned long num, unsigned ct)
{
    unsigned digits = 1;
    unsigned long n = num;

    if (ct == 0|| num == 0)
        return 0;
    while (n /= 10)
        digits++;
    if (digits > ct)
    {
        ct = digits - ct;
        while (ct--)
            num /= 10;
        return num;
    }

    else
        return num;
}

char * left(const char * str, int n)
{
    if (n < 0)
        n = 0;
    char * p = new char[n+1];
    int i;
    for (i = 0; i < n && str[i]; i++)
        p[i] = str[i];
    while (i <= n)
        p[i++] = '\0';
    return p;
}
```
