---
layout: post
title: "Jekyll，属于你的个人博客！"
excerpt_separator: "<!--more-->"
categories:
     - 网页设计
image: assets/images/Jekyll.jpg
---

+ [Jekyll是什么？](https://jekyllrb.com/)
+ 如何结合Github架构属于你的个人博客..
+ [耗时、懵圈？让简书来教你！](https://www.jianshu.com/p/9f71e260925d)

<!--more-->

### 在学习Jekyll中遇到的困难
在专业老师及同学指导下，我尝试使用github操作jekyll项目。本人在学习中遇到许多难题。
#### 例如:
+ [衬线字体的运用](https://www.jianshu.com/p/4db1faaa92a8)
在修改衬线字体时，不知道衬线字体修改与你本人使用的博客皮肤是有关的，我在这里卡了2个小时，一直寻求不到解决方案，最后反复检查代码有无存在问题，从简书上了解到修改衬线字体需要与使用的皮肤相适应，因为原先衬线字体直接对应的是默认皮肤，而在此问题也就迎刃而解了。

<br>
![Alt text](/assets/images/night_face.png)

#### eg:上传首页Banner 
此前在尝试上传我的首页Banner时，想上传的图片一直加载不出来，无论我在index.md中修改图片路径，还是更换图片，仍旧没法显示图片，之后我在我的网页Jekyll中检查代码，发现网页给到我的错误是图片并没有得到反馈，也就是网页并没有发现这张图片。
后来检查我的代码，发现在page-intro.html中，我给它强制加上了一张图片，且图片路径是错误的，导致我在首页banner问题上卡了很多天。之后找到原作者的仓库，将此处的源代码更换，再重新再index.md上直接添加图片路径，问题也就迎刃而解了。

![Alt text](/assets/images/banner_problem.png)