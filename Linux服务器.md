# __Linux服务器__    

# __尺寸__   

# __服务器尺寸__  

&ensp;&ensp;&ensp;&ensp;高度:1U=44.45mm  
&ensp;&ensp;&ensp;&ensp;(高度:1U,2U,4U,5U,7U的,多数企业中常见的是4U,当然现在都用云服务器了,基本没人鸟物理机,实际上是因为你格调够不着许多牛逼的物理机)   

&ensp;&ensp;&ensp;&ensp;宽度:19英寸=48.26cm  

# __放服务器的机柜的尺寸__  

&ensp;&ensp;&ensp;&ensp;宽600mm  
&ensp;&ensp;&ensp;&ensp;深600mm、800mm、1000mm（一般是这种）  
&ensp;&ensp;&ensp;&ensp;高2000mm  

# __硬件组成__  

&ensp;&ensp;&ensp;&ensp;游戏本或者商务本应该都可以用一个叫"鲁大师"的软件中的"硬件检测"这个功能查到自己电脑的具体硬件信息  
&ensp;&ensp;&ensp;&ensp;在Windows的cmd中,基本上使用这些命令就可以查看到下面这些硬件的许多信息,但相比于使用软件看到的没那么详细:  
&ensp;&ensp;&ensp;&ensp;wmic cpu get name&ensp;&ensp;&ensp;&ensp;查看CPU型号.实际上wmic这个命令比较强
&ensp;&ensp;&ensp;&ensp;taskmgr&ensp;&ensp;&ensp;&ensp;可查看下面的绝大多数硬件使用情况以及型号  
&ensp;&ensp;&ensp;&ensp;systeminfo&ensp;&ensp;&ensp;&ensp;功能很强大的一个命令,试试就知道

# __CPU__


&ensp;&ensp;&ensp;&ensp;按照CPU体系架构分为两种:  
# &ensp;&ensp;&ensp;&ensp;__x86__
&ensp;&ensp;&ensp;&ensp;我们在学校使用的游戏本,商务本一般都是这种类型的.有着复杂指令集,CISC服务器,价格相对便宜,兼容性好,稳定性较差,安全性不算太高  

# &ensp;&ensp;&ensp;&ensp;__非x86__
&ensp;&ensp;&ensp;&ensp;精简指令集或并行指令代码,RISC或EPIC,价格贼鸡儿贵,体系封闭,稳定性好,性能强,金融.电信这些大企业的核心系统  

# &ensp;&ensp;&ensp;&ensp;__性能__   

&ensp;&ensp;&ensp;&ensp;个人认为,主要看下面这几种:  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;主频:中央处理器运算时的工作频率  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;外频:系统总线工作频率,与主板芯片组交换数据的频率  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;主频=外频*倍频(主频与外频相差的倍数)  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;CPU缓存:分三级,一级最高  



# __主板__  


&ensp;&ensp;&ensp;&ensp;计算机最基本,最主要的部件之一,与我们生活中关系比较密切的就是主板支持的最大内存.像吃鸡英雄联盟这类游戏一般都需要比较大的运行内存,而主板就决定着最大运行内存,决定着你可以插几块内存条,最多可以扩展到多大的内存等等重要的信息  




# __内存__   


&ensp;&ensp;&ensp;&ensp;用360的那个清理球清理的就是运行内存,手机上的内存加速球清理手机运行内存.  
&ensp;&ensp;&ensp;&ensp;内存在断电后,内存中的数据就会丢失.  
&ensp;&ensp;&ensp;&ensp;这句话什么意思呢?就是说我们断电后,再打开电脑,我们没在英雄联盟的游戏界面里,英雄联盟的数据丢失了,所以我们进入的是开机画面.   

&ensp;&ensp;&ensp;&ensp;相比于内存,外存断电后数据就不会丢失.  


DDR2 667，运行频率为333MHz,带宽为多少？(第一个D是双通道的意思)  
&ensp;&ensp;&ensp;&ensp;怎么算?这玩意儿有个公式  
&ensp;&ensp;&ensp;&ensp;__内存总线频率*数据总线位数/8=内存带宽__  
&ensp;&ensp;&ensp;&ensp;(内存带宽是指内存与北桥芯片之间的数据传输率)(什么是北桥芯片自个儿百度或者谷歌,当然你要是觉着百度谷歌都不靠谱可以来问我,2065513186这是QQ,微信号搜索www_leishujun_com)  
&ensp;&ensp;&ensp;&ensp;333x2x64/8=5400MB/s=5.4GB/s  


# __显卡__  


&ensp;&ensp;&ensp;&ensp;GPU： Graphic Processing Unit，图形处理器.

&ensp;&ensp;&ensp;&ensp;这玩意和视觉效果有关,我们在电脑上常说的GTX960,GTX1080,在服务器的主板上都集成了显卡，而且显存容量都比较低，一般为16M或32M,因为基本上所有的常见的服务器都只需要字符界面,当然Windows server例外.   


# __网卡__  

&ensp;&ensp;&ensp;&ensp;我们生活中直接和你电脑上蓝色的线直接相连接的东西就是网卡,当然,还有种无限网卡,是不和你电脑的网线直接相连接的.市面上主流服务器上一般都有2-4块网卡,但是不装无限网卡.  
&ensp;&ensp;&ensp;&ensp;实际上我们个人用户只要有无线网卡,可以在不使用软件的情况下在Windows版本比较低的系统中也能使用WiFi开启承载模式,然后把正在使用的网络共享给设置好的ssid即可,当然win 10小伙伴比较新的版本自带移动热点,可以无视.具体的操作方式如下:  
1.按下"Windows"键  
2.在搜索栏中输入"cmd"  
3.右击鼠标选择"以管理员身份运行"  
4.点击"确定"  
5.在cmd中输入"netsh wlan set hostednetwork mode=allow ssid=lei key=123456789",这里的ssid设置的是账号,key设置的是密码 ,  输入这条命令后,这里会提示你  

&ensp;&ensp;&ensp;&ensp;承载网络模式已设置为允许。  
&ensp;&ensp;&ensp;&ensp;已成功更改承载网络的 SSID。  
&ensp;&ensp;&ensp;&ensp;已成功更改托管网络的用户密钥密码。   

6.输入"netsh wlan start hostednetwork"这里会提示你  

&ensp;&ensp;&ensp;&ensp;已启动网络承载模式  
  
7.输入"ncpa.cpl"  
8.找到你目前使用的网络   
9.右击这个网络,选择"属性"  
10.再点"共享"  
11.勾选"允许其他用户通过此计算机的internet连接来连接"  
12.在"请选一个专用网络连接"中选择你之前在cmd中设置好的那个网络,名字是lei的那个"本地连接*12"(一般是本地连接*)  
13.确定  
&ensp;&ensp;&ensp;&ensp;现在WiFi可以使用了,用手机试试!  
&ensp;&ensp;&ensp;&ensp;当然,如果想要关闭,只要在dos中输入下面这两条命令就行  
&ensp;&ensp;&ensp;&ensp;netsh wlan stop hostednetwork  
&ensp;&ensp;&ensp;&ensp;netsh wlan set hostednetwork mode=disallow  
&ensp;&ensp;&ensp;&ensp;此时你再看网络连接中就找不到你之前设置的WiFi了.


# __硬盘__  

&ensp;&ensp;&ensp;&ensp;就是我们常说的手机存放内存(不是前面说到的运行内存)容量大小,放不下东西的时候,这时候我们清理的是手机里面的硬盘,而在电脑上方便不下东西的时候清理的是机械硬盘.开机只需6秒,非常快的那叫固态硬盘,也是硬盘的一种.  

常见硬盘接口:IDE,SCSI,SATA（主流）,SAS(主流)  

# __热插拔技术__  
&ensp;&ensp;&ensp;&ensp;又名热交换技术,常与RAID技术一配合使用,可以在不关机状态下恢复故障硬盘上的数据,同时还能影响网络用户对数据的使用

# __在线备用内存技术__:  
&ensp;&ensp;&ensp;&ensp;一个存数据进来,一个做备用.出现故障了,就换另一个.一个当男朋友,一个当备胎,前面那个分了,后面这个换上.

# __内存镜像__:
&ensp;&ensp;&ensp;&ensp;同时写入两个存放数据的区域中.脚踏两只船,同时和两个人交往.

# __存储基础知识--存储网络__  

&ensp;&ensp;&ensp;&ensp;DAS-----直接连接存储(Direct Attached Storage)(自己电脑的内存和硬盘的关系)


&ensp;&ensp;&ensp;&ensp;NAS-----网络连接存储(Network Attached Storage)(学校使用的FTP)


&ensp;&ensp;&ensp;&ensp;SAN-----存储区域网络(Storage Area Networks)  (百度网盘,能上传下载东西,还能管理自己的网盘内的存储空间)

各硬件读取速度小结:  
&ensp;&ensp;&ensp;&ensp;CPU>CPU缓存>内存>内存缓存>固态硬盘>机械硬盘>  

# __短板效应__：

&ensp;&ensp;&ensp;&ensp;由短板效应可知,我们上网玩英雄联盟有时候用一般键盘按DF二连感觉会反应很慢时,换成机械键盘就更流畅的结论并不科学.实际上,与机械键盘直接相关的不仅仅是键盘的问题,我们的输入设备USB接口传输数据的速度本身就比较慢的话,即使换成机械键盘也无用,只是手感上相对普通键盘较好!   
 &ensp;&ensp;&ensp;&ensp;同样的硬盘的读写速率也是影响系统性能的一个原因,用机械硬盘进入用户登陆界面需要1分钟,同样用固态硬盘进入登陆界面也许只要6~15秒!

# __按照应用功能分服务器__    

# web
apache、nginux     

# 数据库
myspl、Oracle  

# 文件
NFS、SAMBA、FTP  

# 中间件
Tomcat  

# 日志
Rsyslog  

# 监控
Zabbix  

# 程序
GIT  

# 虚拟机
KVM  

# 邮件
Sendmail  

# 域控制器
主要是微软用其中有种名叫DC（domain controller）、AD (active directory)
