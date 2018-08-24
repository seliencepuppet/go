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

func main(){
    fmt.Printf("hello world!\n")
}
```
