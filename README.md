# libev
libev with comment

## 编译libev
* ./configure
* make
* sudo make install

## 源码结构
libev的源码结构非常清晰，代码量也很少，主要包括以下几个文件：
* ev_select：对select的封装
* ev_poll：对poll的封装
* ev_epoll：对epoll的封装
* ev_port：对solaris event port的封装
* ev_kqueue：对kqueue的封装
以上几个是不同平台多路复用的后端接口的封装
* ev：对事件框架的全部
* event：提供了兼容libevent接口的封装
* ev++：提供了C++接口
* ev_win32：对Windows的封装
* ev_vars：定义了事件循环的变量

## 参考
这里有一篇关于libev的分析，写的非常好，赞。[链接](http://blog.chinaunix.net/uid-28458801-id-4463801.html)
