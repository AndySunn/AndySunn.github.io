---
title: SVG,实现动画
excerpt_separator: "<!--more-->"
categories:
    - SVG
tags:
    - SVG
image: assets/images/svg_title.jpg    
---
+ 关于SVG的一些知识
<!--more-->
<br>

 + ##### 首先，关于SVG，我们需要了解其概念
 1. 这是一种可伸缩矢量图形
 2. 使用XML(可拓展标记语言)来描述
 3. SVG图像在放大或改变尺寸的情况下其图像质量不会有所损失
 ...
 + #####一些定义
 + <animateTransform> 动画上一个目标元素变换属性，从而使动画控制平移，缩放，旋转或倾斜
    |元素|定义|
    |---|:---:|
    |g|用于把相关元素进行组合的容器元素|
    |animate|随时间动态改变属性| →  ①attributeName="目标属性名称" ②from="起始值" ③to="结束值" ④dur="持续时间"
    |animateTransform|动画上一个目标元素变换属性，从而使动画控制平移，缩放，旋转或倾斜|
    |circle|定义一个圆| →  ①cx="圆的x轴坐标" ②cy="圆的y轴坐标" ③r="圆的半径"
    |svg|创建一个SVG文档片段|
    |text|定义一个文本|
    |...|...|

<svg width="200px"  height="200px"  xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="xMidYMid" class="lds-pacman" style="background: none;">
<g ng-attr-style="display:{{config.showBean}}" style="display:block"><circle cx="79.9238" cy="50" r="4" ng-attr-fill="{{config.c2}}" fill="#ff765c"><animate attributeName="cx" calcMode="linear" values="95;35" keyTimes="0;1" dur="1" begin="-0.67s" repeatCount="indefinite"></animate><animate attributeName="fill-opacity" calcMode="linear" values="0;1;1" keyTimes="0;0.2;1" dur="1" begin="-0.67s" repeatCount="indefinite"></animate></circle><circle cx="40.3238" cy="50" r="4" ng-attr-fill="{{config.c2}}" fill="#ff765c"><animate attributeName="cx" calcMode="linear" values="95;35" keyTimes="0;1" dur="1" begin="-0.33s" repeatCount="indefinite"></animate><animate attributeName="fill-opacity" calcMode="linear" values="0;1;1" keyTimes="0;0.2;1" dur="1" begin="-0.33s" repeatCount="indefinite"></animate></circle><circle cx="60.1238" cy="50" r="4" ng-attr-fill="{{config.c2}}" fill="#ff765c"><animate attributeName="cx" calcMode="linear" values="95;35" keyTimes="0;1" dur="1" begin="0s" repeatCount="indefinite"></animate><animate attributeName="fill-opacity" calcMode="linear" values="0;1;1" keyTimes="0;0.2;1" dur="1" begin="0s" repeatCount="indefinite"></animate></circle></g><g ng-attr-transform="translate({{config.showBeanOffset}} 0)" transform="translate(-15 0)"><path d="M50 50L20 50A30 30 0 0 0 80 50Z" ng-attr-fill="{{config.c1}}" fill="#fc4309" transform="rotate(37.6857 50 50)"><animateTransform attributeName="transform" type="rotate" calcMode="linear" values="0 50 50;45 50 50;0 50 50" keyTimes="0;0.5;1" dur="1s" begin="0s" repeatCount="indefinite"></animateTransform></path><path d="M50 50L20 50A30 30 0 0 1 80 50Z" ng-attr-fill="{{config.c1}}" fill="#fc4309" transform="rotate(-37.6857 50 50)"><animateTransform attributeName="transform" type="rotate" calcMode="linear" values="0 50 50;-45 50 50;0 50 50" keyTimes="0;0.5;1" dur="1s" begin="0s" repeatCount="indefinite">
</animateTransform>
</path>
</g>
</svg>