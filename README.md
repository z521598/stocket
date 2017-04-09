# 计算机网络课程设计
## 指导教师：朱建启老师
## 小组成员：郎世权(55140115)，祝嘉(55140116)，李政辉(55140111)
## 实验环境：Mac OS ＋ IDEA
## 实现技术：Java : Socket + IO + Thread
## 代码仓库：https://github.com/z521598/stocket
### 总述：
> Java Socket 提供了4个API的类,我们使用了其中2个类  
> ServerSocket用于构建服务端,用accept()方法可以接受连接  
> Socket用于构建客户端  
> com.baidu.comon.Var类里面有一些静态变量，用于跨机器调试方便  
### 题目一：Windows平台上简单的客户机端和服务器端的套接字编程
** 服务端搭建:  
>1.a)创建一个服务器端Socket  
>  b)指定绑定的端口，并监听此端口  
>2.创建一个ServerSocket在端口XX监听客户请求  
>3.调用accept()方法开始监听，等待客户端的连接  
>4.获取输入流，并读取客户端信息  
>5.由Socket对象得到输入流，并构造相应的BufferedReader对象  
>6.由Socket对象得到输出流，并构造PrintWriter对象  
>7.while(){}循环,当输入为0时候，就跳出循环  
>8.向"客户端"发送消息,向客户端输出字符串,刷新输出流，使Client马上收到该字符串  
>9.阻塞，监听，等待"客户端"信息  
>10.重复8-9直到输入0结束  
>11.关闭连接，释放资源。  
** 客户端  
>1.创建客户端Socket，指定服务器地址和端口  
>2.类似服务端的获取输入流和输出流  
>3.while循环和服务端类似  
>4.关闭资源  
### 题目二：Linux或Windows平台上多线程、多进程或异步I/O的套接字编程
### 题目三：原始套接字编程
### 题目四：FTP应用编程
