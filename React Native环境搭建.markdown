<center>ReactNative开发环境搭建</center>
--------------------------------------------
- [x] Node
- [x]Python
- [x]JDK
- [x]Android SDK
- [x]visual studio 2015
- [ ]模拟器(可选)

> - 把所不相关的软件都设置为非开机启动，特别是国产杀毒软件，卫士之类软件。然后重新启动系统
- 安装过程和使用过程中如果有防火墙提示，都点击允许访问。如果有权限提示，都点击是或者确定。

### 安装基本工具

__安装Python__
> - 注意目前不支持Python 3版本。

1. 安装Python,点击Next，选装安装目录，如下图所示：

  <!-- ![Python安装步骤1](./img/Python1.jpg)

  ![Python安装步骤2](./img/Python2.jpg) -->

2. 选择下图所示选项，环境变量自动配置。

  <!-- ![Python安装步骤3](./img/Python3.jpg) -->
3. 在命令提示符中输入：python，验证是否安装成功，如果成功即如下图所示，若提示是无效的命令，重启计算机，再输入python验证。  

__安装Java SDK__
- [下载地址](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

- Java Development Kit
- 这是做java语言运行开发所依赖的工具，就像js语言运行需要浏览器一样
- 环境变量: javascript
- 环境变量配置:
  + JAVA_HOME,变量值配置为:jdk安装路径(c:/xxx/jdk1.8.0.25)
  + CLASSPATH,变量值配置为:

  .;%JAVA_HOME%\lib\dt.jar;%JAVA_HOME%\lib\tools.jar;

  *注意最前面有个点*
  + PATH,变量值追加:    %JAVA_HOME%\bin;

- 输入javac较验
- 或输入java -version


__安装Node__
> - 安装完node后建议设置npm镜像以加速后面的过程（或使用科学上网工具）。注意：不要使用cnpm！cnpm安装的模块路径比较奇怪，packager不能正常识别！
> -  目前已知Node 7.1版本在windows上无法正常工作，请避开这个版本！

1. 下载安装nvm

  [nvm Windows下载地址](https://github.com/coreybutler/nvm-windows/releases)

  <!-- ![nvm](./img/nvm1.png) -->

  程序安装过程中，在 Set Node.js Symlink 这一步目录设置，是待会 nvm use 存放你的 nodejs程序的目录 [C:\\DevTools\\nodejs]。

  ```shell

  nvm v // 查看版本 => 1.1.1
  nvm install latest // 下载最新的 node 版本 v7.2.0
  nvm install 4.4.4 // 安装不同版本
  nvm install 6.2.0 32 // 默认是64位，32位需指定
  nvm uninstall 6.2.0 #卸载对应的版本
  ```
  下载完成后，会在 \nvm 文件夹下多个 v7.2.0 文件夹。

  ```shell

  nvm use 4.4.4 // 引入使用
  nvm ls //查看已下载的版本
  ```

2. 安装好nvm就可以利用nvm安装任意版本的node了

__安装Android Studio__

  参照 [ReactNative 文档安装](http://reactnative.cn/docs/0.44/getting-started.html)

__安装Visual studio__
> - 这个东西太大，如果用u盘重其他地方copy,出现文件太大无法复制,将u盘格式化为NTFS

- 主要是为了使用该工具所提供的C++环境
- 这是个终极大Boss
- 安装所需时间30分钟到2小时不等，甚至更长(取决于电脑性能)。
- 傻瓜式的点就行了
