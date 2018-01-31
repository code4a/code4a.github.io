# 联系方式

- 手机：17600975947 
- Email：jiangyantaodev@163.com
- QQ：1286744353

---

# 个人信息

- 蒋彦涛/男/1991 
- 专科/河南科技大学信息工程系 
- 工作年限：4年
- Google+：[Jiang Yantao](https://plus.google.com/+jiangyantao8)
- 技术博客：http://www.code4a.com ( ``` Hexo + Github ```  )
- GitHub：https://github.com/code4a

- 期望职位：Android高级工程师
- 期望薪资：税前月薪17k~20k，特别喜欢的公司可例外
- 期望城市：北京

---

# 工作经历


## 文思海辉技术有限公司 （ 2014年8月 ~ 至今 ）

### IotHub项目

此项目是移动研究院基于自主协议(AndLink)开发的智能家居解决方案。各类传感器(门磁/温湿度/水浸/红外/门锁/等)通过主板的zigbee模块，和网关的zigbee模块进行通讯，网关的zigbee模块通过串口将数据上报到网关的上层程序Andlink模块。数据上报到Andlink云平台，平台通过mqtt再将实时数据推送到手机的和家安App通知用户家庭的状态。

### AndLink项目 

此项目是移动研究院基于自主协议(AndLink)开发的智能家居Android客户端。旨在使用手机客户端通过网络(WiFi/4G/蓝牙)发送各种指令(Http/Tcp/Udp/Socket/WebSocket)到自主研发的家庭网关，从而控制各种配套的家庭智能设备（例：灯、窗帘、车库、冰箱、空调、洗衣机、空气净化器、电饭煲、插座、各种传感器和安防监控设备等）。我在此项目负责客户端与网关的通信，发送对应的智能设备控制指令从而使其正常工作。包括app UI界面的变更优化，使用MVP模式(Model-View-Presenter)剥离Activity中相关的代码逻辑，从而快速完成UI风格的各种变化已应对移动研究院对各种展会的迅速响应。由于每次展会前期开发周期较短，所以从几次展会的过程中获得规律，不断优化改进项目架构，使其每次变更做到效率最高。在一次上海展中由于app良好的展示效果，从而使项目组的领导得到了展会记者的采访，后期得到了领导的赏识和器重。整个项目的开发过程中，需要自行和各个厂商的技术人员进行沟通兼容他们的智能设备，再处理三星的空气净化器时，将每次登陆鉴权，优化为后台刷新Token，从而优化控制流程！


### WiMo项目 

此项目是移动研究院基于自主投屏协议(WiMo协议)开发的屏幕共享和媒体共享的Android客户端，旨在通过手机客户端，将手机资源大屏共享，从而体验大屏乐趣！此客户端主要作用是为了配合移动研究院自主产品：和屏、魔百和、dongle等接收设备开发！其中机顶盒Service，需要保证开机自启动，无网络连接的情况下自启动AP热点，程序意外退出重启，常驻内存，运行小型服务(NanoHTTPD)接收客户端的http请求，并给予相应的响应等功能！Android客户端，需要完成筛选网络优先连接，自动连接指定网络，连接完成后初始化WiMo服务！其中的难点就是为和屏、dongle、魔百盒等进行网络配置，首先需要客户端优先自动连接至WiMo接收端特有的SSID，然后发送Http请求给这些接收端，等待下一步回应，当响应成功之后，手机自动连接至接收端同一网络下，然后初始化WiMo协议，等待发现设备，在用户无感知的情况下，进行媒体和平面共享，当响应不成功时，轮询等待接收端热点出现，然后重新连接该AP，给予用户提示(例如：密码错误)，等待用户下一步操作！通过对这些需求的梳理和慢慢实现优化的过程，也对WiFi这个模块相对熟悉一些，了解程序可以实现到哪一步，从而减少用户的操作次数！


### WiMoSDK

此项目是移动研究院基于自主研发的WiMo投屏协议，封装的SDK，包含媒体大屏共享和屏幕共享的功能！提供给咪咕视频、咪咕动漫、咪咕趣、咪咕音乐、和视频、和动漫等系列App使用，进行大屏共享！此项目由Java、Jni、和C/C++ 封装成的Android SDK，其中Jni 通过动态注册，这种注册可以不受命名限制。动态注册函数调用时机是当java层通过System.loadLibrary加载完jni动态库后，紧接着会查找该库中一个叫JNI_OnLoad的函数，从而将动态注册的工作放到此函数里边，进行方法绑定！


### WiMoPPT

此项目是一个小工具，为了方便移动研究院内部小会议，制作的一款投放PPT的小程序，基于WiMo协议，拓展的PPT专用协议，通过发送URI将客户端的的ppt链接发送给机顶盒Service，使其下载到本地，然后解析PPT在Activity中进行展示，平板也同步解析展示，通过UPNP指令，对其进行放大缩小、上一页、下一页，跳转等指令控制，Service同时也可响应激光笔的指令！


### 发票小工具

此项目是为扫描发票代码开发的小工具，使用了开源的OCR文字识别库tess-two, 可打开关闭闪光灯，调整识别区域，将设备的结果读出来保存到csv中。

## 武汉漫步者文化传播有限公司 （ 2013年7月 ~ 2014年7月 ）


### e拇指

我在此项目协助pm完成应用框架的搭建，完成联网协议的处理和联网工具类的编写，抽象类和接口的抽取，对初始化数据的获取和存储，以及首页模块和活动模块的实现，项目中疑难bug的解决。该项目主界面FrameActivity继承activityGroup，主要完成应用数据的初始化，获取定位和用户信息并通过网络接口异步上传到服务器，初始化界面，完成主界面的切换，检查并维护应用的生命周期，完成各个阶段的数据初始化/销毁等操作和方法调用。界面模块：内部使用到Stack数组存放(封装intent，class，view等信息)自定义类模拟任务栈，存放界面的帧布局数组，界面内部视图的view数组和界面对应的class字节码文件数组。页面切换是通过获取到点击的tab的索引值(需要注意是在底部导航初始化时需要给每个视图设置tag)，取出class等数组中的值通过getLocalActivityManager调用startActivity用intent绑定对应的activity获取返回window对象，调用getDecorView()方法获取到顶层视图，赋值给stack栈中的自定义对象的view属性中，通过切换不同的类中的View的显示与隐藏，实现tab的视图切换。四个界面的父类BaseActivity完成公共的操作的抽取如标题栏的初始化，提示消息，dialog的显示与隐藏等，以及对按键的处理等操作。主界面整个就是使用pullToRefresh开源框架，实现下拉刷新和加载更多功能，第一个条目是一个自定义的线性布局通过addHeaderView将布局添加进去，完成gridview的事件处理，定位，和条目图片的异步加载，活动界面是通过一个自定义的3D画廊，完成图片的展示，该功能的实现是通过自定义类继承gallery，重写getChildStaticTransformation和onSizeChanged两个方法，完成图片的放大，旋转的效果实现，通过LruCache进行图片的缓存管理，通过在适配器中调用getView方法展示图片是首先展示默认图片，通过封装工具类异步加载网络图片进行替换，增强用户体验


### 扯蛋日报

我在职责是完成项目中json数据的解析bean对象的封装，联网工具类和处理图片的工具类的编写，完成主页面的信息展示，该项目主界面是使用一个Activity管理生命周期，做相应的逻辑操作，通过setContentView将布局文件解析成View对象添加到Phonewindow创建的ViewGroup中进行展示，和用户交互。抽取一个BaseActivity，完成标题栏的的初始化，和按键的处理，定义一个baseView抽象类，通过构造传递参数，在内部添加两个抽象方法，initView初始化布局和initData填充布局中的数据，在页面模块的实现中，将界面划分为标题栏，导航栏，带一个帧布局的ListView添加Android-ViewPagerIndicator指针项目，完成导航条功能，每个导航条绑定一个viewpage的页面，利用xutils 框架中的HttpUtils进行客户端与服务器的交互(在模版类中提供方法)，使用BitmapUtils进行对从服务器获取的图片数据的处理，完成ListView异步加载图片完成数据的填充，导入PullToRefresh下拉刷新框架，完成下拉刷新数据和滚动加载更多数据


### 新闻客户端-此项目为逆向工程

逆向后发现该项目源码未做加密处理和代码混淆，分析出其工程的整体架构，和应用到的开源框架，以及常用的第三方的sdk，分析其中对协议的处理封装方式，学习其中优秀的编程思想和代码风格，了解他人是如何利用开源框架的，如何在原有的框架基础之上封装出适合自己公司的工具类，并提供对应的文档(提供文档是自己理解的应该需要文档)给其他pg使用


### 静默安装器-业余项目

查看系统安装应用的原理，编写代码在linux环境下，编译代码，系统进行过Android2.3的源码编译(在Windows环境下有些类无法引用其方法)，编译生成的apk装入手机之后，可以在用户无察觉的情况下进行软件的安装

---

# 开源项目和作品


## 开源项目

- [RetrofitUtil](https://github.com/code4a/NbaEvent)：此项目是对Retrofit + OKHttp + RxJava 简单二次封装，支持Http/Https请求，支持自己定义SSL解析，请求结果可以是String类型也可以是解析好的bean对象！
- [WiFiConnectLib](https://github.com/code4a/WiFiConnectLibrary)：此项目是一个将Android手机WiFi连接到指定热点的开源的Android库，可以很方便的通过程序操作手机的WiFi！
- [JLibrary](https://github.com/code4a/JLibraryDemo)：此项目是一个开源的Android库，提供了一些界面的基类和工具类，包含crash日志本地化，crash重启，修改状态栏颜色等功能，项目在不断完善更新中！
- [BatScript](https://github.com/code4a/BatScript)：这是一个批处理，旨在简化开发环境的配置，如java、sdk等，通过批处理批量添加配置，解决每次换环境一堆配置的麻烦，拷贝，运行轻松搞定！
- [UpdateManager](https://github.com/code4a/UpdateManager)：这是一个支持多线程下载的Library，支持解析json和xml，断点续传等功能
- [CustomView](https://github.com/code4a/CustomView)：这是自定义控件，包含扇形进度条（常用于时速表盘，压力表盘等），和带刻度柱状图（常用于流量计等）

## 技术文章

- [使用NanoHTTPD在Android上建立本地服务器](http://www.code4a.com/2016/03/11/NanoHTTPD-Simple-Use/)


# 技能清单


以下均为我熟练使用的技能

- 扎实的Java基础，熟练掌握面向对象（OOP）思想，熟悉java序列化机制实现Android下IPC的机制。
- 熟练使用集合、IO流及多线程断点上传下载,和线程池的使用。
- 熟练掌握Android四大组件（Activity，Service与intentService，LocalBroadcastManager的BroadcastReceiver，ContentProvider）
- 熟练使用Android下常用的布局设计，新版本Material Design布局和设计，熟练自定义控件和一些主流的第三方控件的使用等。
- 熟悉掌握MVC/MVP模式，单例、工厂，观察者，适配器等设计模式。
- 熟悉Android下的Handler消息机制（Handler，Message，MessageQueen，Looper，HandlerThread），并能熟练使用Handler和熟悉使用EventBus 和RXandroid机制。
- 熟悉Android中的动画，选择器，样式和主题的使用，能够实现市面上大多数动画效果。
- 掌握OOM、ANR异常和各类友盟统计上的BUG的处理和熟练处理App全局Crash异常处理，并可以对应用进行相应的优化。
- 熟悉Android开发的数据（图片，文字，文件等）的缓存技术，并且能够对图片的优化进行相应的处理，熟悉ASimpleCache，LruCache缓存和DiskLruCache缓存使用。
- 熟练并能独立解决市面上各种Android机型屏幕的适配（图片适配，Dimens适配和AutoLayout适配等等）。
- 熟练使用Git/SVN等版本控制工具。
- 熟练使用Android Studio、Eclipse、Vim、XShell、iTerm2、Dash、Volecity、Beyond Compare、Markdown、谷歌浏览器、科学上网、等开发利器
- 熟悉XML/JSON数据解析和生成JSON/XML，以及Android下SQLiter数据库存储方式（greendao，ormlite）。
- 熟悉android 的JNI/NDK开发，通过JNI实现JAVA与C程序间的调用及回调数据通信。
- 熟悉掌握RecyclerView，ListView等重要控件的使用和优化及（AsyncTask）异步任务加载网络数据
- 熟悉使用支付宝，微信支付的SDK和银行的卡SDK的接入，为App增加支付模块。
- 熟练使用Android下的GPS定位和（接入百度地图定位SDK实现定位，标记，搜索等功能）
- 熟悉主流常用的第三方SDK（友盟统计，极光送，QQ和微信的三方登陆和分享SDK，热更新Sophix，基于百度/讯飞语音的文字和语音的相互转化开发）
- 熟悉Android下混合开发，原生App和HTML5的使用，和js交互，数据通信。


## 技能关键字


- android
- java
- app
- http
- sdk
- tcp
- socket
- json
- ndk
- andriod
- github
- jni
- svn
- git
- code review
- stackoverflow
- andorid
- udp
- vim

---

# 致谢
感谢您花时间阅读我的简历，期待能有机会和您共事。