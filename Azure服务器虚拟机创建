# Azure服务器虚拟机构建
如题，在林佬的帮助下，我获得了一个Azure学生优惠的服务器，我在服务器上申请了一个虚拟机，特此记录一下如何申请虚拟机。

---
## Azure界面
![Azure首页](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-03_20-09-24.png)

点击主页，可以看到你所拥有的虚拟机及创建虚拟机的选项
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-03_20-39-12.png)

点击创建虚拟机，进行创建

---
## 虚拟机创建
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_11-33-31.png)  

如界面所示，共有：**基本、磁盘、网络、管理、监管**等配置界面
对于一般的配置来讲，我们只需要对前三个界面进行配置，下面进行分部讲解。

### 基本界面
![配置基本界面](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_10-44-03.png)  

**重点解析**
1.  新建资源组名称，该资源组包含你的虚拟机等内容。一个资源组可以重复进行使用。
2.  区域选项有很多种，但是中国大陆建议选择East Asia，即香港服务器，延迟更低。
3.  可用性区域选择如下图所示的**无需基础结构冗余**，方便后面的网络配置。     
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_10-44-35.png)  
4.  映像即镜像，可以自选所需的操作系统。
5.  大小即内存大小，学生认证后选择1G。
6.  **用户名一定要记住，以后需要用户名来登录虚拟机**
7.  其余如密钥选项不变。
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_10-47-32.png)

### 磁盘界面
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_10-48-46.png)
**重点解析**
1.  磁盘大小，学生认证后选择64GB
2.  其余选项不变

### 网络界面
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_10-51-53.png)
如图所示，首先进行虚拟网络搭配，虚拟网络名称为“虚拟机名称+vnet”(vital net)。
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_10-54-01.png)
配置公用IP，选择新建，如图进行创建，**一定要选择动态IP**

**其余几个配置界面无需更改，略过**

### 创建虚拟机界面
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_11-00-13.png)  
配置好的界面如图所示，点击创建  
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_11-03-05.png)  
如图所示，创建成功。  
**此时会下载下一个ssh密钥，一定要保存下来。**  
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_11-03-43.png)  

**至此，虚拟机配置完成**

---
## 虚拟机登录
1.  将ssh密钥文件复制，在你的C盘的用户(administrator)下创建一个 **.ssh** 文件夹
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_11-04-25.png)
2.  将刚刚保存的密钥复制到此文件夹
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_11-04-33.png)
3.  进入刚才所配置好的虚拟机界面，找到它的公共IP地址用于登录虚拟机
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_11-06-58.png) 
4.  进入power shell，输入：
`` ssh -i **密钥文件地址 虚拟机用户名 @公共IP地址``登录虚拟机
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_11-07-50.png)

例子：
`` ssh -i C:\Users\lee18\.ssh\test_key.pem testt@20.255.96.78 ``

5.  登录后的界面如图所示：
![](https://github.com/Augenstars/legendary-giggle/blob/main/%E5%9B%BE%E7%89%87/Snipaste_2024-07-04_11-08-08.png)

至此，虚拟机配置结束，完结撒花  
以此纪念我的第一篇GitHub文档  
前路漫漫，我会更加努力  
**2024.7.4  21A 5019**  
