---
index_img: https://hexo-blog-netlify.oss-cn-shenzhen.aliyuncs.com/0FEE9279-5461-4521-86A9-70696B2065E7.jpeg
title: Sigmoid函数
date: 2022-12-25 23:09:04
updated: 2022-12-25 23:09:05
tags:
  - 数学
categories:
  - 机器学习
keywords:
  - sigmoid
comments: true
---
[Sigmoid函数](https://baike.baidu.com/item/Sigmoid函数/7981407)是一个在生物学中常见的S型函数，也称为S型生长曲线。在深度学习中，由于其单增以及反函数单增等性质，Sigmoid函数常被用作神经网络的激活函数，将变量映射到\[0,1]之间。\
$$
\mathrm{S}(\mathrm{x})=\frac{1}{1+\mathrm{e}^{-\mathrm{x}}}
$$

Sigmoid函数的导数可以用其自身表示：\
$$
\mathrm{S}^{\prime}(\mathrm{x})=\frac{\mathrm{e}^{-\mathrm{x}}}{\left(1+\mathrm{e}^{-\mathrm{x}}\right)^2}=\mathrm{S}(\mathrm{x})(1-\mathrm{S}(\mathrm{x}))
$$

Sigmoid函数的特性与优缺点：

* Sigmoid函数的输出范围是0到1。由于输出值限定在0到1，因此它对每个神经元的输出进行了归一化。
* 用于将预测概率作为输出的模型。由于概率的取值范围是0到1，因此Sigmoid函数非常合适
* 梯度平滑，避免跳跃的输出值
* 函数是可微的。这意味着可以找到任意两个点的Sigmoid曲线的斜率
* 明确的预测，即非常接近1或0。
* 函数输出不是以0为中心的，这会降低权重更新的效率
* Sigmoid函数执行指数运算，计算机运行得较慢。

Sigmoid函数及其导数的图像：

![Sigmoid](https://hexo-blog-netlify.oss-cn-shenzhen.aliyuncs.com/post/%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0/30EB0B41-AB32-44A6-B91E-860B3997D16A.jpeg)