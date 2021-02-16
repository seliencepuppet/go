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
