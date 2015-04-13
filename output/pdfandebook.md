输出PDF
====
输出pdf文件步骤如下:

1. 由于生成PDF文件依赖于`ebook-convert`，故首先在该处[ebook-convert下载链接](http://calibre-ebook.com/download)点击下载所需要的版本，安装即可;
2. 打开cmd，进入E:\gitbook目录;
3. E:\gitbook>gitbook pdf gitbook-studying gitbook-studying/gitbook入门教程.pdf
4. 则在目录E:\gitbook\gitbook-studying下生成了该pdf文件



然后，你会发现你的目录里多了一个名为`gitbook入门教程.pdf`的文件，就是它了！

但是，笔者在测试的时候发现，生成的PDF文件在排版上不是合理，如页面的边距明显过小，如果是图文混排的话，整个版面感觉有些零乱。



