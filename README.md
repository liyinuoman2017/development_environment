# development_environment
从零入手人工智能（2）——搭建开发环境
## 1.前言

作为一名单片机工程师，想要转型到人工智能开发领域的道路确实充满了挑战与未知。**记得当我刚开始这段旅程时，心中充满了迷茫和困惑**。面对全新的领域，我既不清楚如何入手，也不知道能用人工智能干什么。正是这些迷茫和困惑，激发了我不断探索和学习的动力。经过一段时间的摸索和实践，我逐渐扫清了障碍，找到了入门的钥匙。我开始明白如何去学习，如何去实践，如何去深挖每一个核心知识点。

我撰写了这个系列的文章，**希望能将这段经历和学习的心得分享给更多想要入门人工智能的朋友们**。这些文章将详细记录我学习人工智能的每一个步骤和心得，希望通过我的经验，为大家提供一份实用的入门指南，帮助大家更快地融入这个充满机遇和挑战的领域。

“**万事开头难**”是一句广为流传的谚语，意指无论做任何事情，最初的时候总是最困难的。但是！“**天下事有难易乎?为之,则难者亦易矣**”

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/931b3c9ddac34a5782e2f485cf36efde.png)

## 2.编程环境

人工智能相关的软件开发和单片机软件开发不同，单片机软件开发只需要安装一个集成开发软件就可以了，例如KEIL或者IAR。而人工智能软件开发则需要安装编程软件，配置编程环境，同时还要根据实际情况添加一些软件工具。**因此想要入门人工智能的第一个拦路虎就是编程环境的搭建**。

笔者是一名单片机工程师，人工智能相关的软件开发与单片机相关的软件开发之间存在显著的差异。单片机软件开发通常较为直接，主要围绕一个集成开发环境（IDE）进行，**如KEIL或IAR，这些软件为开发者提供了编写、编译和调试单片机程序的一站式服务**。然而，人工智能软件开发则是一项更为复杂且多层次的任务。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/604183c95a944bd8b1b56da88f11f758.png)

人工智能软件的开发不仅要求安装专业的编程软件，如Python的IDLE、Jupyter Notebook等，还需要根据项目的需求，配置相应的编程环境，如安装各种库和框架，如TensorFlow、PyTorch、OpenAI等。这些库和框架为开发者提供了构建、训练和部署机器学习模型所需的各种工具和算法。除了编程软件和环境的配置，人工智能软件开发还常常需要添加一些辅助的软件工具，如数据可视化工具（如Matplotlib、Seaborn）、模型优化工具（如TensorBoard）等。

因此，**对于想要入门人工智能领域的开发者来说，搭建一个合适的编程环境无疑是我们面临的首要挑战**。在搭建编程环境的过程中，我们可能会遇到各种问题和挑战。例如，软件安装失败、环境配置错误、版本冲突等。这些问题需要开发者具备耐心和毅力，通过查阅文档、搜索网络、寻求帮助等方式逐一解决。
我们的编程环境如下：

> python 3.12.2 
> ancand 2.5.2 
> jupyter 7.0.8 
> pandas 2.2.1 
> numpy 1.26.4 
> keras  3.3.3

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/fec54014c7f746f097943122bb52ed5c.png)

## 3.编程环境搭建

**编程环境的核心是一个安装有人工智能相关工具包的Python编程环境**。构建开发环境主要有以下两个主要步骤：

**步骤1**：安装Python，这是整个编程环境的基础。Python是一种高级编程语言，其简洁的语法、强大的库支持和广泛的应用领域使其成为AI开发的理想选择。

**步骤2**：安装一系列与人工智能开发紧密相关的工具包，也称为库或框架。这些工具包提供了丰富的算法、模型和实用工具，使我们能够更高效地开发AI应用程序。一些常见的AI工具包包括NumPy（用于数值计算）、Pandas（用于数据处理和分析）、Matplotlib（用于数据可视化）、TensorFlow（用于深度学习）和scikit-learn（用于机器学习）。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/cefb65c5372b475e91963d274c996930.png)


### 3.1安装pythoh编程环境

#### 安装pythoh

**下载python安装包**。进入官网下载与自己电脑系统相匹配的python安装包。

> python官网：https://www.python.org

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/9dfa86b68b2341b3a5fc13db80f51dc2.png)

**安装python**。点击python安装包开始安装，安装时需要勾选Add python to PATH，其他步骤使用默认选项直接“下一步”。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/12c05b08ee0b42ceb023e8e71d64e94e.png)

**测试python**。完成安装后打开命令行工具（WIN+R 输入cmd），在命令行工具输入 

```c
python -V
```

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/bf3fba18f7bd477a8228aef2585f4702.png)


如果python正确安装，命令行工具会返回python的版本号。

**编程环境搭建情况：已经完成30%的搭建工作，目前编程环境已经支持python编程**。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/fb99e975e9f94129a9a18bfe71e8c899.png)

#### 安装Anaconda

Anaconda是一个开源的Python发行版本，它不仅仅包含了Python解释器，还集成了大量的科学计算包、库、管理工具等，为数据科学、机器学习等领域的科研人员和工程师提供了便捷的工作环境。ANACONDA有以下四大作用：

> 1、工具包管理。ANACONDA自带了Conda这个强大的包管理工具，可以方便地安装、更新、卸载Python包及其依赖项。
> 2、虚拟环境管理。ANACONDA可以轻松创建和管理多个Python虚拟环境，每个环境可以有不同的Python版本和包依赖，从而满足不同的项目需求。
> 3、数据科学工具。ANACONDA自带了许多常用的数据科学工具，如Jupyter
> Notebook、Spyder等，这些工具为数据分析和可视化提供了强大的支持。
> 4、丰富的工具包。ANACONDA包含了超过180多个科学包，如NumPy、Pandas等，这些包在数据清洗、统计分析、机器学习等方面具有广泛的应用。

**下载Anaconda安装包**。进入官网下载与自己电脑系统相匹配的Anaconda安装包。

> Anaconda官网：https://www.anaconda.com

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/54c26eca3df64ef4b21936382f791891.png)

**安装Anaconda**。点击Anaconda安装包开始安装，使用默认选择进行安装。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/11b6888ff5ea47a9b3d07e00b145c67a.png)


**创建一个虚拟环境**。打开Anaconda点击Environments,点击base选择Open Terminal。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/37847f8750f248f0ab56cf30b2d67282.png)


在终端中输入指令建立自定义环境，env_ai  为自定义环境名，运行该命令后在随后输入的提示符中输入 y 

```c
conda create -n env_ai  
```

 

在终端中输入激活自定义环境

```c
conda activate anv_ai
```

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/f870fc4611764fe8a3e74653ac7e5416.png)

**编程环境搭建情况：已经完成50%的搭建工作，目前编程环境是一个支持python编程，支持便捷安装多种应用库和工具，支持创建管理多个python虚拟环境**。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/5c959538d841466083e357071a8f3669.png)

#### 安装Jupyter Notebook

**Jupyter Notebook是一个功能强大的交互式笔记本，它为用户提供了在Web浏览器中编写、执行和共享文档的能力**。这些文档可以包含代码、可视化和文本，可以为开发者等提供了极大的便利。
**安装Jupyter Notebook**。打开Anaconda，点击home ，找到jupyter,点击install完成安装。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/1e587ca555954cbb91563f400c38f480.png)

**启动Jupyter Notebook**。打开Anaconda点击Environments,点击env_ai选择Open with jupyter notebook

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/7b31e59e435a40d8beaf3207b1368755.png)

浏览器自动打开了juoyter ,我们可以选择new建立一个文件夹或者一个Notebook

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/bb844ad80e0846eb80af286218ead122.png)

在jupyter中新建一个Notebook文件，打开Notebook文件，我们可以在Notebook中写文档，写代码，调试运行代码。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/edecff335c604fef81cd2672bd9cdf08.png)

**编程环境搭建情况：已经完成70%的搭建工作，目前编程环境是一个支持python编程，支持便捷安装多种应用库和工具，支持创建管理多个python虚拟环境，同时还可以灵活便捷的编辑和调试代码**。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/6524b2e4444245b38e018dc8aa82817f.png)

#### 3.2安装工具包

到这里一步可以说我们的环境基本搭建好了，接下来我们需要安装一些和人工智能相关的工具包，如NumPy、Pandas、scikit-learn、keras等，这些包在数据清洗、统计分析、机器学习等方面具有广泛的应用。工具包相当于一个库文件，我们安装了工具包就可以调用其中的各种函数方法。

打开Anaconda点击Environments,点击env_ai选择Open Terminal。我们在终端中用pip指令来安装工具包。例如我们安装pandas 就在终端中输入 

```c
pip install pandas
```

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/f59dd9831e844d21b475d84dc66453c8.png)

这种直接安装的方式默认是用的是国外的下载源，下载速度很慢，经常会出现下载失败的情况，因此我们使用国内的下载源进行下载，大家可以在网上搜素“**pip国内源**",笔者使用的是清华大学下载源，因此我们将安装pandas安装指令改为如下形式：

```c
pip install pandas -i https://pypi.tuna.tsinghua.edu.cn/simple/
```


这样就和迅速的安装好了pandas工具包。在这里我们直接将后续可能用到的工具包一次性安装完，安装指令如下：

```c
pip install matplotlib -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install openpyxl -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install Certificates -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install opencv-python -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install keras -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install tensorflow  -i https://pypi.tuna.tsinghua.edu.cn/simple/
pip install requests -i https://pypi.tuna.tsinghua.edu.cn/simple/
```

**编程环境搭建情况：已经完成100%的搭建工作，目前编程环境是一个支持python编程，支持便捷安装多种应用库和工具，支持创建管理多个python虚拟环境，同时还可以灵活便捷的编辑和调试代码，此时我们的编程环境还支持各种人工智能算法的工具包**。

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/50b5f5ae37514941bec8333b986fbace.png)

**大功告成！至此我们的编程环境已经搭建好了！人工智能我来了！**

![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/c4db15e0f1ba4fbdbc9c85bbe349d7b3.png)


## 4.编写第一个程序

打开在jupyter中新建一个Notebook文件，我们先建立一个Markdown的cell ，写一个程序说明。
![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/c176e5767321414a88c334ef7e461ed1.png)


建立一个Code的cell ，写一个python程序并运行，代码和运行结果如下：

```c
from matplotlib import pyplot as plt
x = [1,2,3,4,5,6]
y = [11,12,13,14,15,16]
plt.figure(figsize = (2,2))
plt.scatter(x,y)
plt.show()
```
![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/ab4500c5be27422a9da9c6471b70c6b6.png)

![在这里插入图片描述](https://img-blog.csdnimg.cn/1ce5585ea26f4b5a99f057ad19a8816a.png#pic_center)

