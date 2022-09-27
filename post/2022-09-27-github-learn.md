---
layout: default
title: "Github Learn"
description: This is a note of github learnning
categories: github
permalink: /post/2022-09-27-github-learn/
---

# github-learn
**This is a repository which i used to learn 'how to use github'**

---

## 创建折叠部分
<details><summary>Click Me</summary>
<p>
    
### 看不见我(:><:)
                   
```C++
   cout << "Hello World" << endl;
```
</p>  
    
</details>

## 创建图表

<details><summary>Mermaid Chart</summary>

<p>
    
### 创建Mermaid图表
    
Here is a simple flow chart:

```mermaid
graph TD;
    A --> B;
    A --> C;
    B --> D;
    C --> D;
```
</p>
    
</details>


### 创建geoJSON和topoJSON

<details><summary>geoJSON Map</summary>
    
<p>
    
#### 创建geosjson
    
```geoJSON
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "id": 1,
      "properties": {
         "ID": 0
      },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
              [-90,35],
              [-90,30],
              [-85,30],
              [-85,35],
              [-90,35]
          ]
        ]
      }
    }
  ]
}
```
    
</p>
    
</details>

## 编辑数学表达式

### 编辑内联表达式

使用`$`分隔符：$\sqrt{3x-1}+(1+x)^2$

### 将表达式编写为块

**The Cauchy-Schwarz Inequality**

$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

or

**Here is some math!**

```math
\sqrt{3}
```

**使用`<span>$</span>`显示`$`符号**

<span>$</span>100/2<span>$</span>

## 自动链接的引用和URL

### URL

visit http://github.com/sunshijiang/github-learn

### 议题和拉取请求

https://github.com/sunshijiang/github-learn/issues/1    //  源引用

or

#1  // 使用`#`和议题或拉取请求编号

or

GH-1    //  `GH-`和议题或拉取请求编号

sunshijiang/github#1    //  使用`用户名/仓库#`和议题或拉取请求编号

### 提交SHA
对提交SHA哈希的引用会自动转换为指向GitHub上提交的短链接

## 附加文件


## 创建指向代码段的永久链接

github.com/sunshijiang/android_kernel_xiaomi_msm8998/blob/f4d429ae82f1e546b96358ad349f781fa7807a6c/arch/arm64/Makefile#L24-L31

## 链接到Markdown

github.com/sunshijiang/android_kernel_xiaomi_msm8998/blob/lineage-19.1/README?plain=1#L22


## Contact me
- Blog -> [shijiang.tk](https://shijiang.tk)
- Email -> <ssj1595329871@qq.com>
- Github -> [sunshijiang@Github](https://github.com/sunshijiang)
