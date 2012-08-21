12306.CN 订票助手
===================

这是一个用于辅助在[12306.CN]上订票的Chrome&amp;Firefox脚本。



功能
---------------------

这是一个可以运行在[Chrome]或[Firefox]浏览器上的脚本扩展，可以帮助您在 [12306.CN](https://dynamic.12306.cn/otsweb/) 购买火车票（或抢火车票？），反正就是偷懒呗。
    

**目前已经实现的功能包括**：

*	记录登录的用户名和密码，在打开登录页面后自动填写；
*	自动登录，遇到人过多或繁忙的时候自动重试，直到登录成功（有点儿抢线的味道）；
*	自动记录查询信息，一次查询线路后下次再查询自动填入；
*	自动刷新查询，当没有需要的车次时，自动重新刷新；
*	在[Chrome]下，查票和登录有右下角提示和声音提示；[Firefox]下暂不支持声音提示，但有桌面弹窗提示。
*	自动提交订单，直到订单成功
*	查询失败时自动刷新
*	预定失败时自动重新预定
*	禁用查询缓存
*	查询界面参数和设置自动保存
*	支持过滤无法预定车次
*	支持过滤无需要席别车次
*	现在系统已禁止验证码自动跳过，所以当出现验证码错误时，系统将会自动刷新验证码并自动定位到验证码输入框中并请求输入验证码，输入满四位的时候系统将会自动重新提交。


安装需求
---------------------

目前支持[Chrome]（含RC、Beta以及每夜版），[Firefox]（需要Scriptish扩展支持，使用了新的API所以GreaseMonkey不支持）。

####在Chrome上安装
[Chrome]下可以直接安装。直接打开 [助手主页](http://www.fishlee.net/soft/44/)，在**下载**一节中点击**通用版本**后（如果您实在木有找到，也可以直接[点击这里安装](http://www.fishlee.net/Service/Download.ashx/44/47/12306_ticket_helper.user.js)），Chrome将会在浏览器下方的下载区域通知进行安装：

![Chrome安装提示1](https://github.com/iccfish/12306_ticket_helper/raw/master/images/installation/chrome_1.png)

点击『继续』后，在弹出的对话框中继续点击『安装』。安装完成后即可。

![Chrome安装提示2](https://github.com/iccfish/12306_ticket_helper/raw/master/images/installation/chrome_2.png)


如果您未能看到安装提示，而是提示了下载或其它内容，请确认您的浏览器版本较新。

####在Firefox上安装
在[Firefox]上运行需要**Scriptish**扩展提供支持。**请注意，由于使用了Scriptish提供的新语法，因此_GreaseMonkey_扩展是不支持的**。

* 如果您尚未给[Firefox]安装Scriptish扩展，请[在此安装](https://addons.mozilla.org/zh-CN/firefox/addon/scriptish/)；
* 打开 [助手主页](http://www.fishlee.net/soft/44/)，在**下载**一节中点击**通用版本**后（如果您实在木有找到，也可以直接[点击这里安装](http://www.fishlee.net/Service/Download.ashx/44/47/12306_ticket_helper.user.js)）
* 正常情况下，Scriptish会弹出下列的安装提示，请点击『安装』继续；如果没有这样的提示框而是看到了下载或一堆『乱码』，那么请检查是否成功安装了Scriptish扩展。


提醒
---------------------

由于各大网银都不支持Firefox/Chrome支付，因此请务必在订票前做好支付的准备措施。
这里推荐使用银联在线支付，请开通银联后绑定快捷支付，这样在Firefox和Chrome下都可以顺利付款。
也可以使用招行的手机银行进行支付。


更新历史
----------------------
**版本: 1.0，更新时间： 2012-1-9**

**版本: 1.1，更新时间： 2012-1-9**

* 增加订单自动提交功能

**版本: 1.1.1，更新时间： 2012-1-9**

* 增加取消自动提交订单的功能

**版本: 1.1.2.1，更新时间： 2012-1-9**

* 更改登录判断逻辑，避免提示登录成功却又跳回登录页面的问题； 
* 其它细微更改

**版本: 1.1.3，更新时间： 2012-1-10**

* 增加改签页面的自动刷新支持

**版本: 1.3，更新时间： 2012-1-10**

* 新增查询失败时自动刷新的功能 
* 新增预定失败时自动重新预定的功能 
* 新增禁用查询缓存的功能 
* 其它细节更改

**版本: 1.3.2，更新时间： 2012-1-11**

* 修复了一些BUG 
* 增加了自动提交订单时的休息时间的设置

**版本: 1.4，更新时间： 2012-1-16**

* 将Chrome和Firefox两个版本分支完全合并，兼容处理 
* Firefox下支持声音提示 
* 修改了提示声音 
* 提示窗口均设置默认值自动关闭 
* 修正点击查询后参数保存的问题 
* 修改了参数保存位置，不再保存在Cookies中 
* 加入改签页面的自动提交 
* 增加脚本更新提示功能

**版本: 2.0.0.0，更新时间： 2012-1-19**

* 登录界面重新调整 
* 增加查询界面参数和设置保存功能 
* 增加过滤无法预定车次功能 
* 增加过滤无需要席别车次功能 
* 修复数个BUG 
* 现在系统已禁止验证码自动跳过，所以当出现验证码错误时，系统将会自动刷新验证码并自动定位到验证码输入框中并请求输入验证码，输入满四位的时候系统将会自动重新提交。 

**版本: 2.2.0，更新时间：2012.05.30**
* 根据最新版12306网站修正登录脚本
* 其它细节更新

**版本3.0.0，更新日期：2012.08.20**
* 增加新开专门订票网页窗口的提示；
* 席别过滤的勾选可以记录到设置中；
* 修改列表标题文字，避免换行；
* 增加过滤车次功能；
* 增加出现指定车次时，自动进入预定的功能；
* 增加自定义提示音乐地址功能；
* 增加进入预定页面后，自动播放提示音乐功能（针对自动预定）
* 增加自定义提示音乐地址功能
* 修复进入订票页面时，没有点击自动提交时输入验证码也会提交的BUG

**版本3.0.1，更新日期：2012.08.21**
* 修复勾选“仅座票”、“仅卧铺”过滤无效的BUG

官方网站
---------------------

* [官方发布主页](http://www.fishlee.net/soft/44/)
* [作者的腾讯微博](http://t.qq.com/ccfish)
* [项目主页@GitHub](https://github.com/iccfish/12306_ticket_helper)

相关资料
---------------------

* 感谢所有开发过相关脚本，以及作出贡献的前人们。



[软件主页]: http://www.fishlee.net/soft/44/
[腾讯微博]: http://t.qq.com/ccfish/
[木鱼]: http://www.fishlee.net/ "木鱼的软件主页"
[12306.CN]: http://dynamic.12306.cn/otsweb/ "12306.CN 购票网站"
[Chrome]: https://www.google.com/chrome/ "Google Chrome"
[Firefox]: http://www.mozilla.org/en-US/firefox/all.html "Firefox"