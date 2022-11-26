---
layout: default
title: "Conda note"
description: This is a note about conda
cateogries: conda
permalink: /post/2022-07-29-conda-note/
---
# Conda note

## What is Conda

[The offical website of Conda](https://www.anaconda.com/)

## How to use Conda

### Conda command

#### Conda list
List linked packages in a conda environment.

```
usage: conda list [-h] [-n ENVIRONMENT | -p PATH] [--json] [-v] [-q]
                  [--show-channel-urls] [-c] [-f] [--explicit] [--md5] [-e]
                  [-r] [--no-pip]
                  [regex]
```


#### Conda 换源
[Anaconda清华镜像换源](https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/)
在`.condarc`中添加TUNA镜像源

```
channels:
  - defaults
show_channel_urls: true
default_channels:
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/r
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/msys2
custom_channels:
  conda-forge: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  msys2: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  bioconda: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  menpo: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  pytorch: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  pytorch-lts: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  simpleitk: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
```
**注意**: Windows下需要执行`conda config --set show_channel_urls yes`生成文件后再修改

运行`conda clean -i`清除索引缓存

使用`conda config`生成`.condarc`文件


#### Conda update conda
```
conda update conda

proceed ([y]/n)? y
```

#### Managing environments

创建环境
```
conda create -n 你想要的名字 python
```

eg:创建一个名叫tf包含Python和TensorFlow两个包的环境
```
conda create -n tf python=3.8 tensorflow=2.3
```


查看环境
```
conda info -e
```

激活环境
```
conda activate 虚拟环境的名称
```

在环境中安装模块
```
conda install 模块名
```

删除环境
```
conda remove -n 环境名 --all
```





```
conda create --name snowflakes biopython
```

```
proceed ([y]/n)? y

---

## Contact me

* Blog -> <https://shijiang.tk>
* Email -> <ssj1595329871@qq.com>
* Github -> [sunshijiang@Github](https://github.com/sunshijiang)
