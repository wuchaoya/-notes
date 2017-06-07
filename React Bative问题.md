<center>React Native问题及其解决方法</center>

### `$ react-native run-android `
__error：__
```shell

error: could not install *smartsocket* listener: cannot bind to 127.0.0.1:5037: 通常每个套接字地址(协议/网络地址/端口)只允许使用一次。 (10048)
```
__ resolve：__
检查电脑是否开启了手机助手，将其关闭
__error:__
```shell

Unzipping C:\Users\Administrator\.gradle\wrapper\dists\gradle-2.14.1-all\8bnwg5hd3w55iofp58khbp6yv\gradle-2.14.1-all.zip to C:\Users\Administrator\.gradle\wrapper\dists\gradle-2.14.1-all\8bnwg5hd3w55iofp58khbp6yv
Exception in thread "main" java.util.zip.ZipException: error in opening zip file
```
__resolve:__
删除`C:\Users\Administrator\.gradle\wrapper\dists`的`gradle-2.4-all`文件夹，重新执行初始命令,或者去网上下载http://pan.baidu.com/s/1b2Vb2Y包，放在C:\Users\xxxx\.gradle\wrapper\dists\gradle-2.4-all下，重新运行

__打包安装完成，服务断开__

使用安卓5.0以上进行调试
