---
title: SVG,初次尝试
excerpt_separator: "<!--more-->"
categories:
    - SVG
tags:
    - SVG
image: assets/images/svg_title.jpg    
---
+ 遇到的一些难题
<!--more-->

+ ##### 关于<picture>标签
此前我有想使用jpg格式的图片来实现动画效果，于是我想直接加入图片以及svg动画效果尝试有无反应..
![Alt text](/assets/images/img_modify.png)
结果不如所料，没能得到我想要的结果...	
<br>

接着，我猜测是否可以用<picture>标签来尝试能否实现svg动画效果
于是——
![Alt text](/assets/images/picture_label.png)
结果，还是无法显示效果。
之后从百度上了解到，<picture>标签目前仍不被浏览器支持，如果想使用<picture>标签，必须用<span>配合媒体查询或者使用javascript动态返回图片。
但由于网新专业没有学习js语言，所以我不得不放弃了这个想法...

<svg height="70">
  <g> 
<text font-family="microsoft yahei" font-size="20" y="30" x="30" font-color="blue">
 I Love Jekyll！！！
<circle cx="100" cy="200" r="30" style="fill:none;stroke-width:3;stroke:black">
<animate attributeType="XML" attributeName="r" 
from="0" to="30" dur="3s"
restart="always" repeatCount="3">
</animate>
</circle>
</text>
  </g>
</svg>   

