# beego-demo

## 环境变量

| 变量名        | 含义           | 
| :------------- |:-------------|
| `$GOROOT`     | 表示`Go`在你的电脑上的安装位置，它的值一般都是 `$HOME/go`，当然，你也可以安装在别的地方 | 
| `$GOARCH`       |  表示目标机器的处理器架构，它的值可以是 `386`、`amd64`或`arm`    |   
| `$GOBIN`  | 表示编译器和链接器的安装位置，默认是`$GOROOT/bin`，如果你使用的是`Go 1.0.3` 及以后的版本，一般情况下你可以将它的值设置为空，`Go`将会使用前面提到的默认值      |    
| `$GOPATH`  | 默认采用和`$GOROOT`一样的值，但从`Go 1.1`版本开始，你必须修改为其它路径。它可以包含多个包含`Go` 语言源码文件、包文件和可执行文件的路径，而这些路径下又必须分别包含三个规定的目录：`src`、`pkg` 和 `bin`，这三个目录分别用于存放源码文件、包文件和可执行文件      | 
| `$GOARM`  | 专门针对基于 arm 架构的处理器，它的值可以是 5 或 6，默认为 6      | 
| `$GOMAXPROCS `  | 用于设置应用程序可使用的处理器个数与核数     | 


## GOPATH

`GOPATH`环境变量指定了你的工作空间位置。它或许是你在开发`Go`代码时，唯一需要设置的环境变量。注意，它绝对不能和你的`Go`安装目录相同。

### Windows下设置环境变量名

如果想查看和`Go`相关的环境变量,输入

```javascript
go env

```

以下是在Git上看到的数据

```javascript
set GOARCH=amd64
set GOBIN=
set GOEXE=.exe
set GOHOSTARCH=amd64
set GOHOSTOS=windows
set GOOS=windows
set GOPATH=
set GORACE=
set GOROOT=E:\Go
set GOTOOLDIR=E:\Go\pkg\tool\windows_amd64
set CC=gcc
set GOGCCFLAGS=-m64 -mthreads -fmessage-length=0
set CXX=g++
set CGO_ENABLED=1
```

>提示: 注意`CMD`中查看的`Go`环境变量可能和`Git`上的有所不同,是因为在设置环境变量的时候只设置了**系统变量**而没有设置**用户变量**,建议两者都设置上,否则之后无法使用`go get`命令去获取`github`上的远程包.


### win7下设置环境变量

控制面板 -> 系统 -> 高级系统设置 -> 环境变量 -> 设置`GOPATH`并设置`PATH`
关于这两个环境变量如何配置,以及如何创建`GOPATH`环境变量指定的工作空间位置,请查看官方文档(如何使用Go编程)[http://docscn.studygolang.com/doc/code.html]







## 链接

- (Go中文官方)[http://docscn.studygolang.com/]



