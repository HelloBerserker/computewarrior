上周六接的，做report的项目，做好了感觉又能做功能丰富的小工具了。包括，提交加班申请。生成加班情况报表，这个东西完全可以当个临时的数据库用。就连写程序都想着加班，好痛苦，好难受。还是那句话别忘了自身的发展。  
写好自己的代码。

### 2017年2月23日 11:26:32

> 今天一个bug写了一个多小时，原来DateTable的表头不能重复，有点像数据库的主键了，但是我让他重复了，居然不会报错提醒我  
> 所以一个bug写了几个一个多小时，真难。

### 2017年2月24日 15:07:56

> 接下来要用EPPLUS把数据导出，就是今天。

### 2017年2月25日 13:57:45

> 今天状态不怎么好，不过还是把导出xlsx的功能做出来了。今天把动态导出表头的功能也试着做一下。后天就考虑从不同库别抓取数据了。合在一起，然后交给景宇去测。

### 2017年2月27日 18:30:23

> 只能把一个个不同厂别抓出来的DataTable合在一起了，也是有点麻烦，不然今天都能把这个程式做好的。这么多个厂啊，要合好多个。F3,F4,F5,F7,ALL。一个个 DataTable，合个4下。哦，还有个是————最初抓出来的那个MO表如果行数为0,跳出不要继续进行后面的操作，省事

### 2017年2月28日 10:52:27

> 把不同DB数据和在一起的方法已经做好了，剩下的就是决定抓哪些DB的数据了。格式要换，取消自动换行。

### 2017年3月1日 16:29:06

> 美云的活真落了一个在我头上，还又接上了一个新需求，还真有点难，不想加班也要加班了。不能Counting stars,只能Counting dollars。

### 2017年3月2日 10:18:50

> 美云的那个需求，先按照他的需求抓，然后把箱号对应的数量后面处理出来。前面后面，抓来抓去，真是麻烦

### 2017年3月6日 09:42:58

> 想不到需求这么快就快做完了，MO\_VSN\_REPORT先交给景宇去测。多线程的等下搞定，C\#怎么可以不会多线程，自己的这个记事本有时间也可以优化一下，不然太low了，方法就用html或者自己使用xml，可以使用加粗，ul、ol标签，再下去都要自己做个编辑器了。也是有点interesting。

### 上午 10:39 2017/3/7

> 寻找一个异步抓取数据合并数据的方法，必须要异步抓取，不然很多程式我看都会卡死。

### 上午 10:22 2017/3/8

> 也别找什么异步的方法了，那个LOG\_ISN表有4000万行数据，我这样去抓，多少个线程也会卡死。

### 下午 3:27 2017/3/8

> 可以后台把一个个表缓存出来，然后search的时候就在里面找。这个不知道怎么样。

### 2017年3月21日 16:28:27

> MO\_VSN\_REPORT这个需求差不多快要完成了，学习了异步编程和多线程编程，对C\#更加熟悉了。同时别忘记基础知识的学习，自己还很多东西不懂，要多花时间，菜鸡互啄到最后，发现自己才是菜鸡。太残忍了，必须多加班学习。不学习不加班就是咸鱼。

### 2017年4月1日 09:56:30

> 都四月了，还是没有一个项目出来。起初是说要做个个性化壁纸的工具，现在发现完全可以用WallpaperEngine来做个HTML5和CSS3，js的静态网页。  
>   后来又想利用HTML做个记事本，结果发现Github使用的MarkdownLanguage这么好用，是否要放弃了，但是明显自己写的记事本样式会更加丰富，看起来更爽。

### 2017年4月1日 13:48:31

> 刚才看了一下消息，携程居然也要转JAVA，内心还是有一点波动的。C\#是没有哪里不好，可是国内的C\#开发环境不好，招不到高级的C\#开发。 JAVA人好招。  
>   不必担心C\#学了不好，少了一个携程，还那么多用.net技术的公司呢。连腾讯都在用，只要牛X甚至可以出国，不必担心没前景。

### 2017年4月3日 10:29:56

> 还是决定先学XML,然后网络编程，再后面就xaml和WPF,想学习新技术。希望后面需求别那么的多啊。

### 2017年4月3日 11:26:06

> git不会用，只会用svn,为什么不能提交啊。想提交一下这个还非要，打开SVN.

### 2017年4月4日 18:07:36

> 今天就有点残忍了，3倍工资没看多少代码，只是看了一下用存储过程怎么分页，倒是逛了一天知乎，明天继续加油吧。

### 2017年4月5日 09:27:16

> #### [逻辑查询处理阶段简介](http://www.cnblogs.com/qanholas/archive/2010/10/24/1859924.html)
>
> ---
>
> 1. **FROM**：对FROM子句中的前两个表执行笛卡尔积（Cartesian product\)\(交叉联接），生成虚拟表VT1
> 2. **ON**：对VT1应用ON筛选器。只有那些使`<join_condition>`为真的行才被插入VT2。
> 3. **OUTER\(JOIN\)**：如 果指定了OUTER JOIN（相对于`CROSS JOIN` 或\(INNER JOIN\),保留表（preserved table：左外部联接把左表标记为保留表，右外部联接把右表标记为保留表，完全外部联接把两个表都标记为保留表）中未找到匹配的行将作为外部行添加到 VT2,生成VT3.如果FROM子句包含两个以上的表，则对上一个联接生成的结果表和下一个表重复执行步骤1到步骤3，直到处理完所有的表为止。
> 4. **WHERE**：对VT3应用WHERE筛选器。只有使`<where_condition>`为`true`的行才被插入VT4.
> 5. **GROUP BY**：按`GROUP BY`子句中的列列表对VT4中的行分组，生成VT5.
> 6. **CUBE ROLLUP**：把超组\(Suppergroups\)插入VT5,生成VT6.
> 7. **HAVING**：对VT6应用HAVING筛选器。只有使`<having_condition>`为`true`的组才会被插入VT7.
> 8. **SELECT**：处理`SELECT`列表，产生VT8.
> 9. **DISTINCT**：将重复的行从VT8中移除，产生VT9.
> 10. **ORDER BY**：将VT9中的行按`ORDER BY`子句中的列列表排序，生成游标（VC10\).
> 11. **TOP**：从VC10的开始处选择指定数量或比例的行，生成表VT11,并返回调用者。

### 2017年4月11日 10:58:57

> 偶尔会忘记接下来要学点什么东西，先Xml，然后网络编程吧。

### 2017年4月14日 10:27:19

> 复制粘贴是最快的，既然他说了follow哪个页面我也不必浪费时间了啊。

### 2017年4月14日 14:41:16

> 这么凶残的代码也是醉了  
> 为什么要这么的无敌。**我这是在玩走迷宫还是找不同啊！**

```csharp
                                               }
                                           }
                                       }
                                   }
                               }
                               strKP = strKP1;
                           }
                       }
                   }
                   }
```

### 2017年4月15日 10:14:52

> 又开始了加班，一开始说要加班我是拒绝的，因为加班不是没状态就是有需求。我的责任心又不允许我停下手上的需求干其他的。加班也写不出好项目。
>
> ---
>
> _能不能不逛知乎_
>
> ### 2017年4月18日 11:06:01
>
> 昨天又接到了两个需求，今天完成了一个，还有一个是多DB还带着10道卡关，鬼知道这个礼拜能不能写好呵。

### 2017年4月19日 16:49:52

> 现在发现合箱的需求好做了，只要在device所在DB，isn所在DB和p1db做好转换就好了。只是CG\_STOCK又开始烦人了。不知不觉又快一周过去了，什么时候才能**Counting Stars**。

### 2017年4月24日 11:08:11

> 新的一周又开始了，转眼间又做了不少的需求。TO DO！  
>   DBnull不能转换成其他类型，Get!不能也不能**强制转换为String\(Convert.ToString\(\)\)**

### 2017年4月26日 16:39:03

> 在DateGridView的时候遇到了内存溢出，那时候出错的语句又没用循环递归。原来我只是改了单元格的值，这个操作每次都会调用数据绑定，绑定数据后又判断单元格的值，每次对变量进行赋值，而一赋值就报错了，因为每次触发数据绑定。

### 2017年5月2日 15:37:54

> 五月了，用户体验：交互体验，情感体验，感官体验。大家笑得都是有道理的，需求多起来谁管的上用户，用户怎么不考虑一下程序员体验 ，把需求提好点。

### 2017年5月3日 11:30:28

> hope is four letter work.say no more counting dollars we will be counting stars.

### 2017年5月5日 13:47:51

> 看到耦合度这么高的公共（_**public**_）方法，我真是不想复制粘贴啊,简直是辣眼睛。

### 2017年5月8日 13:02:43

> 转眼间就到了5月份，How time flies。

### 2017年5月9日 10:42:25

> CG\_STOCK那个需求终于更新了，留下的坑终于给填了，手上还有SFIS.KIRIN的SMART IN 和SMART OUT ，还有合箱页面。一大波需求正在接近。string是引用类型，int是值类型，我觉得用Int应该更快，为什么这么多方法还是用string做参数。

### 2017年5月9日 19:10:30

> > “五岁的时候人的记忆有五年，这时候过一年，到六岁时，记忆增加了五分之一。六岁到七岁，记忆增加了六分之一。七岁到八岁记忆就只增加了七分之一。以此类推，到了二十岁的时候，过多一年，记忆便只增加二十分之一。这一年的时光虽然没变，但是参照物变了。所以大家就感觉时间过得快了。可能等你六十岁的的时候，过一年记忆只增加六十分之一，那时时间就过得更快了。”

### 2017年5月11日 11:09:41

> 代码的效率不行。虽然这个人写的代码效率还可以，但是这个人写代码的效率不行。

### 2017年5月16日 08:40:18

> SortedList, dictionary, linkedList, Sequence, Stack, IEnumrable

### 2017年6月20日 10:05:22

> 要走了。

### 2017年8月21日 14:56:36

> 现在换了地方写代码，实现了暂时的目标。想想做个项目玩具项目也行，做什么好呢。  
> 搞个游戏是最好的，因为我现在没有云服务器了额。

### 2017年8月29日 16:31:43

> 周二迟到了，很难受。服务器弄了一个AWS的，12个月免费使用。FontAwesome的C\# cheetsheet也做好了，主要是int，char,string各个类型的隐式转换，看来打好基础真是必要的啊。还有国庆节要来了，想写个项目来的，想想做个啥子来啊。

### 2017年8月31日 11:31:43

> 越来越感觉到这具身体不适合现在的我了。晚上习惯了晚睡（躺床上还要玩下手机，通勤时间这么长因为地铁挤浪费了）。

### 2017年9月5日 14:05:45

> 因为不清楚FTP服务器的主动模式和被动模式，结果没配置好服务器。花费了很多时间。  
> 没有打开AWS服务器的50000-60000这些高位端口，这些端口是受安全组或者是防火墙控制的。不过今天配置了一个FTP服务器，还解决了AWS配置网站的问题。  
> \(1\) PORT（主动模式）  
> PORT中文称为主动模式，工作的原理： FTP客户端连接到FTP服务器的21端口，发送用户名和密码登录，登录成功后要list列表或者读取数据时，客户端随机开放一个端口（1024以上），发送 PORT命令到FTP服务器，告诉服务器客户端采用主动模式并开放端口；FTP服务器收到PORT主动模式命令和端口号后，通过服务器的20端口和客户端开放的端口连接，发送数据，原理如下图：

![图片](http://static.oschina.net/uploads/space/2011/0528/204156_vG81_97118.jpg?_=3607767)  
\(2\) PASV（被动模式）

PASV是Passive的缩写，中文成为被动模式，工作原理：FTP客户端连接到FTP服务器的21端口，发送用户名和密码登录，登录成功后要list列表或者读取数据时，发送PASV命令到FTP服务器， 服务器在本地随机开放一个端口（1024以上），然后把开放的端口告诉客户端， 客户端再连接到服务器开放的端口进行数据传输，原理如下图：

![](http://static.oschina.net/uploads/space/2011/0528/204218_G2gD_97118.jpg?_=3607767)

2.两种模式的比较

从上面的运行原来看到，主动模式和被动模式的不同简单概述为： 主动模式传送数据时是“服务器”连接到“客户端”的端口；被动模式传送数据“客户端”连接到“服务器”的端口。

主动模式需要客户端必须开放端口给服务器，很多客户端都是在防火墙内，开放端口给FTP服务器访问比较困难。

被动模式只需要服务器端开放端口给客户端连接就行了。

3.不同工作模式的网络设置

我在实际项目中碰到的问题是，FTP的客户端和服务器分别在不同网络，两个网络之间有至少4层的防火墙，服务器端只开放了21端口， 客户端机器没开放任何端口。FTP客户端连接采用的被动模式，结果客户端能登录成功，但是无法LIST列表和读取数据。很明显，是因为服务器端没开放被动模式下的随机端口导致。

由于被动模式下，服务器端开放的端口随机，但是防火墙要不能全部开放，解决的方案是，在ftp服务器配置被动模式下开放随机端口在 50000-60000之间（范围在ftp服务器软件设置，可以设置任意1024上的端口段），然后在防火墙设置规则，开放服务器端50000-60000之间的端口端。

主动模式下，客户端的FTP软件设置主动模式开放的端口段，在客户端的防火墙开放对应的端口段。

### 2017年9月6日 15:17:13

多线程还是能提高程序运行效率的，刚才编写的测试样例中。因为网络原因，10个进程同时抢网速，然而在网不好的时候，返回的结果还会更慢。  
多线程还是得看配置，要网速够好，配置够高，不然抢占CPU资源的时候也是一样的不能提高效率。多线程和异步都提高了UI的响应能力，能分出心做其他东西。

### 2017年9月8日 14:57:40

今天就8号了，还有几个礼拜就放假，还是没想到要做个什么项目耍耍。说好的玩具项目叻。

### 2017年10月13日 09:20:32

今天又是星期五，时间真的过的好快啊，买了个腾讯手环。*腾讯手环已经丢了，过年坐火车的时候*

> 猝不及防的弯道，还好我装了龙头凤尾。

这句话好逗啊。

### 2017年11月8日 09:54:38

WebApi和Redis功能实现那边也已经没问题了，现在要整合到一起。先写WebApi吧，先写服务端，再写客户端。

### 2017年11月17日 17:01:01

Redis服务器也已经做好了，刚刚测试了有用，就是不能远程访问，而且密码也没有用,redis已经Ok了。

### 2018年4月10日 17:21:30

N久没用这个了试试看。今天又迟到了啊，还出了一身的汗，现在闹钟是不管用了吗。这里加个一段这是SSH协议那个库加的。stupid,HTTP还要尝试一下,test http。

### 2018年4月12日 17:13:13

终于熬到了周四啊，这周不容易，发现TortoiseGit也挺好用的，可以不输命令。如果分支多，明显用git快很多啊。到底我哪个是用ssh的啊，好像是这个哦。