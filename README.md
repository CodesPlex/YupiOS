# Yupios-鱼皮OS

## 项目介绍

这是一个基于 [GoodManWEN/GoodManWEN.github.io: 网页模拟桌面](https://github.com/GoodManWEN/GoodManWEN.github.io) 的项目二次开发的鱼皮操作系统/博客项目

## 快速使用[来自原中文仓库]

https://github.com/GoodManWEN/GoodManWEN.github.io/blob/main/misc/readme_chs.md

~~~
这是一个web驱动的仿写Deepin桌面UI的博客工具，设计上完全依托于Github Pages开源部署，
你可以用来提供一个你的个人博客或者用来当做个人简历。

这个项目产生于偶然，恰好由于近期需要整理一个博客做项目展示。作者在论坛看到Ubuntu的
同类版本，但由于该作品是由react编写，我不熟悉react，所以想要迁移一个vue的同类版本，
所以有了本项目。

打算要做一个项目的话，首先面临的是要实现哪个系统的问题。由于大家最喜欢的Ubuntu已经
有人完成，重新实现轮子没有什么意义，另外作者本人以前也曾见过MacOS的类似版本，而
Windows由于多年耕耘，模仿其动画细节的成本似乎过大。Linux发行版虽然丰富，但摆在我们
面前的选择似乎并不多，日常使用的红帽系发行版似乎并不专注于桌面体验，实现意义并不大。
剩下的广泛被接受的发行版似乎还剩Manjaro, Fedora, 以及一些所谓的Gaming ready distro。
最后我还是选择了Deepin，虽然没有用过，但也算是久闻大名，项目放在Github上供全世界的
vue开发者参考，也算是为国产做宣传了吧。
~~~

本项目在设计上是由Github Pages提供服务的，所有api都会被转化为静态文件分发。如果你想要在本地运行和调试的话，请尝试以下步骤:

~~~
git clone https://github.com/GoodManWEN/GoodManWEN.github.io.git
cd GoodManWEN.github.io.git
npm install
npm run serve
~~~

如果你的npm和vue-cli版本合适的话，这样应该足够令程序跑起来，项目使用的版本你可以在下文和`package.json`中找到参考。

如果你希望修改博客内容，那么你应该直接修改`/blog`目录中的内容，该目录中所有.md内容都会被直接映射到网站中。

修改后执行以下命令生成静态文件。

```
python3 generate.py
npm run build
```

由于修改了vue-cli的默认设置，静态文件生成在/docs目录中。

## 开源协议

**[AGPL-3.0 license](https://github.com/CodesPlex/YupiOS#AGPL-3.0-1-ov-file)**