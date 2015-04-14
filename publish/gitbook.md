发布到Gitbook.com
==
[GitBook.com](gitbook.com) 是一个围绕 gitbook 发行书籍的社区，于 2014 年初创，GitBook.com 提供免费和付费的服务，而且免费账户就可以享受诸多服务,这里，我们将编写的gitbook书籍发布到Gitbook个人账户里。

登陆 [GitBook.com](gitbook.com) 后,在用户页面，点击create a new book后,如下图所示：

![](../imgs/create_gitbook.png)

创建的书籍，title:`gitbook入门教程`,name为`gitbook-studying`
则创建后的Gitbook线上仓库地址为`https://git.gitbook.com/yuzeshan/gitbook-studying.git`(当然，也可以打开书籍settings查看)

这样，gitbook.com线上的仓库就建好了，由于GitBook.com 上的每本书都使用 Git 项目来管理，所以，事先写好的书籍就可以通过git提交上去，具体步骤如下：

 1. 首先打开cmd，进入书籍目录，E:\gitbook\gitbook-studying;
 2. 运行E:\gitbook\gitbook-studying>`git init`，这里如果git提示错误，则是没配置git的环境变量的path；
 3. 将目录的章节文件夹一个个加进，git里，使用`git add 文件夹名`;
 4. 接下来，`git commit -m "提交信息(必填，否则出错)"`;
 5. 然后，将本地的git 仓库与gitbook.com上远程仓库连接，`git remote add gitbook https://git.gitbook.com/yuzeshan/gitbook-studying.git`(注意:不是github上的git remote add origin git@....);
 6. 最后，将本地仓库全部push到远程，`git push -u gitbook maste`r，以后每次更改，然后add再commit，而第二次push时，直接`git push gitbook master`即可


提交到 GitBook.com 后，书籍就自动发布了，用户就可以通过书籍的地址访问了，例如：<http://yuzeshan.gitbooks.io/gitbook-studying/content/>

**ps:如果本地没有git初始化过得仓库，则可以将在线建立的仓库，克隆到本地，进行修改，提交，push，简洁步骤如下:**

- 首先进入想要建立书籍的目录，这里是E:\gitbook\gitbook-studying；
- 运行命令`git clone https://git.gitbook.com/yuzeshan/gitbook-studying.git`;
- 然后，通过之前介绍的书籍编辑:gitbook init,gitbook serve 等方法，编辑好书籍后，再用git命令add commit添加提交书籍目录文件；
- 最后，`git push gitbook master`即可。


