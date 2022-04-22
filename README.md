# JNO-Proposal-Author-Kit-LaTex
联合现在提案文件的 LaTex 版本，在 [WACV 2023 Author Kit](https://github.com/wacv-pcs/WACV-2023-Author-Kit) 基础上的编辑与增加，主要对其增加目录和页头和 CTEX 的支持，具有中文排版的功能。

## 本地构建
如果想本地构建 LaTex，那么请确保您安装了完整的 LaTex 环境以及具有相应的写作工具，如果具有，那么您可以在需要的工作目录下执行
- 克隆我们的存储库

```ssh
git clone https://github.com/jn-un/JNO-Proposal-Author-Kit-LaTex.git
```

当然你也可以点击 [main.zip](http://www.github.com/jn-un/JNO-Proposal-Author-Kit-LaTex/archive/refs/heads/main.zip) 来直接获取到 main.zip 文件。

## 模板使用
### 编译
在编译的过程中，我们建议直接使用 ```latexmk -pdf egpaper.tex``` 来进行构建，而不是通过编译器自带的编译进行运行，这有可能会出现错误（如果您有解决方案，欢迎提交 Pr）。

在编译的过程中，很有可能出现参考文献、目录等无法显示等问题，或显示乱码，此时只需要多运行几次 ```latexmk -pdf egpaper.tex``` 即可。当然也可以通过使用 [LaTex 手册](https://ftp.yz.yamagata-u.ac.jp/pub/CTAN/info/lshort/chinese/lshort-zh-cn.pdf) 中的解决方案来进行解决。


### 使用
在第一次编译成功的时候，会在本地出现 pdf 文件，阅读即可查看 WACV 2023 和我们追加的相关编写指引。同样的也会在 ```egpaper.tex``` 中增加了些许编码注释，可以阅读注释来快速理解 LaTex 的基础语法使用。

对于参考文献的修改，可以对 ```egbib.bib``` 文件进行追加或增减修改等操作，最终参考 .tex 文件中的注释来理解详细的使用方法。 