gitbook命令行&markdown编辑
====
##1. 首先介绍下一本书的主要文件：
### README.md

这个文件相当于一本Gitbook的简介，最上层(和SUMMARY.md同级)的是本书的Introduction。

### SUMMARY.md()

这个文件是一本书的目录结构，使用Markdown语法， 这个文件在使用gitbook命令行之前要先写好，以便之后生成书籍目录,如我们这本书的`SUMMARY.md`：

```
* [基本安装](howtouse/README.md)
 - [Node.js安装](howtouse/Nodejsinstall.md)
 - [Gitbook安装](howtouse/gitbookinstall.md)
 - [Gitbook命令行速览](howtouse/gitbookcli.md)
* [图书编辑](book/README.md)
 - [gitbook命令行&markdown编辑](book/gitbook-cli.md)
 - [gitbook editor编辑](book/editor.md)
* [图书输出](output/README.md)
 - [输出为静态网站](output/outfile.md)
 - [输出PDF](output/pdfandebook.md)
* [发布](publish/README.md)
  - [发布到gitbook.com](publish/gitbook.md)
  - [Github集成](publish/github.md)
  - [发布到Github Pages](publish/gitpages.md)
* [结束](end/README.md)


```

列表加链接，链接中可以使用目录，也可以不必使用。

##2. 书籍目录初始化&内容编写

当这个目录文件创建好之后，我们可以使用Gitbook的命令行工具将这个目录结构生成相应的目录及文件,步骤如下：


- 打开cmd,cd命令进入创建的存书籍的目录，如:E:\gitbook\gitbook-studying;
- 在这个目录下我们创建了上述的SUMMARY.md文件;
- 然后使用命令gitbook init,则生成一系列目录文件，见下方；


```
$ gitbook init
$ ls
LICENSE    SUMMARY.md book       output
README.md      howtouse   publish
$ tree .
.
├── LICENSE
├── README.md
├── SUMMARY.md
├── book
│   ├── README.md
│   ├── gitbook-cli.md
│   └── editor.md
├── howtouse
│   ├── Nodejsinstall.md
│   ├── README.md
│   ├── gitbookcli.md
│   └── gitbookinstall.md
├── output
│   ├── README.md
│   ├── outfile.md
│   └── pdfandebook.md
└── publish
    ├── README.md
	├── gitbook.md
	├── github.md
    └── gitpages.md
```

我们可以看到，gitbook给我们生成了与`SUMMARY.md`所对应的目录及文件。

每个目录中，都有一个`README.md`文件，相当于一章的说明。

最后，我们在对应目录中用markdown编辑器(这里推荐使用markdownpad)编辑自己想要的内容即可.
