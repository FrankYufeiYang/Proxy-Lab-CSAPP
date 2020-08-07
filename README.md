# Proxy-Lab

## 背景
* 课程: System programming
* 教材: Computer Systems: A Programmer's Perspective (CSAPP)

## 语言
C

## 环境与使用
linux下给定的实验环境
* 创建 `cache.c`
* 添加code进 `proxy.c`
* 适配 `makefile`

## 实验目标
Part1: 实现一个代理服务器
* 接收客户端发出的请求
* 解析HTTP请求
* 响应请求并返回客户端

Part2: 实现代理服务器的多线程
* 利用 线程detach `pathread_detach()`，以此来确保线程结束时可以释放占用的资源

Part3: 实现代理服务器的缓存机制
* LRU
* 缓存web对象
* `读写者问题`---> 读者优先

## 调试
* 用telnet调试不安全的ssh以及非法的header
* 用cURL构建HTTP请求

## 总结
通过一项代理服务器的项目，我们既了解了客户端，也明白了服务器的工作原理，同时还需要结合之前所学的缓存与多线程技术。这个LAB也称得上是对整个课程的总结与融会贯通
