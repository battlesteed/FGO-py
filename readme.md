> 抽了4个小时的友情点才出了4张活动礼装,还手抖卖了3张  
> 人这东西还真是能力有限啊  
> 我从短暂的人生当中学到的就是  
> 人越是写代码,代码就越可能因意料之外的情况而失效  
> 要成为超人的存在才行啊  
> 我不做人啦!JOJO!  

# "智能战斗不间断,不靠礼装不用拐"的FGO全自动脚本  
当前版本[v3.4.2](#版本记录-Version-Logs)  
仅适用于安卓简体中文版本  
开学快乐  
虚拟机vmwareWorkstation 模拟器Bluestacks 虚拟摄像头e2eSoftVCam 虚拟声卡e2eSoftVSC 已就绪  
祝间桐樱生日快乐  
GitHub项目地址:[https://github.com/hgjazhgj/FGO-py/](https://github.com/hgjazhgj/FGO-py/)  
抽奖池抽友情之类的功能可以用airtest轻松实现,没有必要再从头写过,因此大概率不会更新此类功能,除非将来对效率有较高需求  
当前版本更新较快,因此**不建议fork**  
你可以star以便日后访问,或者直接把本项目地址加入浏览器收藏夹  

# 警告  
**[<<哔哩哔哩游戏平台用户协议V1.0.0>>](https://yhxy.biligame.com/)第11条第2款规定:**  
**用户不得通过不正当的手段或其他不公平的手段使用本平台游戏、本平台服务或参与本平台活动。**  
**用户不得干扰本平台正常地提供游戏和服务，包括但不限于：攻击、侵入本平台的网站服务器，或集中时间段内以超出正常用户登录需求的高频率登录或尝试登录服务器从而使网站服务器过载；破解、修改本平台提供的本平台游戏程序；攻击、侵入本平台游戏的服务器/游戏服务器端程序或使游戏服务器过载；制作、发布、传播、使用任何形式的妨碍游戏公平性的辅助工具或程序(包括但不限于“外挂”, “外挂”是指独立于游戏软件之外的，能够在游戏运行的同时影响游戏操作的所有程序，包括但不限于模拟用户操作、改变操作环境、修改数据等一切类型）。用户不得：利用程序的漏洞和错误(Bug)破坏游戏的正常进行或传播该漏洞或错误(Bug)；不合理地干扰或阻碍他人使用本平台所提供的游戏和服务；通过异常或者非法的方式使用本平台游戏(包括但不限于利用本平台游戏登录游戏私服)；使用异常的方法登录游戏（包括但不限于使用非本平台开发、授权或认可的第三方软件、系统登录游戏）、使用网络加速器等外挂软件或机器人程序等恶意破坏服务设施、扰乱正常服务秩序的行为；修改、翻译、注释、整理、汇编、演绎本平台游戏；利用本平台游戏或者线上游戏系统可能存在的技术缺陷或漏洞而以各种形式为自己及他人牟利（包括但不限于复制游戏虚拟物品等）或者从事其他不正当行为等。**  
**由于使用本脚本而导致的包括但不限于上述各项的损失本人概不负责,您下载并使用该脚本即代表您已知晓使用脚本可能带来的风险并愿意承担可能出现的后果,望周知**  
<del>但是fgo内部的用户条款好像没有限制脚本的使用</del>  
***  
# 使用说明 Instruction  
脚本可以后台运行  
分辨率最好是长1920或宽1080,其他分辨率亦可  
使用了以下外部库:  
`configParser` `airtest` `PyQt5`  
其他包含在上面这三个库里面的外部库未单独列出  
速览脚本功能,运行fgoGui.py,大部分说明也在ui里  
本脚本的代码部分仅有`fgoFunc.py`是fgo算法相关的  
这个脚本会自动放技能(默认不用技能),自动放宝具(默认充能满就直接放宝具),自动选卡(优先三色chain,否则优先红卡).合理设定后实战7-12回合能够刷完无限池终本  
如果要三回合速刷,请自己写一个战斗函数  

我的联系方式  
qq 979449732(加好友请说明来意  
email huguangjing0411@geektip.cc  
关于airtest首次安装/重新启动带来的本脚本中没有考虑到的问题请提交issue  
有任何技术问题或bug反馈或本readme中有任何包括但不限于错别字语法错误描述错误的问题请联系,觉得有帮助请为我star  
无论通过什么方式反馈bug都请附上出错traceback等必要的信息  
**没有标明免费的东西都不是免费的**  

又tm有憨憨上来就"大佬我不会用请教教我".  
如果你瞬间理解了上面这句话的含义,就不必看本部分剩下的内容  
我乐意回答一些技术问题,但没有义务提供教学.为使耳根清净的最好方法就是收费,故制定以下政策  
关于本脚本算法及实现之外的问题(包括但不限于adb工具/python语言/win32相关/特定设备调试)不在支持范围内,对于相关问题的解答可能不是免费的.  
如果确实需要帮助,请发送邮件到我的邮箱huguangjing0411@geektip.cc  
具体的收费渠道还在思考中  
从解决一封邮件中的零碎的小问题到帮你调试到你的设备能用为止可能会酌情收取一颗圣晶石到一单(6-518RMB)的费用.  
建议您仔细阅读readme,尝试使用搜索引擎来解决您的问题,以免给您带来不必要的损失.谢谢.  
## 助战 Friends  
你需要事先将你期望的各种助战的样子截图为png放在image/friend下,参照image/friend/unused中的文件,如果image/friend目录下没有png文件,就选取好友列表中的第一个  
**被截图范围都应该可以点击来选中该好友**  
助战截图的文件名中若有下划线'\_',且下划线之前的部分为km,ml,cba,则代表好友就挂的是孔明,梅林,十八岁美少女,这会影响助战技能的使用  
## 快速查错引导 When Error Occurred  
+ 游戏是否已经运行  
+ 路径中是否有空格  
+ 游戏画面是否足够大足够清晰  
+ 手机屏幕是否点亮  
+ 相关技能宝具参数是否正确  
+ adb的连接是否有效  
+ 设备是否被airtest支持  
+ 是否看到了命令行窗口  
+ 模板图片是否正确  
+ 你的手机是否运行流畅  
+ 当前场上从者与脚本中的从者是否对应  
+ 该错误是否重复出现  

如果以上问题的答案均为"是",请按照上述的方式联系我  

# 版本记录 Version Logs  
## 2020/03/05 v3.4.3  
更新:所有3.3.0版本的功能全部恢复  
优化:设备连接懒加载,先记录序列号,要用时再更新对象  
你甚至可以先手动输入一个并不存在于设备列表中的序列号,然后再连接设备  
重构部分代码,看着舒服,用着也舒服  
## 2020/03/05 v3.4.2  
更新:基本功能基本稳定,多设备兼容性也没有问题,但仍有待优化  
airtest偶尔会莫名其妙出错,并且是那种进程直接崩掉一点信息不给的  
迟早有一天我得把airtest库给阉了重构,源代码越看越气  
完全移除了win32引用  
增加了窗口置顶的功能  
## 2020/03/03 v3.4.1  
更新:延时调整  
当前的目标是先让代码跑起来,原有的功能之后再补  
关于airtest首次安装/重新启动带来的本脚本中没有考虑到的问题请提交issue  
有些地方延时是数帧数卡得正好的,可能你的电脑一卡就出问题了  
## 2020/03/02 v3.4.0  
更新:我已经基本搞明白了airtest安卓部分的工作原理,现在已经用上了airtest库进行截图与触摸,效率奇高  
但是现在点得太快了,又得手动延迟  
airtest最大的问题就是基于模板识别的点击效率太低,并且难以修改参数,这应该是处于通用性作出的牺牲  
airtest最大的优点就是把所有高效的底层交互整合到了一起,一步就能到位  
因此无论是谁移植到谁那里都应该是用我的识别和airtest的IO  
我看airtest的源码写得有点臃肿,有空把它精简一下  
另外,我用的是airtest的底层接口,这些接口好像并没有出现在官方文档里,因此可能出现错误  
由于不同版本的adb间会有冲突,所以现在统一使用airtest自带的adb  
这样就可以去除win32库和大量命令行调用  
由于截图不用win32了,所以也去除了其他附属品,易用性略有下降,但是稳定性提升  
现在设备序列号是写在代码里的,你得手动更改  
ui里面那些过时的代码已经被注释掉了,会在之后的更新中慢慢补齐  
## 2020/03/02 v3.3.0  
使用了基于底层设备的`swipe`,消除`swipe`的后摇.所以当前版本只能用于Bluestack模拟器  
由于进程间通讯的关系比原有的慢  
更改了助战截图,先前版本的截图选取的范围过大以至于包含了威力加成图标而导致匹配失败  
## 2020/03/02 v3.2.2  
补充了状态栏信息  
现在几乎所有的说明都可以直接在ui里看到,所以大幅精简了readme  
我希望readme变成广告,展现我的脚本的特点而非具体实现  
## 2020/03/02 v3.2.1  
bug修复:
`swipe`在上个版本误删了一些字符  
新增:
添加了菜单栏和状态栏及相关信息  
## 2020/03/02 v3.2.0  
ui改版,稳定性优化,添加了一些功能  
在绝大多数情况下,安卓的信息并不需要每次都检查改变,就像各窗口句柄一样.因此更改了ui  
有时你需要更改助战模板,添加了一个按钮使得现在你不需要重新启动应用就能完成更改  
注意:当前的一些功能可能对于错误的输入产生难以预料的反应  
## 2020/03/01 v3.1.9  
优化:情人节活动不能在游戏内筛选掉巧克力礼装.现在到了chooseFriend函数重见天日的时候了  
添加了相应活动礼装的截图,增大了每次刷新助阵页面前识别的页面数量以应对mix职介.  
如果你确定你只需要在特定职介中筛选,请自行调整代码,但是请注意两次刷新之间需要时间间隔  
## 2020/02/28 v3.1.8  
微乎其微聊胜于无的小改动  
修订readme  
我仔细地研究了airtest的工作原理  
minicap采集屏幕的原理很简单:通过ndk的截屏接口不停的截屏并通过socket接口实时发送,这样客户端便可以得到一序列的图片流,图片流合成后就成为视频  
我不需要实时显示,因此minicap就截一张图时应该和win32的截图差不多  
STF框架对于点击,拖拽等操作比adb快得多  
细节部分有待进一步学习.等我什么时候研究透了,就可以更快乐地跑脚本了  
## 2020/02/27 v3.1.7  
bug修复:开始创建线程前将熔断器复原,否则熔断后无法继续操作  
## 2020/02/26 v3.1.6  
bug修复:选卡报错  
先前的版本会在场上队员不满三名时ListIndexOutOfRange  
此bug可能是v2.10重构时留下的  
优化:将一些列表改为了生成器,应用了(可能)更高效的选卡算法  
本以为sorted是快速排序,相同颜色的指令卡有多张时不会枯燥地选排在前面的了,结果发现用的是稳定的归并  
更改:现在宝具优先级越大越先用  
## 2020/02/24 v3.1.5  
优化:从者头像识别阈值修改  
说明:通过今日对数百场战斗的分析,当从者未变时,匹配结果约为1e-9,不超过2e-3.当从者改变时,匹配结果约为0.25,不低于0.08  
因此看起来取几何平均值是比较合适的  
但是有些从者长得比较歪,实际框选的区域包含了大量背景;又有些从者长的比较像(比如黑骑呆和伊莉雅).因此实际取值仍有待进一步优化  
二次元人脸识别?要是有现成库的话可以考虑一下,不过我觉得现有功能够用了  
## 2020/02/16 v3.1.4  
bug修复:现在当hFgoWnd最小化时启动脚本不会把脚本窗口移到屏幕外面去  
对于最小化的窗口,GetWindowRect返回[i-32000for i in rcNormalPosition]也就是说,如果你不幸拥有一个分辨率高于32000*32000的显示屏,就可能在相关win32的判断上出问题  
<del>ロン！国士無双！-32000</del>  
bug修复:有些应用,尤其是游戏,不允许消息队列操作,此时不应让窗口弹出打扰用户,所以在setForeground里加了一个try  
优化:调整了tab顺序  
## 2020/02/14 v3.1.3  
杂七杂八的修改:  
处理了工作路径的问题,不依赖调试器设置工作路径(我才发现双击运行会报错)  
现有的7个队伍设置差不多够了,新建/重命名/删除等功能也不见得常用,如果要修改的话就手动改config文件吧,不想写代码了,删库跑路  
确认了Tab顺序  
试图减少了各ui文件的体积(-40%)  
## 2020/02/14 v3.1.2  
bug修复:有关类,列表生成式,eval之间命名空间继承所带来的bug修复  
bug修复:修复了宝具设置不生效的问题,这一bug可能是v2.10.3重构时留下的  
即将更新:编队设置的新建/重命名/删除等功能.代码已经写好了,但是效果有点不友好,所以相关控件被改为了不可编辑不可点击  
## 2020/02/12 v3.1.1  
bug修复:保证setForeground能正常执行  
优化:修改了Key映射,以应对boss血条与小兵血条不在一行里的情况,从上到下从右到左依次为dangerPos0-5,按键为小键盘9-4  
优化:你可以看见你点过哪个编队按钮  
"一个控制台窗口+一个ui"的布局基本确定,我希望移动动其中一个窗口时另一个跟着动  
## 2020/02/12 v3.1.0  
功能移植  
在以前版本中,我可以一边挂脚本一边修改代码,因为代码会在执行开始时全部载入内存  
但是现在由于线程之间共享内存,你可以战斗途中变更各项配置,如果你在两个设备上用相同的队伍打同一个图,你甚至可以在这两个设备间切换  
这究竟是好是坏有待实践证明,目前我认为应该删除这一特性  
但是,想要删除这一特性比较困难.首先我想到的是改为多进程,但是我希望进程退出时对ui进行变动,而Qt的一堆控件都是不可序列化的...  
所以**多进程**是不可能的,也无法利用多进程进行挂起或中断  
再者就是将各项配置都作为参数传入战斗函数,这将大幅重构代码  
还有就是强行禁止一些更改,这样就使用体验极差  
当然究极的解决方案是存在的,那就是搞一个服务端和客户端然后进程间交互,但是这对于一个小项目而言负担过重  
Qt好像有他自己的线程库Qthread,看看能不能解决这个问题----不能  
脑阔疼  
最后还是从进程与线程的区别入手,创建线程前拷贝一份变量,这样,我的线程有了属于他自己的内存.蠢,但是有效  
挂起/中断的功能也用了很原始的实现,但是绝对不会出问题  
## 2020/02/12 v3.0.0  
ui基本定型,基本功能基本生效.  
之后还会移植一些功能  
修订readme  
在开发中遇到了以下问题:  
1. 当`app=QApplication(sys.argv)`执行完毕后,Qt将系统缩放倍率强行调整为1.  
2. QtDesigner里面应用layout的显示效果和预期相去甚远.  
3. python的线程无法挂起或中断,目前要取消脚本运行必须关了整个应用重开  
## 2020/02/11 v3.0.0beta
我打算开始写ui了  
## 2020/01/31 v2.10.10  
代码结构更改,无实质性变化  
我才发现函数定义本身就是可以挤在一行里面的  
## 2020/01/30 v2.10.9  
加入英文readme  
<del>xjb乱写了一个ui之后说不定用得上</del>本来想搞个ui的但是测试到一半发现比直接改代码麻烦得多,就不搞了...但是今后可能会向代码中添加一些接口以便ui访问  
bug修复:修改了一些写代码时手抖留下的错误  
## 2020/01/22 v2.10.8  
优化:又把所有代码塞进一个文件里了,方便交互  
负优化:在`hWnd`初始化的下方加了一行被注释掉的代码,方便那些经常换设备/模拟器的用户  
现在所有启用中的代码少于200行  
## 2020/01/21 v2.10.7  
bug修复:彻底修复了先前版本存在的宝具充能检测方式存在的不稳定不兼容因素  
说明:录屏数了一波帧数,从按下选课按钮到普通指令卡加载完毕需要正好0.5秒,然而按下选课按钮到宝具卡加载完毕需要2.17秒,宝具充能条闪烁周期为1.62秒.因此,每隔0.81秒检测一次就可以保证任意连续两次检测中有一次检测中宝具条的亮度大于从最暗变到最亮区间时间中点的亮度.实际使用时考虑一波误差和截图运算所需时间,取40%亮度值.最暗,最亮和实际使用的亮度阈值的截图在  
另:`isHouguReady`现在应该在选卡之后运行,整合了之前的`isHouguSealed`函数,又压缩掉了一堆代码,并且由于短路运算符的关系效率应该比之前高一些  
另:严格来讲,亮度指的是`0.3*R+0.6*G+0.1*B`,但我的代码中就暴力地`(R+G+B)/3`,反正也是严格递增的,效果相同  
另:上一个版本的更改是完全错误的,只是碰巧圣诞节的几个本背景偏白才有效  
## 2020/01/20 v2.10.6  
优化:多设备兼容性优化,也可能没有优化,也可能负优化,更改了`isHouguReady`函数    
说明:随便网上找了个安卓投屏软件在我自己的手机上测试了一波.全屏显示要会员?C语言写了个脚本强行全屏显示.勤劳与智慧的天朝人民是绝对不会给你一分钱的!转念一想我的脚本现在已经不用全屏了啊...然后这个投屏软件有四个标题类名都一样的子窗口,所以我还得在每次投屏后手动填写句柄值...垃圾软件毁我青春!  
另:`isHouguReady`函数是当前唯一一个像素识别而非模板匹配的函数,之后可能还得改  
## 2020/01/20 v2.10.5  
bug修复:现在fgo_shell内的初始化部分能正确地获取尺寸及缩放信息  
说明:`adb shell wm size`会返回通常使用方向的尺寸,比如手机就是1080\*1920之类,而平板就可能是1920\*1080,而fgo始终是横屏(landscape)方式显示,这导致了之前版本的初始化有可能将长宽颠倒  
## 2020/01/18 v2.10.4  
优化:`setSkillInfo`更名为`setInfo`,以便添加更多快速换装信息  
优化:重写一些代码,现在能够适应任意(非16:9)分辨率及显示画面  
另:重构了一堆代码,极大地并且过分地压缩了代码的纵向长度,将已经基本定型的代码挤到了一行里,可读性大幅下降.用更精简的代码实现更强大的功能  
lambda函数是好文明!  
## 2020/01/16 v2.10.3  
修改了一些写代码时的失误,简化了一些代码,删去了一些很久都没有再次用上的代码段  
说明:能写在一行里的绝不写两行  
更改了代码开头的字符画  
## 2020/01/14 v2.10.2  
bug修复&优化:考虑了从者行动不能的情况,不会试图使用行动不能的从者的宝具,并更合理地选择指令卡  
说明:魅惑导致的行动不能的图标好像是不一样的,等实战遇到了再处理  
bug修复:增加了部分延时  
另:把所有模板的位深度都改为了24,删除了以后不会再用的图片  
另:明确了战斗函数的管辖范围  
## 2020/01/14 v2.10.1  
新:向代码中增加播放声音的功能,现在一旦脚本停止运行就会播放战歌  
说明:为什么不用pygame或者playsound呢?pygame音质奇差,playsound已经不更新了  
无限池最高效率本开启前几个小时发布此更新,就是为了牺牲睡眠质量保证24小时不断肝  
## 2020/01/13 v2.10.0  
bug修复:代码重构带来了一些后续的麻烦...但降低一点内聚性总是好的  
优化:现在这个脚本可以用于任意分辨率的16:9的模拟器显示画面了  
## 2020/01/13 v2.9.0  
代码重构,无实质性变化  
把所有(依赖于adb的)底层交互接口放到了一个新文件里,如果要换平台应用脚本,只要更改新文件里面的内容就行了  
看了一波下来突然发现我的脚本封装的是真滴好,只有三个函数和少数变量是跟fgo运行所在平台相关的,他们是:  
`tap`,`swipe`,`screenShot`(已弃用)  
并且对于当前版本的脚本,你几乎用不到`chooseFrined`函数,截图识别也跟adb无关,也就是说,你甚至可以不写`swipe`和`screenShot`函数,因为在所有其他地方都没有使用这两个函数,就是不停地点点点  
我要不要再把所有依赖Windows的函数也搞个文件放着呢?应该没有人吃了空用Linux打fgo吧...<del>mac?那是什么我不知道</del>
## 2020/01/12 v2.8.8  
bug修复:现在在战斗结束时如果提示加好友会更稳定地拒绝  
说明:此前版本中由于点击时机不精确有可能导致卡在加好友界面  
## 2020/01/12 v2.8.7  
重大bug修复:现在每截一次图就会释放在调用win32api时分配的内存  
说明:在此前的版本中进行大约9场battle就会占用大约8G内存进而导致截图中的某一步分配内存失败,  因此所有使用v2.8.x版本的用户都应该立刻安装此更新  
果然,珍爱生命,远离win32api  
## 2020/01/11 v2.8.6
优化:现在在好友选择界面发现没有好友时(多半是由于使用了过于严苛的筛选条件导致的),会刷新一次好友列表,再发现列表为空才会GG  
优化:`chooseFriend`函数现在不会无止境地找好友,最多识别`Fuse.__max`(默认300)个页面
## 2020/01/09 v2.8.5  
延时调整  
## 2020/01/09 v2.8.4  
bug修复:现在不会试图使用被封印的宝具  
对于这个bug的修复可能有bug  
## 2020/01/09 v2.8.3  
期末考结束了...  
稳定性大优化  
全面修订readme  
## 2020/01/08 v2.8.2  
截图从<某个已经消失的版本>的qt改回win32api了...  
修改了一些判定的模板图片  
由于截图效率的提高,正在尝试用多帧来进行一次判定来提高可靠性,比如houguinfo  
## 2020/01/08 v2.8.0  
稳定性优化  
肝!
## 2020/01/07 v2.8.0beta  
紧急更新  
本次更新内容可靠性未经充分验证,请谨慎下载使用  
使用了win32api代替之前的adb进行截图,单次截图时间从1s级别减低到了10ms级别  
这段代码是不带裁剪和缩放的,所以**需要模拟器在正好1920\*1080的显示器上全屏显示,真机的话要用投屏软件**  
由于之前的代码有一些地方是依赖截图的耗时来进行延迟的,这一延迟消失后可能引发各种各样的问题,所以我正在一点一点地在必要的地方加上显式延迟,但是仍然会有疏漏,之后发现一个解决一个,慢慢改  
## 2020/01/03 v2.7.0  
打版本日志的时候突然发现已经2020年了...期末考好累...  
圣诞活动7号晚上开始,但是期末考9号才结束...  
所以复习放一边去,先把脚本给写了  
重大bug修复,带指向的技能现在会正确地施放了(尽管识别错误的问题仍然存在)  
微调了部分按键坐标,**现在你可以吃银苹果和铜苹果了**  
小优化,切换目标后加了冗余点击以关闭在点击已选中目标时产生的敌人详情对话框  
增加了所谓"快速换装(setSkillInfo)"函数,**先把配置写好,然后活动一开就上号挂机岂不美哉**!  
flag:我圣诞要吃光苹果,当前金苹果当量287  
## 2019/11/26 v2.6.0
蓝叠模拟器更到最新版就不会闪退了  
chooseFriend函数还是挺重要的,要用来选取特定从者  
明天(2019年11月27日星期三)上午8:30通关主线第8话(前篇)后开启炎舞击退战,
增加了一小段代码用于otk,现在直接运行脚本就是单次执行该脚本  
这段代码专用于"三美少女队",如果你没有bba/cba中的任何一个,或嫖不到cba,告辞.  
需要极地迦勒底制服  
**本次活动特攻是"特殊的魔放",会稀释其他的倍率,可恶!**  
## 2019/11/10 v2.5.2
版本更新后蓝叠模拟器闪退,在物理机上的兼容性未发现显著问题.  
版本更新后可以对助战礼装进行筛选,chooseFriend函数变得不再重要,已在主程序中禁用.  
