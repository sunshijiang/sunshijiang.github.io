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
unsigned long left(unsigned long num, unsigned ct); //����left������leftΪlong�ͣ�����left����������������һ�������ͣ�һ����unsigned
char * left(const char * str, int n = 1);   //  ����left������leftΪchar�ͣ�����left������������һ���ǳ���char��һ��������

int main()
{
    using namespace std;
    char * trip = "Hawaii!!";   //  char�ͣ�����
    unsigned long n = 12345678; //  long��
    int i;      //  ����
    char * temp;    //  char��

    for (i = 1; i < 10 ; i++)
    {
        cout << left(n, i) << endl; //  ����long left����
        temp = left(trip, i);   //  ���� char left������i����
        cout << temp << endl;   //  ���temp
        delete[] temp;  // ���ָ��

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
