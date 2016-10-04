#MyPCQQ - 错误
>这里收集了一些关于MyPCQQ使用过程中可能出现的错误以及一些你可能需要的解决方案。如果您遇到问题，这里也许会有你需要的答案。

#
>写文库真心很累啊有木有！！！
如果每个人帮我写一道题，那么这世界就充满爱了有木有！！！
骚年想在这里留下你的名字么有木有！！！
还不快发送邮件到admin@mypcqq.cc啊有木有有木有有木有！！！















































[TOC=2,4]
##启动之前的问题
####1、MyPCQQ可以开几个？可以多开吗？
我们没有限制MyPCQQ在同一台机子内多开，也就意味着您可以这样做。但是多开会引起各种各样的问题所以建议尽量不要多开。
####2、MyPCQQ的运行环境？
我们建议您使用Windows 10来作为使用环境。另外我们目前还保持着对于Win8/7的兼容。
对于Windows Server 系列的系统，我们建议使用2012或者2016.***极力不推荐使用2003***

####3、MyPCQQ添加Q的上限是多少？
19个。
>Q：我记得以前是无限的啊？
A：是的，那是曾经。为了打击非法用途，特地做了这个限制。
Q：为什么你们要这么做？
A：<font  style="font-size:7px;">
>MyPCQQ是是一款永久免费的信息框架 面向个人普通用户.不欢迎用于**黑产灰产黄赌毒PC蛋蛋算账下注群发群加各式量产或其他违法犯罪或犯罪边缘相关内容**.违者必究.
>经过一定时间的观察发现：这些人通常会频繁重启框架/频繁更换ip/带参启动/添加很多Q。所以我们针对这些行为做了一些限制。
>很抱歉目前无法在文档里告知阈值，因为阈值会随时调整。
所以再次警告这些人们，不要试图使用MyPCQQ歹做非为。后果就是“必究”，不论任何方式。良好的互联网环境和秩序需要我们共通维护。
></font>

##启动过程中的问题
####1、提示：插件载入失败/未公开任何处理函数
![](image/56aa1a4039054.png)
原因：
1、被杀软或者各种安全软件拦截
2、插件本身有问题

解决方案：
1、卸载或退出安全软件、杀软后重新下载。
>Tips：对于这种情况，把插件添加到白名单内是无效的。因为插件已经被杀软破坏过了，自然无法载入。

2、反馈给作者。


####2、提示：发现调试器或Core.exe主程序被非法修改

解决方案：把IDE或调试器关了。或再次重开
>Tips：MyPCQQ自带一定的反调试措施。如果您尝试调试程序，造成的后果由您自己承担。

####3、症状：一点开就闪退
原因:
1、杀软拦截
2、插件载入过程中崩溃。
解决方案：
1、卸载或退出安全软件、杀软后重新下载。
>Tips：对于这种情况，把软件添加到白名单内是无效的。因为软件已经被杀软破坏过了，自然无法正常载入。

2、挨个插件从Plugin文件夹中移除、删掉测试。

####4、提示：Not found the kernel library or the kernel library is invalid or the kernel library of this edition does not support DLL!
![](image/56adde5fbf58b.png)
原因：某个/某些插件没有静态/独立编译
解决方案：挨个插件删除排查


####5、Err10004:受到新浪云防火墙拦截或被封禁IP段

原因：最近有过**作死**行为。
>[info]还是要给**作死**下个定义......
1、同一机器（码）一定时间内多次更换ip
2、同一机器频繁重启<font  style="font-size:7px;">①</font><br />
>
>①：如果您是因为插件调试被封而来到这里，那么提醒你，MyPCQQ可以热安装或者热卸载插件的。详情请看添加插件第三部分。
>
><font  style="font-size:7px;">再啰嗦两句：我们为什么要这么做？
>MyPCQQ是是一款永久免费的信息框架 面向个人普通用户.不欢迎用于**黑产灰产黄赌毒PC蛋蛋算账下注群发群加各式量产或其他违法犯罪或犯罪边缘相关内容**.违者必究.
>经过一定时间的观察发现：这些人通常会频繁重启框架/频繁更换ip/带参启动/添加很多Q。所以我们针对这些行为做了一些限制。
>很抱歉目前无法在文档里告知阈值，因为阈值会随时调整。
所以再次警告这些人们，不要试图使用MyPCQQ歹做非为。后果就是“必究”，不论任何方式。良好的互联网环境和秩序需要我们共通维护。
></font>

所以原因很明确了：
1、同一机器（码）一定时间内多次更换ip
2、同一机器频繁重启

解决方案：
等待24小时-48小时后自动解封。

>若有作死行为仍然会被封掉的，然后就这样循环了。
附赠：
下载之前你应该清楚的东西
https://f.mypcqq.cc/thread-4274-1-1.html
<br />(出处: MyPCQQ官方站)

####6、界面完全乱码，一坨什么鬼
就像这样↓
![](https://mypcqqupload.b0.upaiyun.com/forum/201609/17/212647n6in300s80q0rzsn.png)
![](https://mypcqqupload.b0.upaiyun.com/forum/201609/17/212652tdfuzdffxk2d5u2s.png)



































我当然知道为什么嘛~
MyPCQQ系易语言编写，系统内部的文本是灰常本土化滴ANSI的储存方式。
这一类问题通常发生在海外机器上，**因为系统没有中文语言包**（里面包含ANSI的解码）。
所以也就很明确了，**安装中文语言包即可解决**。不出意外的话，Windows自带的Updata的可选更新里面就有。当然微软官网也有。
>科普：为什么这种机器开网页却可以显示中文呢？
网页的编码和软件不一样的！
网页的编码一般以Utf-8为主，这种编码兼容多国语言（包括日文俄文泰文等等等等），但是标准出来的比较晚。而ANSI则是中文加入电脑的时候就出现了的（看起来和GB2312差不多？），比较早，比较落后。
那为什么还没被淘汰呢？
UTF-8每个字都要拿出一定的字节取储存头部ROM信息。而ANSI没有这些。也许你听不懂什么叫“ROM信息”，那就举个例子：ANSI就是头，而UTF-8则是带了头盔。能更加保证安全（装更多的语言）但是略微臃肿（头大）（也就是要头ROM信息）。所以用ANSI的一个好处就是极力减少体积。
——其实刚刚那些不是理由，软件用ANSI完全看是用什么语言的！否则就需要额外处理喽！易语言作为国产第一语言，不用母语编码（ANSI才怪）。


















##登录过程中的问题
####1、提示：刷刷刷一排UDP服务器可用性测试->无回音
![](image/56aa1e0d68239.png)
>Tips：布局可能和实际情况不符，但提示基本一致。

原因：
1、VPS安全策略引起
2、网络环境UDP数据包不通
解决方案：
1、找到Windows控制面板 - 搜索“本地安全策略”，仅保留图示三条记录，其他的安全策略删除。
![](image/56aa1ed5a9b7e.png)


####2、提示：登录->接触服务器->失败 服务器无响应

1、软件本体被破坏、自身校验未通过。建议从官网下载最新版的MyPCQQ运行。
2、IP或机器码被封导致云校验不通过。

解决方案：
1、卸载所有插件
2、重新下载软件覆盖
3、关闭杀软等【白名单无效 白名单无效 白名单无效 重要的事情说三遍，只要接触到了杀软就肯定被破坏（也就是所谓的无毒化）】并重新下载软件并覆盖。



>[info]如果是旧版的话...
原因：
网络不稳定或腾讯服务器宕机。
解决方案：
重试或重连网络。

####3、提示：登录->接触服务器->反回包异常FD->服务器载荷过高.需要更换服务器
原因：
网络不稳定或腾讯服务器宕机。
解决方案：
重试或重连网络。

####4、提示：登录->帐号被回收或冻结
解决方案:去 安全中心（http://aq.qq.com ） 登陆机器人号码处理。


####5、提示：登录->密码不正确
解决方案：作为高智商机器人这种低级错误是肯定不会犯的惹:(一定是亲输错了呢
另外需要注意密码有效长度 太长的密码不一定能全部敲进去。


####6、提示：登录->验证密码流程->服务器返回提示:需要解除设备锁 / 登录->验证密码流程->QQ受到设备锁保护无法登录。
请至aq.qq.com或登录手机QQ->设置->关闭设备锁
解决方案：aq.qq.com或手机QQ设置里关掉设备锁


####7、提示：登录->验证密码流程->00DE验证
解决方案:若出现验证失败的提示请至用户组群联系作者以解决 必要的情况下可能需要您的机器QQ+密码或借用您的VPS


####8、提示：返回时间戳异常&本地时间于服务器时间偏差过大
原因：
1、系统被从休眠\睡眠里唤醒。
2、本地时间不准确。
解决方案：
1、重开解决。
2、电脑右下角系统时间自己调整一下 误差尽量在2分钟以内。然后重开。


####9、提示：协议版本过期 请至官网下载最新版本
解决方案:若为突发提示请耐心等待更新


####10、提示：私有_SessionKey获取失败
解决方案:1、尝试重开 2、删除Cache目录以及其所有文件


####11、提示：登录->获取会话秘钥->失败
解决方案:1、尝试重开 2、删除Cache目录以及其所有文件

####12、提示：在class->在执行登录过程中发生了一个异常
解决方案:在反馈区反馈给我们





































##运行过程中的问题


####1、提示：似乎处于被屏蔽群信息状态，建议更改密码后重新登录
原因：
1、被所在群禁言
2、帐号被腾讯方面临时性屏蔽信息。
>Tips：为什么账户会被屏蔽？
可能的原因：
1、发送信息过快 
2、信息中包含过多连接、类似广告信息、群发信息 
3、帐号近期被多次举报冻结 
4、帐号被多次冻结且未更改密码 
5、可信度较低的新Q 
6、异地登录

解决方案：
1、解除禁言
2、建议更改密码后重新登录、更换老QQ、开会员、若异地登录则需要多挂几天。
>Tips：异地的鉴别标准是登陆的IP地址变化的差异。如果在VPS/服务器内登陆那么会认为你是在VPS/服务器所在的地理位置登陆的。因此如果从本地挂机突然转移到服务器上很有可能遭遇屏蔽。

.
>Tips：若上述方案均无法解决请检查目录下set.ini内的通信协议设定 若为TCP请清空并转到问题：1、提示：刷刷刷一排UDP服务器可用性测试->无回音
通信协议=UDP
服务器IP=111.161.88.20


####2、提示：无法找到指定DLL库文件 "xxxxxxxxxxxxxx.dll"中的命令xxxxxx
1、若为Message.dll 可能原因为文件版本过老：重开更新至新版或者重新下载即可解决。
2、若为其他DLL 则极有可能为某插件的瞎调用或文件缺失：可以尝试关闭杀软亦或者反馈给作者。


####3、提示：插件:XX插件对Api_XXXXX错误的调用
>包括但不限于这些：
插件:某某插件对Api_Reply错误的调用->不正确的回复类型:XXXXX
插件:某某插件对Api_SendMsg错误的调用->不正确的回复类型:XXXXX
插件:某某插件对对Api_Reply错误的调用->内容为空
插件:某某插件对对Api_SendMsg错误的调用->内容为空

原因:插件本身问题
解决方案:反馈给插件作者




####4、提示：提示存在类似群发行为。发送取消
原因:插件的原因
>Tips：MyPCQQ禁止任何群发行为 无论是向群还是好友还是讨论组还是临时会话。

解决方案:反馈给插件作者或放弃使用该插件、停止群发行为




####5、提示：提示图片上传失败
原因：网络不稳定或无法取得图片数据
解决方案：检查网络环境、检查插件




>[info]编写:Eghuai
>[info]润色:freejishu & a632079
>[info]审核:Eghuai
>[info]最后更新:2016.10.03