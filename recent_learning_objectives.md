学习 Markdown 语法

ide rename goland 下

zendstdio功能学习

elasticsearch 学习

goroutine调度器原理，p的作用，抢占过程
chan原理，从写入到读取的整个过程，内部发生了是么
锁的原理，自旋、饥饿模式
k8s cni网络插件原理，从外部访问某个pod，中间经过了什么
从podA访问podB网络如何转发，访问一个service时，如何到的目的地pod
k8s ipvs工作原理
k8s scheduler调度器原理，如何自定义调度器，内部如何工作
k8s 探针有哪几种，如何工作的


1、任何情况下禁止使用cgo, 这个也需要在编译中，把cgo指令禁用

2、如果在特殊情况下使用goroutine，必须在每个goroutine中实现recover，没有特殊情况，不要使用go func(), 我们一般做业务，也很少用到， 任何位置的recover需要打入panic日志

3、尽量避免使用没有条件的for,  比如 for { }， 如果里面流程处理出错，可能会导致大量goroutine空转cpu和goroutine泄露，历史上曾经出现过因为这个导致整个集群崩溃的P0故障，虽然现在不会导致崩溃了，但是尽量避免或谨慎使用

4、消费者在任何情况下不要close(chan)

5、谨慎使用类型断言，如使用，要加是否成功判断或使用switch case，不得使用 v := interface.(type)

6、禁止使用unsafe.Pointer，反射时可以例外，除非所有人都能整明白unsafe.Pointer


编程规范奔着追求代码简洁，并具有可读性的目标去制定，遵循标准库的规范及静态代码检查工具Golangci-lint规则制定。

Golangci-lint

git地址：https://github.com/golangci/golangci-lint

官方文档:https://golangci-lint.run/usage/quick-start/

go语言李文周学习博客 https://www.liwenzhou.com/archives/
=======
专业计算机术语翻译网站 http://www.deepl.com/zh/translator

godoc命令可以查看项目中所有包的文档，包括go官方的，第三方引入的和自己写的,go get golang.org/x/tools/cmd/godoc 之后执行godoc -http://6060

阅读《go专家编程》

visualdesigner 流程图制作软件

git stash暂时保存命令

git cheeckout . 可以放弃啊之前没有add过的修改

fastdfs 分布式文件系统
