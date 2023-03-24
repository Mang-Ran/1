# linux服务器管理

## 建议下载xftp,xshell,Todesk软件进行远程管理

| ![image-20230323211710015](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232117552.png) | **Xftp是一个用于Windows系统平台上的FTP、STFP协议文件传输程序，它能帮助用户安全地在Unix系统和Windows系统上进行快速的文件传输任务，并且它可对文件列表进行可视化展示，更符合Windows用户的使用习惯。** | 下载地址：https://www.xshell.com/zh/xftp/       |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ----------------------------------------------- |
| ![image-20230323211721171](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232117559.png) | **Xshell 是一个强大的安全终端模拟软件，它支持SSH1, SSH2, 以及Microsoft Windows 平台的TELNET 协议。Xshell 通过互联网到远程主机的安全连接以及它创新性的设计和特色帮助用户在复杂的网络环境中享受他们的工作。Xshell可以在Windows界面下用来访问远端不同系统下的服务器，从而比较好的达到远程控制终端的目的。** | **下载地址：https://www.xshell.com/zh/xshell/** |
| ![image-20230323211814127](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232118279.png) | **Xshell可以在Windows界面下用来访问远端不同系统下的服务器，从而比较好的达到远程控制终端的目的。作用：远程操控电脑，进行远程的图形化操作** | **下载地址：https://www.todesk.com/**           |

## 服务器介绍

什么是服务器 ？

​	就像他的名字一样，服务器在网络上为不同用户提供不同内容的信息、资料和文件。可以说服务器就是Internet网络上的资源仓库，正是因为有着种类繁多数量庞大内容丰富的服务器的存在，才使得Internet如此的绚丽多彩

FTP服务器(FTP Server) 

​	FTP免费云服务器是专门为用户提供各种文件(File)的服务器，FTP免费服务器上往往存储大量的文件，例如：软件、MP3、电影、程序等等。用户只要使用FTP客户端软件登录到FTP服务器上就可以从FTP免费服务器下载所需文件和资源到自己的电脑上，同时， 还有免费虚拟主机
你也可以把自己电话上的文件上传到FTP上供其他用户下载，以实现文件资源的共享。

服务器：分为服务器硬件和服务器软件。在硬件服务器（计算机）上安装服务器软件，才可以对外提供服务。
比如：让其他的计算机访问当前服务器，为其他的计算机提供服务。
（1）服务器硬件：是指在互联网上具有独立IP地址的计算机，比如我们自己用的计算机也可以作为服务器使用。
（2）服务器软件：就是一个计算机程序。比如Mysql服务器软件，tomcat服务器软件。服务器软件分为很多类型，比如：ftp服务器，数据库服务器，web服务器软件，邮件服务器等。

![image-20230323220712543](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232207567.png)

想玩服务器的还有很多，比如说家庭的NAS，硬盘的RAID技术，各级别的优缺点，有兴趣的都可以去看看，还是挺好玩的（B站视频动态化可能更有趣）



详细参考[1](https://blog.csdn.net/Song_xiaochen/article/details/123163619?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167957914816800180646298%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=167957914816800180646298&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_positive~default-1-123163619-null-null.142)

详细参考[2](https://blog.csdn.net/Song_xiaochen/article/details/123163619?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167957914816800180646298%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=167957914816800180646298&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_positive~default-1-123163619-null-null.142)



## Linux介绍

Linux是一种自由和开放源码的操作系统，存在着许多不同的Linux版本，但它们都使用了Linux内核。Linux可安装在各种计算机硬件设备中，比如手机、平板电脑、路由器、台式计算机

![image-20230323221331662](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232213685.png)

我们比较常用的是：CenOS和UBUNTU

Linux特点:

多用户，多任务，丰富的网络功能，可靠的系统安全，良好的可移植性，具有标准兼容性，良好的用户界面，出色的速度性能
开源

CentOS

- 主流：目前的Linux操作系统主要应用于生产环境，主流企业级Linux系统仍旧是RedHat或者CentOS
- 免费：RedHat 和CentOS差别不大，基于Red Hat Linux 提供的可自由使用源代码的企业CentOS是一个级Linux发行版本
- 更新方便：CentOS独有的yum命令支持在线升级，可以即时更新系统，不像RedHat 那样需要花钱购买支持服务！

![image-20230323221559023](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232215044.png)

![image-20230323221642340](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232216361.png)

[详细解释](https://blog.csdn.net/Song_xiaochen/article/details/123163619?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167957914816800180646298%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=167957914816800180646298&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_positive~default-1-123163619-null-null.142)

# Linux常用代码

```
关机
    shutdown -h now        立刻关机
    shutdown -h 5          5分钟后关机
    poweroff               立刻关机
重启
    shutdown -r now        立刻重启
    shutdown -r 5          5分钟后重启
    reboot                 立刻重启

目录切换 cd
命令：cd 目录

cd /           切换到根目录
cd /usr        切换到根目录下的usr目录
cd ../         切换到上一级目录 或者  cd ..
cd ~           切换到home目录
cd -           切换到上次访问的目录

目录查看 ls [-al]
命令：ls [-al]

ls                  查看当前目录下的所有目录和文件
ls -a               查看当前目录下的所有目录和文件（包括隐藏的文件）
ls -l 或 ll         列表查看当前目录下的所有目录和文件（列表查看，显示更多信息）
ls /dir             查看指定目录下的所有目录和文件   如：ls /usr
```

### su、sudo

```
su
su用于用户之间的切换。但是切换前的用户依然保持登录状态。如果是root 向普通或虚拟用户切换不需要密码，反之普通用户切换到其它任何用户都需要密码验证。

su test:       切换到test用户，但是路径还是/root目录
su - test :    切换到test用户，路径变成了/home/test
su :           切换到root用户，但是路径还是原来的路径
su - :         切换到root用户，并且路径是/root
su - 用户名 ：  切换用户

su不足：             如果某个用户需要使用root权限、则必须要把root密码告诉此用户。
退出返回之前的用户：    exit

sudo
sudo是为所有想使用root权限的普通用户设计的。可以让普通用户具有临时使用root权限的权利。只需输入自己账户的密码即可。

进入sudo配置文件命令：
vi /etc/sudoer或者visudo

案例：
允许hadoop用户以root身份执行各种应用命令，需要输入hadoop用户的密码。
hadoop  ALL=(ALL)   ALL 
案例：
只允许hadoop用户以root身份执行ls 、cat命令，并且执行时候免输入密码。 
配置文件中： 
hadoop  ALL=NOPASSWD:  /bin/ls, /bin/cat 
```



### 目录操作

```
创建目录【增】 mkdir
命令：mkdir 目录

mkdir    aaa            在当前目录下创建一个名为aaa的目录
mkdir    /usr/aaa       在指定目录下创建一个名为aaa的目录

删除目录或文件【删】rm
命令：rm [-rf] 目录

删除文件：
rm 文件        删除当前目录下的文件
rm -f 文件    删除当前目录的的文件（不询问）

删除目录：
rm -r aaa    递归删除当前目录下的aaa目录
rm -rf aaa    递归删除当前目录下的aaa目录（不询问）

全部删除：
rm -rf *    将当前目录下的所有目录和文件全部删除
rm -rf /*    【自杀命令！慎用！慎用！慎用！】将根目录下的所有文件全部删除

注意：rm不仅可以删除目录，也可以删除其他文件或压缩包，为了方便大家的记忆，无论删除任何目录或文件，都直接使用 rm -rf 目录/文件/压缩包

目录修改【改】mv 和 cp
一、重命名目录
    命令：mv 当前目录  新目录
    例如：mv aaa bbb    将目录aaa改为bbb
    注意：mv的语法不仅可以对目录进行重命名而且也可以对各种文件，压缩包等进行    重命名的操作

二、剪切目录
    命令：mv 目录名称 目录的新位置
    示例：将/usr/tmp目录下的aaa目录剪切到 /usr目录下面     mv /usr/tmp/aaa /usr
    注意：mv语法不仅可以对目录进行剪切操作，对文件和压缩包等都可执行剪切操作

三、拷贝目录
    命令：cp -r 目录名称 目录拷贝的目标位置   -r代表递归
    示例：将/usr/tmp目录下的aaa目录复制到 /usr目录下面     cp /usr/tmp/aaa  /usr
    注意：cp命令不仅可以拷贝目录还可以拷贝文件，压缩包等，拷贝文件和压缩包时不    用写-r递归
```

### 文件操作

```
新建文件【增】touch
命令：touch 文件名
示例：在当前目录创建一个名为aa.txt的文件        touch  aa.txt

删除文件 【删】 rm
命令：rm -rf 文件名

修改文件【改】 vi或vim
【vi编辑器的3种模式】
    基本上vi可以分为三种状态，分别是命令模式（command mode）、插入模式（Insert mode）和底行模式（last line mode），各模式的功能区分如下：
1) 命令行模式command mode）
      控制屏幕光标的移动，字符、字或行的删除，查找，移动复制某区段及进入Insert mode下，或者到 last line mode。
      命令行模式下的常用命令：
      【1】控制光标移动：↑，↓，j
      【2】删除当前行：dd 
      【3】查找：/字符
      【4】进入编辑模式：i o a
      【5】进入底行模式：:
      
2) 编辑模式（Insert mode）
      只有在Insert mode下，才可以做文字输入，按「ESC」键可回到命令行模式。
      编辑模式下常用命令：
      【1】ESC 退出编辑模式到命令行模式；
      
3) 底行模式（last line mode）
     将文件保存或退出vi，也可以设置编辑环境，如寻找字符串、列出行号……等。
     底行模式下常用命令：
     【1】退出编辑：   :q
     【2】强制退出：   :q!
     【3】保存并退出：  :wq

打开文件
命令：vi 文件名
示例：打开当前目录下的aa.txt文件     vi aa.txt 或者 vim aa.txt

注意：使用vi编辑器打开文件后，并不能编辑，因为此时处于命令模式，点击键盘i/a/o进入编辑模式。

编辑文件
使用vi编辑器打开文件后点击按键：i ，a或者o即可进入编辑模式。

i:在光标所在字符前开始插入
a:在光标所在字符后开始插入
o:在光标所在行的下面另起一新行插入

保存或者取消编辑

保存文件：
第一步：ESC  进入命令行模式
第二步：:     进入底行模式
第三步：wq     保存并退出编辑

取消编辑：
第一步：ESC  进入命令行模式
第二步：:     进入底行模式
第三步：q!     撤销本次修改并退出编辑
```

### 权限修改

```
rwx：r代表可读，w代表可写，x代表该文件是一个可执行文件，如果rwx任意位置变为-则代表不可读或不可写或不可执行文件。

示例：给aaa.txt文件权限改为可执行文件权限，aaa.txt文件的权限是-rw-------

第一位：-就代表是文件，d代表是文件夹
第一段（3位）：代表拥有者的权限
第二段（3位）：代表拥有者所在的组，组员的权限
第三段（最后3位）：代表的是其他用户的权限

   421  421  421
-  rw-   ---     ---

命令：chmod +x aaa.txt
或者采用8421法
命令：chmod 100 aaa.txt
```

### 压缩文件操作

```
Windows的压缩文件的扩展名  .zip/.rar
linux中的打包文件：aa.tar      
linux中的压缩文件：bb.gz    
linux中打包并压缩的文件：.tar.gz

Linux中的打包文件一般是以.tar结尾的，压缩的命令一般是以.gz结尾的。
而一般情况下打包和压缩是一起进行的，打包并压缩后的文件的后缀名一般.tar.gz。

命令：tar -zcvf 打包压缩后的文件名 要打包的文件
其中：z：调用gzip压缩命令进行压缩
  c：打包文件
  v：显示运行过程
  f：指定文件名
  
示例：打包并压缩/usr/tmp 下的所有文件 压缩后的压缩包指定名称为xxx.tar
tar -zcvf ab.tar aa.txt bb.txt 
或：tar -zcvf ab.tar  *

解压
命令：tar [-zxvf] 压缩文件    
其中：x：代表解压
tar -xvf ab.tar -C /usr------C代表指定解压的位置
```

### 系统服务

```
service iptables status  --查看iptables服务的状态
service iptables start  --开启iptables服务
service iptables stop  --停止iptables服务
service iptables restart  --重启iptables服务
 
chkconfig iptables off  --关闭iptables服务的开机自启动
chkconfig iptables on  --开启iptables服务的开机自启动
```

### VSFRPD服务



#### 1.vsftpd简介

vsftpd是very secure FTP daemon的缩写，安全性是它的一个最大的特点，可以运行在多种平台之上提供安全的FTP服务。在CentOS等系统以及多个互联网厂商都在使用的FTP服务程序，你值得拥有。

> 除了vftpd程序外，如wu-ftpd、proftpd、pufeftp也是较为流行的服务端程序，关于FTP相关知识请参考[Vsftpd服务器](https://zhuanlan.zhihu.com/p/393007688)



#### **2.安装服务**

```
#一般来说，安装系统会自带vsftpd，我们如果设置错了，或者怎么样，直接卸载
su -               --切换管理者root用户
sudo apt-get remove --purge vsftpd      --使用管理者权限卸载vsftpd(--purge是可选项，是将软件及其配置文件一并删除)
sudo apt-get install vsftpd             --使用管理者权限安装vsftpd
vsftpd -version                         --查看安装的vsftpd版本号
```



**关闭本机防火墙**

```
# iptables防火墙管理工具默认禁止了FTP传输协议的端口号
iptables -F			--关闭本机防火墙
```



**配置 FTP 服务**

```
程序的主配置文件为/etc/vsftpd/vsftpd.conf

#使用vim命令进行编辑
----------------------------------------
anonymous_enable=YES
local_enable=YES
write_enable=YES
local_umask=022
dirmessage_enable=YES
xferlog_enable=YES
connect_from_port_20=YES
xferlog_std_format=YES
listen=NO
listen_ipv6=YES
pam_service_name=vsftpd
userlist_enable=YES
tcp_wrappers=YES
-----------------------------------------------
```



#### 3. 配置文件

> 这里主要说的是ubuntu

- 配置文件
  ==主配置文件：/etc/vsftpd/vsftpd.conf==
  配置文件目录：/etc/vsftpd/*.conf
  服务启动脚本：/etc/rc.d/init.d/vsftpd
  用户认证配置文件：/etc/pam.d/vsftpd
- 共享目录
  匿名用户(映射为ftp用户)共享资源位置：/FTP
  系统用户通过ftp访问的资源的位置：用户自己的家目录
  虚拟用户通过ftp访问的资源的位置：给虚拟用户指定的映射成为的系统用户的家目录

#### **4配置参数**

> 常用配置参数都为主配置文件，/etc/vsftpd/vsftpd.conf的常用配置。其他的不需要动

- **通用基础配置**

| 参数                        | 作用                                                         |
| --------------------------- | ------------------------------------------------------------ |
| listen=[YES] [NO]           | 是否以独立运行的方式监听服务                                 |
| listen_address =IP地址      | 设置要监听的IP地址                                           |
| listen_port =21             | 设置FTP服务的监听端口                                        |
| download_enable=[YES]  [NO] | 是否允许下载文件                                             |
| max_client=0                | 最大客户端连接数，0为不限制                                  |
| max_per_ip=0                | 同一IP地址的最大连接数，0为不限制                            |
| chown_uploads=[YES]  [NO]   | 是否允许改变上传文件的属主                                   |
| chown_username=whoever      | 改变上传文件的属主为whoever                                  |
| pam_service_name=vsftpd     | 让 vsftpd 使用 pam 完成用户认证，使用的文件为/etc/pam.d/vsftpd |

 

**匿名用户的配置**

| 参数                               | 作用                                                         |
| ---------------------------------- | ------------------------------------------------------------ |
| anonymous enable=[YES] [ NO]       | 是否允许匿名用户访问                                         |
| anon upload enable=[YES] [ NO]     | NO是否允许匿名用户上传文件                                   |
| anon mkdir write enable=[YES] [NO] | 是否允许匿名用户创建目录                                     |
| anon other write enable=[YES] [NO] | NO]是否开放匿名用户的其他写入权限(包括重命名、删除等操作权限） |
| anon umask-022                     | 匿名用户上传文件的 umask 值                                  |
| anon root=/var/ftp                 | 匿名用户的 FTP 根目录                                        |
| anon max rate=0                    | 匿名用户的最大传输速率(字节/秒 )，0 为不限制                 |



**系统用户配置**

| 参数                                     | 作用                                                         |
| ---------------------------------------- | ------------------------------------------------------------ |
| anonymous enable=NO                      | 禁止匿名访问模式                                             |
| local enable=[YES] [NO]                  | 是否允许本地用户登录 FTP                                     |
| write enable=[YES] [NO]                  | 是否开放本地用户的其他写入权限                               |
| local umask=022                          | 本地用户上传文件的 umask 值                                  |
| local root=/var/ftp                      | 本地用户的 FTP 根目录                                        |
| local max rate=0                         | 本地用户最大传输速率(字节/秒)，0 为不限制                    |
| userlist enable=[YES] [NO]               | NO]匿名用户的最大传输速率(字节/秒 )，0 为不限制              |
| userlist deny=[YES] [NO]                 | 启用禁止用户名单，名单文件为 ftpusers 和/etc/vsftpd/user_list |
| chroot local user=[YES] [NO]             | 是否将用户权限禁调在 FTP 家目录中，以确保安全                |
| chroot list enable=[YES] [NO]            | 禁调文件中指定的 FTP 本地用户于其家目录中                    |
| chroot list file=/etc/vsftpd/chroot list | 指定禁锢文件位置，需要和 chroot_list enable 一同开启         |



**日志功能**

| 参数                          | 作用                                 |
| ----------------------------- | ------------------------------------ |
| xferlog_enable=[YES] [NO]     | 是否开启 FTP 日志功能                |
| xferlog_std_format=[YES] [NO] | 是否以标准格式保持日志               |
| xferlog file=/var/log/xferlog | 指定保存日志的文件名称，需要一同开启 |



#### **5.vsftpd 认证模式**

> vsftpd 作为更加安全的文件传输的服务程序，允许用户以三种认证模式登录到 FTP 服务器上。

- 匿名开放模式
  匿名开放模式是一种最不安全的认证模式，任何人都可以无需密码验证而直接登录到FTP服务器。这种模式一般用来访问不重要的公开文件，在生产环境中尽量不要存放重要文件，不建议在生产环境中如此行事。
- 本地用户模式
  本地用户模式是通过Linux系统本地的账户密码信息进行认证的模式，相较于匿名开放模式更安全，而且配置起来相对简单。但是如果被黑客破解了账户的信息，就可以畅通无阻地登录FTP服务器，从而完全控制整台服务器。
- 虚拟用户模式
  虚拟用户模式是这三种模式中最安全的一种认证模式，它需要为FTP服务单独建立用户数据库文件，虚拟出用来进行口令验证的账户信息，而这些账户信息在服务器系统中实际上是不存在的，仅供FTP服务程序进行认证使用。这样，即使黑客破解了账户信息也无法登录服务器，从而有效降低了破坏范围和影响



**具体的设置方式请查看参考[Vsftpd服务器](https://zhuanlan.zhihu.com/p/393007688)**



**常用命令**

```
sudo service vsftpd start  --开启服务
sudo service vsftpd stop   --停止服务
sudo service vsftpd restart    --重启服务
service vsftpd status   --检查vsftpd服务的运行状态
```













### 网络通信命令

```
ifconfig：查看网卡信息
ifconfig 或 ifconfig | more

ping：查看与某台机器的连接情况
ping ip

netstat -an：查看当前系统端口

搜索指定端口
netstat -an | grep 8080
```

### 重启网络

```
service network restart
```

### 关闭防火墙

```
chkconfig iptables off

或
 iptables -L;
 iptables -F;
 service iptables stop
```

### 修改文件权限

```
chmod 777
```

[详细解释](https://blog.csdn.net/qq_23329167/article/details/83856430?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522167961802716782427480599%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=167961802716782427480599&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~top_positive~default-2-83856430-null-null.142^v76^control_1,201^v4^add_ask,239^v2^insert_chatgpt&utm_term=linux%E5%B8%B8%E7%94%A8%E5%91%BD%E4%BB%A4&spm=1018.2226.3001.4187)

# 服务器地址：172.21.4.186

## 软件登录设置

```
用户名称：
gis-sys
root
arcgis
```

```
密码：统一为 giser2.5
```

|                           操作流程                           |                 步骤                 |
| :----------------------------------------------------------: | :----------------------------------: |
| ![image-20230323213221122](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232132160.png) |        连接主机，填写相关参数        |
| ![image-20230323213504384](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232135450.png) | 此页面表示登录成功，可进行图形化操作 |

| ![image-20230323213723544](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232137579.png) | 连接主机，填写相关参数                                       |
| :----------------------------------------------------------: | ------------------------------------------------------------ |
| ![image-20230323213823771](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232138800.png) | 连接主机，填写相关参数                                       |
| ![image-20230323213905573](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232139645.png) | 表示连接成功                                                 |
| ![image-20230323214044011](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232140078.png) | 通过xshell可直接登录xftp并直接连接服务器，进行管理           |
|                   用户：gis-sys  登录界面                    | 用户：root   登录界面                                        |
| ![image-20230323214208131](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232142174.png) | ![image-20230323214239161](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232142199.png) |



**用我的电脑进入服务器相信你们都会了就不教了**

![image-20230323222218053](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232222102.png)

| ![image-20230323222119177](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232221199.png) | ![image-20230323222134654](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232221688.png) |
| ------------------------------------------------------------ | ------------------------------------------------------------ |

## 更改权限方法

| ![image-20230323222341351](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232223391.png) | 这个代表的是返回上一级目录，点击此处可返回至最底层文件夹所在位置 |
| ------------------------------------------------------------ | ------------------------------------------------------------ |

**先用xshell登录服务器**

**再连接xftp**

**账号用root**

**进行两次返回文件夹操作**

![image-20230323222603250](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232226283.png)

**选择FTP文件夹，进入文件夹后选择文件夹，右键即可更改权限**

![image-20230323222549267](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232225307.png)

![image-20230323222623966](https://longchaohuo.oss-cn-hangzhou.aliyuncs.com/jj_img_for_typora/202303232226003.png)





