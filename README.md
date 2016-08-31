React Native Webstrom2016.2.2

环境搭建

软件安装
========

安装Java
--------

> 这里需要注意对环境变量的设置，可以根据java -version来检测一下，同时最好安装JDK1.8以上版本（原因待查）。

安装SDK
-------

> 这里需要注意设置环境变量ANDROID\_HOME：Android SDK Manager的位置 例如：（ANDROID\_HOME=&gt; E:\\Android\\sdk）设置环境变量PATH：例如：（PATH=&gt; %ANDROID\_HOME%\\tools;%ANDROID\_HOME%\\platform-tools）

### 下载地址

> https://dl.google.com/android/installer\_r24.4.1-windows.exe

### 设置SDK

#### 打开Andorid SDK Manager

**注：必须用管理员权限打开。否则会报错，提示无法访问该文件**。

#### 设置SDK. 选中以下项目

-   Android SDK Build-tools version 23.0.1

-   Android 6.0 (API 23)

-   Android Support Repository

-   Local Maven repository for Support Libraries(如图)

> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image1.png" width="418" height="315" /> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image2.png" width="418" height="140" />
>
> （注：上图中这些最好都选上，否则后面会出各种问题。）

#### 加速下载设置

1.  首先打开已下载的安卓SDK管理器“Android SDK Manager”，然后点击菜单栏中的“Tools”菜单选项，选择“Options”选项打开设置窗体。在设置窗体中勾选以Force开头的复选框按钮(关键步骤)，点击Close即可。

> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image3.png" width="452" height="322" />
>
> Server 和端口分别设置为。
>
> **大连东软信息学院镜像服务器地址:**
> **- [*http://mirrors.neusoft.edu.cn*](http://mirrors.neusoft.edu.cn/) 端口：80**（**推荐使用**）
> **北京化工大学镜像服务器地址:**
> - IPv4: [*http://ubuntu.buct.edu.cn/*](http://ubuntu.buct.edu.cn/) 端口：80
> - IPv4: [*http://ubuntu.buct.cn/*](http://ubuntu.buct.cn/) 端口：80
> - IPv6: [*http://ubuntu.buct6.edu.cn/*](http://ubuntu.buct6.edu.cn/) 端口：80
> **上海GDG镜像服务器地址:**
> - [*http://sdk.gdgshanghai.com*](http://sdk.gdgshanghai.com/) 端口：8000
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image4.png" width="336" height="301" />

1.  打开Windows资源管理器，进入以下路径“C:\\Windows\\System32\\drivers\\etc”（注意路径，不要出错，Win7可直接拷贝路径进入相应文件夹）。找到“hosts”文件并用记事本打开。在hosts文件的末尾添加以下内容

> 74.125.237.1 dl-ssl.google.com
>
> 203.208.46.146 www.google.com
>
> 203.208.46.146 dl.google.com
>
> 203.208.46.146 dl-ssl.google.com

安装node
--------

> 基于js的，node.js轻量级的Web服务器，想要是React Native跑起来需要安装node， 如果没有安装node.js，先去官网安装node.js,最好是4.1以上版本
>
> 下载地址：https://nodejs.org/en/
>
> 下载node.js，找好对应的版本，然后去安装就可以了。
>
> 大家可以通过node -v的命令来测试NodeJS是否安装成功
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image5.png" width="510" height="163" />

安装git
-------

> 安装React-native需要用到git，如果没有配置git，需要先下载对应的客户端，然后将git加入path环境变量即可
>
> 下载地址：https://git-for-windows.github.io/
>
> 安装：
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image6.png" width="329" height="254" />
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image7.png" width="321" height="248" />

安装react-native命令行工具react-native-cli
------------------------------------------

> git配置完成后可以clone React-native-cli了，建议大家到将react-native-cli克隆到某个盘，不要在c盘直接clone

1.  ### 在命令行中进入你希望RN安装的目录

2.  ### 输入git clone

> https://github.com/facebook/react-native.git，等待下载
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image8.png" width="553" height="139" />
>
> clone成功后：
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image9.png" width="553" height="265" />

### 进入刚刚目录下的react-native目录下的react-native-cli目录

> 输入npm install –g
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image10.png" width="553" height="237" />
>
> 安装好之后，可以命令行下就有react-native命令了

创建RN项目 
-----------

> 进入你希望创建项目的目录后，输入react-native init AwesomeProject，等待一段时间（较慢）
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image11.png" width="553" height="127" />成功后：
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image12.png" width="553" height="269" />
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image13.png" width="553" height="242" />

运行package
-----------

> 在命令行中进入项目目录，输入react-native start，等待一段时间：
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image14.png" width="450" height="474" />
>
> 这时候可以用浏览器访问http://localhost:8081/index.android.bundle?platform=android，如果可以访问表示服务器端已经可以了。
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image15.png" width="398" height="401" />

运行项目
--------

> **\*（此时一定要记着把android手机连接USB介到电脑上，而且手机需要调成开发模式）**
>
> 刚刚运行package的命令行不要关闭，重新启动一个新的命令行，
>
> 进入项目目录，输入react-native run-android
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image16.png" width="553" height="166" />
>
> 等待运行(如果是第一次运行，首先会下载gradle，时间较长)
>
> 运行成功后出现下图
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image17.png" width="553" height="368" />
>
> 第一次手机肯定报错
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image18.png" width="309" height="547" />
>
> 这时候我们摇一摇手机，点击Dev Settings后，点击Debug server host & port for device,设置IP和端口
>
> “摇一摇”这个动作在模拟器可以用ctrl+M (Menu)来调出Dev setting菜单。
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image19.png" width="553" height="367" />
>
> 这里的IP是电脑的IP，不知道的可以在命令行中输入ipconfig进行查询，端口号固定8081
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image20.png" width="222" height="394" />
>
> 设置完成后，回到空白页面，再次摇一摇手机，选择Reload JS，程序就运行起来，出现Welcome to React Native！
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image21.png" width="553" height="358" />
>
> **到此Andorid开发环境以及单间完毕，一下的内容都是围绕更好的使用工具提高开发速度和效率。**

1.  Andorid环境搭建完成
    -------------------

2.  WebStrom集成React Native
    ------------------------

安装和破解（略）

### 新建项目

> File-&gt;new-&gt;Project-&gt;E（工作区）
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image22.png" width="553" height="205" />

### 刷新浏览项目

> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image23.png" width="358" height="314" />

### 下载项目的依赖包

打开项目找到package.json文件—&gt;右键选择—&gt;Run npm install/update

这个过程较长，慢慢等吧。

<img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image24.png" width="281" height="388" />

<img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image25.png" width="435" height="56" />

### 初始化项目（过程比较长）

点开Terminal –&gt; cd MaterialReactNative –&gt; react-native run-android

<img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image26.png" width="444" height="147" />

见到BUILD SUCCESSFUL 及为成功！

### 启动项目

> Package.json 右键—&gt; Show npm Script
> 如下图
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image27.png" width="272" height="367" />
>
> 双击
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image28.png" width="360" height="101" />
>
> 启动
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image29.png" width="439" height="92" />
>
> 为成功。

### webStrom 不识别React 和React Native时

<img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image30.png" width="430" height="194" />

识别React.

<img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image31.png" width="427" height="136" />

在下图的download manager里面找到react和react-native下载安装，然后返回到上图的窗口，按照上图第五部分勾选刚才下载的两个library即可

<img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image32.png" width="430" height="113" />

必须勾选，保存。

至此完毕，最终效果如下：

<img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image33.png" width="397" height="286" />

模拟器安装Genymotion
--------------------

> 在安装Genymotion的时候，他会提示你需要安装VirtualBox，这个必须安装。
>
> 优点：与Android SDK自带的模拟器相比，Genymotion更为流畅，推荐安装使用。需要去官方网站（https://www.genymotion.com/）注册个人用户账号。

### 安装说明

1.  #### **确保你系统之前没有装过虚拟机或者已经卸载干净，或者你懂关联genymotion和你本身安装了的虚拟机；**

2.  #### **安装VirtualBox4.1.20,一路点击next；**

3.  #### **安装genymotion-2.4.0；**

###  使用说明

1.  #### **启动genymotion，并使用自己在Genymotion官网注册的账号密码登陆；**

2.  #### **如果要关联自己本地的SDK就需要进行配置：在genymotion主界面，依次点击settings—&gt;ADB—&gt;Use custom Android SDK tools,在Android SDK框中选择你电脑上sdk文件夹路径，如我电脑上就是E:\\adt-bundle-windows-x86\_64-20140702\\sdk；**

<img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image34.png" width="391" height="99" />

<img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image35.png" width="400" height="247" />

#### **在genymotion主界面点击add即可添加你想要的模拟器型号，选择一个，让他下载好就可以用了**

> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image36.png" width="388" height="78" />
>
> <img src="https://github.com/jonymrshi/react-native-webstrom/blob/master/media/image37.png" width="388" height="276" />
>
> 选择一个一直Next 就可以了

#### **模拟器下载好后双击模拟器将其启动；**

学习技巧
========

(待续)
