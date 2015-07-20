# GITHUB的android客户端设计与实现

### 序·写在前面
这是鄙人在大学本科的一个毕业设计，设计思路的来源是当时在公司实习导师的启发：官方的GitHub客户端一直迟迟不更新，我们可以做一个自己的客户端。在实习期间导师提了一下，在毕业设计选题的时候，很巧地想到了当时的这个建议。在实施之前，我先去GitHub的开发者网站上是否有相应的API以及其功能的覆盖程度够不够高。在研究完GitHub的API之后，初步认为可行性极强，然后就向导师确立了这个题目。刚开始，学校的导师建议换个题目，说这个课题实用性不大。其实实用性是什么，做出来有人会用就好，这个又不是很严格的商业项目。最后，导师妥协了。
这算是一个完全是经我手的一个项目，从开始的可行性以及需求分析，到框架设计，以及切图都是自己完成的（图片都是从[阿里巴巴矢量图标库](http://www.iconfont.cn/)获取，再经过自己的部分修改）。在做的过程中，慢慢地发觉自己的不足。比如刚开始觉得自己设计的框架挺不错的，然而到后面发觉自己封装地还不够，就停下进度，再重新改了好几遍框架。
做的过程中，我发觉了[GitHub官方的客户端](https://github.com/forkhubs/android)是开源，这为了后期的修Bug给了很大的帮助，这也使得最后一阶段的开发有点模仿开源的了。但我还是坚决要作出自己的一个特色。
软件算是已经完成了吧，放到市场上，发觉Bug好多。开始时一个月，鸵鸟算法，不想管他。后面发觉不管不行，然后就反复修了一点点。
总的来说，这个对我的锻炼还是挺大的。


------

### 一、使用的库

这些库需要导入依赖：
> * [GitHub Java API](https://github.com/eclipse/egit-github/tree/master/org.eclipse.egit.github.core)
> * [SmoothProgressBar](https://github.com/castorflex/SmoothProgressBar)
> * [Android-Universal-Image-Loader](https://github.com/nostra13/Android-Universal-Image-Loader)

项目当中还继承了一些其他的类库：
> * [android-gif-drawable](https://github.com/koral--/android-gif-drawable)
> * [SwipeBackLayout](https://github.com/ikew0ng/SwipeBackLayout)
> * [gravatar-android](https://github.com/tkeunebr/gravatar-android)
> * [TouchImageView](https://github.com/MikeOrtiz/TouchImageView)


![logo](https://github.com/gdestiny/graduation_github/blob/master/Test/Screenshot/show.png?raw=true)

# 二、使用
使用eclipse导入项目与相应的库

# 三、软件部分截图
| ![logo](https://github.com/gdestiny/graduation_github/blob/master/Test/Screenshot/01-splash.png?raw=true) |![logo](https://github.com/gdestiny/graduation_github/blob/master/Test/Screenshot/02-homeMenu.png?raw=true)|![logo](https://github.com/gdestiny/graduation_github/blob/master/Test/Screenshot/03-code.png?raw=true)|
| --------   | -----:  | :----:  |
| ![logo](https://github.com/gdestiny/graduation_github/blob/master/Test/Screenshot/04-codefile.png?raw=true) | ![logo](https://github.com/gdestiny/graduation_github/blob/master/Test/Screenshot/05-commit.png?raw=true) |  ![logo](https://github.com/gdestiny/graduation_github/blob/master/Test/Screenshot/06-event.png?raw=true)  |
|  ![logo](https://github.com/gdestiny/graduation_github/blob/master/Test/Screenshot/07-issue.png?raw=true) |  ![logo](https://github.com/gdestiny/graduation_github/blob/master/Test/Screenshot/gist.png?raw=true)  | ![logo](https://github.com/gdestiny/graduation_github/blob/master/Test/Screenshot/dashboard.png?raw=true)|

