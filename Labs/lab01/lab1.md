### -1 环境

首先确保你有可以正常访问 GitHub, Google 等的网络环境。

如果你在这步出现了问题，请私聊。（但想看见这个md不就需要科学么？）



### 0. Git lab

这个 lab 是本次课程的基础。你需要：

#### 配置 ssh_key (可选)

这个在互联网上已经有足够多的资源了，请自行 STFW。

> [!NOTE]
>
> Github 现在已经几乎不能使用 密码 来进行身份验证，所以我们推荐你配置 ssh_key

#### Clone 仓库

尝试使用 git clone 克隆下来学习仓库

> [!IMPORTANT]
>
> 如果你发现 git clone 的时候出现了网络错误，请 STFW 或者直接问 GPT，为你的 Git 配置代理服务（我们假设你已经完成了 TASK -1）。

#### 配置 Git

配置你本地 Git, 告诉 Git 你的用户信息

```bash
git config --global user.name "xx"
git config --global user.email xx@example.com

```

#### 查看仓库基础信息

尝试分别输入下面内容

```bash
git remote -v
git status
git log
```

思考这些命令告诉了你什么信息



#### 链接你自己的远程仓库（可选）

如果你有需求要把仓库放在 GitHub 上（比如你有多个电脑等等），你需要自己添加一个远程仓库，使用 git remote add 来添加远程仓库，具体使用可以 STFW 。

这样，你就有2个远程仓库了，一个是我们的发布页你可以用来 pull 我们更新的代码，一个是你自己的远程仓库。

> [!TIP]
>
> 思考下到目前为止你 仓库 的结构是怎么样的

#### Git 使用

尝试随便写点东西，练习如何提交，如何回退到某个提交等等。正如讲义所说，你可以根据需求学习使用。但一定记得，尽可能原子化的提交会减少你未来的悔恨。

### 1. C 练习

打开我们的仓库目录，在 Labs/lab01/C_TASK 中是我们这次的 C 练习。

这次只是让你初步尝试 GCC 的使用，让你自己可以跑起这个程序。

> [!TIP]
>
> 你可以使用 tree 命令查看 C_TASK 的结构。

> [!IMPORTANT]
>
> 参考手册，讲义和自行查阅资料，使用 GCC , 让这个程序跑起来。
>
> 这只是一个非常简单的程序，无论你有没有基础，你都可以自己去想一下，程序从哪里开始执行的？（当然，我们还是保留质疑）

#### 拓展练习

我们在讲义中提到了 Makefile, 如果你觉得这次 Lab 很无聊，可以尝试学习下 怎么编写 Makefile, 让这个程序更加优雅地跑起来，当然，你也可以随意添加自己的功能。