# go

<br/>

Go是Google在2009年发布的编程语言

学习Go语言的理由相当充分
1) Go语言的设计哲学是大道至简, Go语言的语法是非常简约的, Go语言非常容易学习
2) Go语言是编译型的语言, 而且是跨平台的. Go语言在发布时不需要依赖或需要很少的依赖
3) Go语言对并行支持非常好, Go语言非常适合开发服务端程序. Erlang从语言易用性, 并行支持, 编译或解释型综合指标, Go语言是最高的
4) Go语言支持非侵入式接口.

```go
interface MyInterface{
    void method();
}

class MyClass implements MyInterface {
    void method(){
    
    }
}
```

阿里, 百度, 腾讯, 京东, 亚马逊, 都在尝试使用Go语言作服务端的应用

docket(虚拟化平台), go 语言本身也是用go语言开发

知识点
1) go语言代码的第1行必须声明包
2) 入口的go语言代码 (包含main函数的代码文件) 的包必须是main否则运行go程序会显示 go run: cannot run non-main package

```go
package main
import "fmt"

func main() {
    fmt.Printf("hello world!\n")
}
```
3) 左花括号 {} 不能独自在一行, 必须和其他代码在一行
4) 导入 Go Library 需要用import指令
5) Go语言规定, 所有导出的函数名称的首字母必须大写. fmt.Printf("hello world!\n")


| 命令行的使用方法        | 产生的作用                  |
|------------------------|----------------------------|
| go run helloworld.go   | 使用该命令可以直接执行go程序 |
| go build helloworld.go | 使用该命令之后会产生编译好的二进制文件可以直接执行并运行 |


go在国内的代理网站 - https://goproxy.cn

go语言解释器下载网站 - https://golang.google.cn/


设置 go module

```cmd
C:\Users\Administrator>
C:\Users\Administrator>go env -w GO111MODULE=on

C:\Users\Administrator>go env
set GO111MODULE=on
set GOARCH=amd64
set GOBIN=
set GOCACHE=C:\Users\Administrator\AppData\Local\go-build
set GOENV=C:\Users\Administrator\AppData\Roaming\go\env
set GOEXE=.exe
set GOFLAGS=
set GOHOSTARCH=amd64
set GOHOSTOS=windows
set GOINSECURE=
set GOMODCACHE=C:\Users\Administrator\go\pkg\mod
set GONOPROXY=
set GONOSUMDB=
set GOOS=windows
set GOPATH=C:\Users\Administrator\go
set GOPRIVATE=
set GOPROXY=https://proxy.golang.org,direct
set GOROOT=E:\GOLANG
set GOSUMDB=sum.golang.org
set GOTMPDIR=
set GOTOOLDIR=E:\GOLANG\pkg\tool\windows_amd64
set GCCGO=gccgo
set AR=ar
set CC=gcc
set CXX=g++
set CGO_ENABLED=1
set GOMOD=NUL
set CGO_CFLAGS=-g -O2
set CGO_CPPFLAGS=
set CGO_CXXFLAGS=-g -O2
set CGO_FFLAGS=-g -O2
set CGO_LDFLAGS=-g -O2
set PKG_CONFIG=pkg-config
set GOGCCFLAGS=-m64 -mthreads -fno-caret-diagnostics -Qunused-arguments -fmessage-length=0 -fdebug-prefix-map=C:\Users\ADMI
hes

C:\Users\Administrator>
```

设置 go proxy 

```cmd
C:\Users\Administrator>go env -w GOPROXY=https://goproxy.cn,direct

C:\Users\Administrator>go env
set GO111MODULE=on
set GOARCH=amd64
set GOBIN=
set GOCACHE=C:\Users\Administrator\AppData\Local\go-build
set GOENV=C:\Users\Administrator\AppData\Roaming\go\env
set GOEXE=.exe
set GOFLAGS=
set GOHOSTARCH=amd64
set GOHOSTOS=windows
set GOINSECURE=
set GOMODCACHE=C:\Users\Administrator\go\pkg\mod
set GONOPROXY=
set GONOSUMDB=
set GOOS=windows
set GOPATH=C:\Users\Administrator\go
set GOPRIVATE=
set GOPROXY=https://goproxy.cn,direct
set GOROOT=E:\GOLANG
set GOSUMDB=sum.golang.org
set GOTMPDIR=
set GOTOOLDIR=E:\GOLANG\pkg\tool\windows_amd64
set GCCGO=gccgo
set AR=ar
set CC=gcc
set CXX=g++
set CGO_ENABLED=1
set GOMOD=NUL
set CGO_CFLAGS=-g -O2
set CGO_CPPFLAGS=
set CGO_CXXFLAGS=-g -O2
set CGO_FFLAGS=-g -O2
set CGO_LDFLAGS=-g -O2
set PKG_CONFIG=pkg-config
set GOGCCFLAGS=-m64 -mthreads -fno-caret-diagnostics -Qunused-arguments -fmessage-length=0 -fdebug-prefix-map=C:\Users\ADMINI~1\AppData\Local\Temp\go-build581816714=/tmp/go-build -gno-record-gcc-switc
hes

C:\Users\Administrator>
```
