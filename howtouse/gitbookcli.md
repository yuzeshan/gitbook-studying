Gitbook命令行速览
====

Gitbook是一个命令行工具，使用方法(这里简单介绍)：

**本地预览**

```
C:\Users\lenovo> gitbook serve ./图书名称
```

**输出一个静态网站**

```
C:\Users\lenovo> gitbook build 图书目录 输出目录 
```

*注意:上面win下命令运行所处在的目录必须是写好的gitbook书籍目录前一个，
可以使用cd..切换，否则建立时会出错,后面会详细讲解*

**查看帮助**


`C:\Users\lenovo> gitbook help`

    build [book] [output]          build a book
    --format     Format to build to (Default is website; Values are website, jso
	n, ebook)
    --log        Minimum log level to display (Default is info; Values are debug
	, info, warn, error, disabled)

    pdf [book] [output]    build a book to pdf
    --log        Minimum log level to display (Default is info; Values are debug
    , info, warn, error, disabled)

    epub [book] [output]   build a book to epub
    --log        Minimum log level to display (Default is info; Values are debug
	, info, warn, error, disabled)

    mobi [book] [output]   build a book to mobi
    --log        Minimum log level to display (Default is info; Values are debug
	, info, warn, error, disabled)

    serve [book]   Build then serve a gitbook from a directory
    --port       Port for server to listen on (Default is 4000)
    --lrport     Port for livereload server to listen on (Default is 35729)
    --watch      Enable/disable file watcher (Default is true)
    --format     Format to build to (Default is website; Values are website, jso
	n, ebook)
    --log        Minimum log level to display (Default is info; Values are debug
	, info, warn, error, disabled)

    install [book]         install plugins dependencies

    init [directory]       create files and folders based on contents of SUMMARY.m
	d

