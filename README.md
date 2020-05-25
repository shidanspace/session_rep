
# Session控制器 客户端
因编写时未连外网，上传为压缩包，解压后运行


实现一个Session控制器(实现client端)。这里的Session 可以想象为一些有时间长度的会话请求。会话起停需要通过向服务器提供的http 接口发送请求来控制。
具体要求如下：
*	根据接口描述和协议类型发送 session start/stop请求给服务端
*	可支持同时(向同一个server)并发发送多个请求
*	Stop请求需要根据session 时长来发送
*	创建日志来记录session 状态 (发送时间,发送url,和body,结果,连接信息)


* 支持异步
* 支持动态调整并发参数



## 使用指南


### 环境

* JAVA JDK 1.8

### 运行步骤

1. 导入Maven项目
2. 运行服务端：SessionServer下的SessionServerApplication类
3. 运行客户端：SessionClient下的Main类

## 配置方法

application.properties可配置属性
* durTime 持续时间
* threadNum 启动的线程数
* async 是否采用异步 1:是 0:否

## 其他
见各下注释文件
