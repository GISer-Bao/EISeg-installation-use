# EISeg的安装和使用

## **1. 介绍**
**1.1 何为EISeg?**

EISeg(Efficient Interactive Segmentation)基于飞桨开发的一个高效智能的交互式分割标注软件。它涵盖了通用、人像、遥感、医疗、视频等不同方向的高质量交互式分割模型。 另外，将EISeg获取到的标注应用到PaddleSeg提供的其他分割模型进行训练，便可得到定制化场景的高精度模型，打通分割任务从数据标注到模型训练及预测的全流程。（百度做的一个工具）

**1.2 EISeg的特点**

（1）高效的**半自动**标注工具，已上线多个Top标注平台

（2）覆盖**遥感**、医疗、视频、3D医疗等众多垂类场景

（3）多平台兼容，简单易用，支持多类别标签管理

**1.3 GitHub官方链接**

* 链接：<https://github.com/PaddlePaddle/PaddleSeg/tree/release/2.6/EISeg>

**1.4 官方视频介绍**

* [业界首个高性能交互智能标注工具EISeg_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1sQ4y1r754/?spm_id_from=333.337.search-card.all.click&vd_source=03252c088981228940ef0422a6ef7695)

## **2. 安装**
**2.1 创建虚拟环境**

（1）创建一个名为eiseg，python版本为3.8的环境
```
conda create -n eiseg python=3.8
```
（2）激活环境
```
conda activate eiseg
```

**2.2 安装EISeg**

（1）安装PaddlePaddle（安装的是CPU版）
```
pip install paddlepaddle
```
（2）安装EISeg
```
pip install eiseg
```
（3）打开EISeg
```
eiseg
```

**2.3 参考资料**
* [EISeg分割标注软件使用_太阳花的小绿豆的博客-CSDN博客](https://blog.csdn.net/qq_37541097/article/details/120154543?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522166747936816782414919113%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fblog.%2522%257D&request_id=166747936816782414919113&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~blog~first_rank_ecpm_v1~rank_v31_ecpm-2-120154543-null-null.nonecase&utm_term=%E6%A0%87%E6%B3%A8&spm=1018.2226.3001.4450)（安装时，请参考此文档）
* EISeg的 [github](<https://github.com/PaddlePaddle/PaddleSeg/tree/release/2.6/EISeg>)链接 
* 安装PaddlePaddle的GPU版本（<https://www.paddlepaddle.org.cn/install/quick?docurl=/documentation/docs/zh/install/conda/windows-conda.html>）

## **3. 使用教程**

**3.1 下载模型预训练权重**

* 模型下载链接(https://github.com/PaddlePaddle/PaddleSeg/blob/release/2.6/EISeg/docs/image.md)

![](https://github.com/GISer-Bao/EISeg-installation-use/blob/main/picture_shortcut/picture1.png)


**3.2 载入模型权重。**

* 在EISeg右上角点击“加载网络参数”按钮，加载刚刚下载的模型权重

![](https://github.com/GISer-Bao/EISeg-installation-use/blob/main/picture_shortcut/picture2.png)


**3.3 添加类别标签。**

* 在EISeg右侧点击“添加标签”按钮，添加自己分割任务中的目标类别

![](https://github.com/GISer-Bao/EISeg-installation-use/blob/main/picture_shortcut/picture3.png)

**3.4 标注图片**

关于如何使用EISeg进行具体标注，以及EISeg相关快捷键的使用，请参考以下文章或视频，可能出现的问题或错误，文章（视频）中都有详细说明。

* [EISeg分割标注软件使用_太阳花的小绿豆的博客-CSDN博客](https://blog.csdn.net/qq_37541097/article/details/120154543?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522166747936816782414919113%2522%252C%2522scm%2522%253A%252220140713.130102334.pc%255Fblog.%2522%257D&request_id=166747936816782414919113&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~blog~first_rank_ecpm_v1~rank_v31_ecpm-2-120154543-null-null.nonecase&utm_term=%E6%A0%87%E6%B3%A8&spm=1018.2226.3001.4450)
* [eiseg简单教学_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1dQ4y1674A/?spm_id_from=333.337.search-card.all.click&vd_source=03252c088981228940ef0422a6ef7695)）
* [eiseg_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1PR4y197Pk/?spm_id_from=333.337.search-card.all.click&vd_source=03252c088981228940ef0422a6ef7695)
* [好用的语义分割标注软件:Paddle-EISeg_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1e8411Y78k/?spm_id_from=333.337.search-card.all.click&vd_source=03252c088981228940ef0422a6ef7695)
* [使用EISeg进行半自动图像分割标注/抠图/抠视频_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1944y1f7P1/?spm_id_from=333.337.search-card.all.click&vd_source=03252c088981228940ef0422a6ef7695)
