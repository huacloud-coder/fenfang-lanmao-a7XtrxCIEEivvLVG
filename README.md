

> 🍄 **大家好，我是风筝**
> 
> 
> 🌍 个人博客：【[古时的风筝](https://github.com)】。
> 
> 
> 本文目的为个人学习记录及知识分享。如果有什么不正确、不严谨的地方请及时指正，不胜感激。
> 
> 
> 每一个赞都是我前进的动力。
> 
> 
> 公众号：「古时的风筝」


前几天顺手改的一个安卓启动器，开源没几天，没想到[GitHub](https://github.com)上已经获得了40多颗星，要知道我前段时间花了两个星期写的[Jetbrains](https://github.com):[westworld加速](https://tianchuang88.com) 摸鱼插件一直无人问津。


**事情是这样的：**


前几到一个开源的安卓启动器，叫做Olauncher。是那种极简风格，是那种“穷凶极恶”的简约风格。作为一个安卓老用户（没错，从来没用过iPhone，主要因为穷），我一直想用最原生的那种风格。


![](https://p0-xtjj-private.juejin.cn/tos-cn-i-73owjymdk6/89cfd5800e1c4def9097083eab9029d1~tplv-73owjymdk6-jj-mark-v1:0:0:0:0:5o6Y6YeR5oqA5pyv56S-5Yy6IEAg5Y-k5pe255qE6aOO562d:q75.awebp?policy=eyJ2bSI6MywidWlkIjoiNTAxMDMzMDM1Mzc0MDQ1In0%3D&rk3s=f64ab15b&x-orig-authkey=f32326d3454f2ac7e96d3d06cdbb035152127018&x-orig-expires=1728179601&x-orig-sign=EXw%2BPyk5yvkbzvmqc6%2F4burMEzs%3D)



> 科普一下什么是启动器。
> 
> 
> 启动器是一个安卓应用，负责管理和显示主屏幕和应用抽屉。它决定了用户在主屏幕上的图标布局、桌面小部件（widgets）、快捷方式等。启动器也是用户打开应用的入口。


我一看，这是我的菜啊。然后马不停蹄的给自己安排上了，果然是极简，将它设置成默认启动器后，整个手机只有一屏了，也就是启动屏幕，屏幕上最多可以放置 8 个应用入口。


且应用出口的显示就是纯纯的应用名称，整个屏幕只有三部分组成，壁纸、几个主要应用入口和日期显示，且日期还可以不显示。


![](https://p0-xtjj-private.juejin.cn/tos-cn-i-73owjymdk6/b4a6f49b729948939ae4dfa6e28b3f1f~tplv-73owjymdk6-jj-mark-v1:0:0:0:0:5o6Y6YeR5oqA5pyv56S-5Yy6IEAg5Y-k5pe255qE6aOO562d:q75.awebp?policy=eyJ2bSI6MywidWlkIjoiNTAxMDMzMDM1Mzc0MDQ1In0%3D&rk3s=f64ab15b&x-orig-authkey=f32326d3454f2ac7e96d3d06cdbb035152127018&x-orig-expires=1728179601&x-orig-sign=5hhYpIvmVIqQV4tANgvMORefO5I%3D)


## 站在巨人的肩膀上


本以为这样就结束了，用就好了。但是，我发现几个地方不太符合我的要求。


谁让咱是程序员呢，谁让这项目是开源的呢，实在是没忍住，我就把源码拉下来了，又是没忍住，我就把代码给改了，顺便给它起了个名字叫做『一无桌面』。


改完之后又没忍住，我就给刚到 GitHub 上了，仓库地址： [https://github.com/huzhicheng/ALauncher](https://github.com)


主要改动的地方有下面几个：


1、日期和电量的显示


默认日期是显示为西式格式的，我给改成了 `2024/09/25 周三`这种格式，并且给电量前面加了个图标，这也是主屏上的唯一一个图标了，但这个图标实际上就是一个 emoji 。


上图已经是我改完之后的了。


2、长按屏幕空白区域会弹出设置界面，去掉了一些多余的信息，将界面变得更简单了。


3、上划会显示所有应用列表，因为是极简风格，所以应用以单列表形式展示，并且没有图标。我改成了三列显示，并且添加了图标。


4、调整了默认字体大小，之前的默认字体过大，有点儿像老年主题，可能刚使用的人看到这个大字号，影响观感，容易劝退。


下面是修改后的样式，注意壁纸需要你自己设置啊，壁纸很大程度上影响这个启动器的格调。


一张风景壁纸配上启动器
![](https://p0-xtjj-private.juejin.cn/tos-cn-i-73owjymdk6/4f72a7ba55cb4eee9fcf72838572e523~tplv-73owjymdk6-jj-mark-v1:0:0:0:0:5o6Y6YeR5oqA5pyv56S-5Yy6IEAg5Y-k5pe255qE6aOO562d:q75.awebp?policy=eyJ2bSI6MywidWlkIjoiNTAxMDMzMDM1Mzc0MDQ1In0%3D&rk3s=f64ab15b&x-orig-authkey=f32326d3454f2ac7e96d3d06cdbb035152127018&x-orig-expires=1728179601&x-orig-sign=aodabwye8isCcKC5hmnlmhlL5XA%3D)


一张人物壁纸配上启动器
![](https://p0-xtjj-private.juejin.cn/tos-cn-i-73owjymdk6/65119abdfb7b4cb58f14ee9ce733a514~tplv-73owjymdk6-jj-mark-v1:0:0:0:0:5o6Y6YeR5oqA5pyv56S-5Yy6IEAg5Y-k5pe255qE6aOO562d:q75.awebp?policy=eyJ2bSI6MywidWlkIjoiNTAxMDMzMDM1Mzc0MDQ1In0%3D&rk3s=f64ab15b&x-orig-authkey=f32326d3454f2ac7e96d3d06cdbb035152127018&x-orig-expires=1728179601&x-orig-sign=dGvu3rEJkbesW61fCb7f%2FMB7BrQ%3D)


## 使用方式


使用很简单，默认按照应用后，会提示你是否设置为默认启动器，当然了，如果你不设置成默认启动器，好像没什么意义。


在主界面设置常用应用，比如微信、微信读书等


长按桌面空白处，可以呼出设置界面，在设置界面可以设置主屏内容排布位置、字体大小、日期格式、左滑右滑呼出的应用等。


在主界面上滑会呼出所有应用列表，可以打开任意应用。且支持名称搜索。


## 最后


使用之后呢，感觉界面清爽了很多，仿佛手机都变轻了。


而且，刷手机的时间都变短了。比如闲下来时顺手拿起手机想打开某音看一下，结果一看屏幕啥都没有，然后就放下了，哈哈。


有兴趣的可以试一试哦。


源码地址和下载地址： [https://github.com/huzhicheng/ALauncher](https://github.com)


![](https://img2023.cnblogs.com/blog/273364/202307/273364-20230726083817916-1774523265.png)


