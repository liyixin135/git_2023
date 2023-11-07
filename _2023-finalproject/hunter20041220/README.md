# 课程总结

## ubuntu的安装以及各式软件的安装

* 安装ubuntu

作为一名电脑小白，开学前没有摸过电脑键盘，在优秀的学长以及奕欣姐姐的优秀教导之下，我学会了安装ubuntu,clion以及ros

## vim文本编辑器的使用，shell,脚本

* vim各种命令

第一节课我们学习了vim编辑器，学会了如何使用vim这款强大的编辑器，例如在编辑模式，命令模式，一般模式中切换：i,a,o进入编辑模式；esc退出。:或/进入命令模式；esc退出。以及光标的移动，复制粘贴，改单词，高亮，搜索关键词等功能。功能众多
请联系我查看我精美的书面笔记。


* shell及脚本

学习了简单的shell的设计原理，以及脚本的应用，就比如第一讲作业中打印错误出现了多少次。还有鱼香ros的脚本，一键安装ros（虽然我没用，但我安装完回头看发现我是真的小丑。

## linux基本命令以及命令行环境

* linux命令

学习了ls;man;help;pwd;cd;mkdir;rmdir;touch;cp;mv;rm;cat;more;less;echo;head;tail;ln;>和>>;history这些命令以及他们加选项后的应用，-a;-l;-t;等等众多命令，还有下载安装中的unzip等等，详情请联系我查看我精美的书面笔记。

* 命令行环境以及数据整理

在第二节作业中，我学习了正则表达式，以及创建别名alias,还有配置ssh,以及任务控制。并且在作业中进行了应用。

## git使用以及github

* git使用

了解了git的简单设计原理，并基于此基础上学会了建立本地空仓库，并进行git add,git commit,git status,git push。并且了解了工作区，缓冲区等概念。

* github使用

学会了fork以及Pull request，学会配置ssh密钥以及将gihub上的源码通过git clone克隆到本地仓库。

## catkin和cmake

* cmake

了解到cmake的基本设计原理，它作为编译语言的中间工具，可以不拘泥限制于编译器。并且从六个实际案例学到了：

1. 配置简单cmakelists

2. 配置简单的cmake工程

3. 将自身代码作为库目标

4. 配置多级cmakelists工程

5. 如何添加第三方库

6. 如何安装自己的工程

* catkin

了解到catkin的工作空间主要构成，并了解CMakeLists,Package.xml

## ROS

1. ros软件包结构

包括package.xml;CMakeLists,txt;src以及相关日志文件

2. 使用clion开发ros程序

如何创建软件包
catkin create pkg <包名> <依赖包如roscpp> 

3. ros话题通信

订阅者和发布者以及相关源码实现

4. ros参数服务器

如何获取参数的值以及设置参数大小

5. Rviz

ros的3D可视化工具，订阅节点和观看消息内容

6. TF

* 如何跟踪多个坐标系，并且以树形结构维护多个参考系坐标变换关系

* 如何将向量，时间等数据的坐标在两个参考系中完成坐标变换

7. rqt

* 实时获得可视化图像

* 可视化ros节点关系

8. plotjuggle 

* 二维图像中可视化数值

9. URDF

* 定义XML格式文件表机器人模型从而包括
  * 运动学轨迹
  * 视觉显示
  * 碰撞模型

10. SDF

描述环境；物体；传感器；机器人等从而生成机器人外部环境






