

官方网站： www.5mrk.com         Telegram万人群https://t.me/BT_json



<h3><strong>简单介绍</strong></h3>

- 插件功能：弹幕后台、前置广告、暂停广告、会员去广告，记忆回放，自动下一集


- 插件支持：.m3u8、.mp4、.flv、等常见视频格式 注释:不支持MP4 H265格式的视频（如果你发现说支持的那他牛逼了）

- 插件兼容：电脑、手机端


<h3><strong>版权声明</strong></h3>
- 本插件开发者：BTJSON丶黑白丶乐乐丶某毅 唯一官方网站https://www.5mrk.com ，你如果在 什么 根网站、什么 鱼源码等等乱七八糟的网站下载，那么你得到的永远是高危、高风险、自带后门的垃圾程序，而正版永久更新，永久售后！！

- 本文未经允许禁止任何人以任何形式转载，违者必究！

- 本插件为收费插件，使用者必须向本插件开发者一次性支付费用才能使用，本插件售后方式 为QQ群方式，如果发现倒卖或者随意传播，我们将永久封号解除所有相关服务！

- 如您以购买我们的开发版本，请您再次二开的时候请自己写核心代码，不能用我们的，为了您的利益请自己写核心代码丶

- 永久包更新—————————打击盗版

- 正版请关注：BTJSON社区 站长资源网 其他均为假冒~！ 官方唯一客服QQ 58249393

- 我们郑重承诺：一次消费永久包更新，持久享受售后服务




<h3><strong>更新说明：</strong></h3>

2021年04月21号

1.更新远程js为在线实时更新（免去你们总是手动自己更新的麻烦）

 

2021年04月17号

 

全新前端（重构各种功能。抛弃0.3.8以前的所有版本，此版本大概4月底强制更新）目前最新的版本为1.0版本
————————————————————

（此内容是给技术人员预留的，会技术的可以自己继续开发 不会的无视此项）

/library/docking/socket/Currency.php

此文件可以自己随意构造自己想要的播放json输出模式

里面已经给你们放了一个演示例子 自己可以按照例子设置

也可以这样
$this->setPlayer();

$this->setPlayer(‘ckplayer’);

$this->setPlayer(‘dplayer’);

———————————————————–

1. 修改json接口 在此文件夹里面/library/config/config.php

2.

* 解析接口对接模式 – 高级版
* 可用参数说明 – >
* – title 接口名称
* – match 匹配值 (解释【*,自定义】)
* – custom 自定义对接JSON(配合url字段 – 详细看对接文档) true | false
* – url 接口地址 (解析接口,支持自定义对接)
* – spare_url 备用接口地址 (主接口请求失败使用备用接口) 自定义对接不生效(可留空或删除该字段)
* – cache 自定义缓存 [switch缓存开关 true:false | cacheTime缓存时间 整数 (秒)]
* – parameter 自定义回调参数 [url局内地址 : “解析json字段(url)” | source来路定义 : “解析json字段(metareferer)”] 自定义对接不生效
* – referrer 来路设置 [default默认 : “never” | no-referrer匹配模式 | never匹配模式]

3. /library/docking/socket/Currency.php 这个文件我默认对接的是/library/config/config.php里面的奇艺 优酷 自己把json接口放在Currency.php里面即可， 因为Currency.php文件是自定义所有的东西所有目前只给你们写了一个参考例子

4. /library/config/config.php 里面设置json跟0.3.8版本基本上是大同小异，自己看下说明或者自己研究下也可以

5. 修改player.php 文件在 view/player.php 设置好自己的后端域名 和key

重构说明：
1. 重构了一个最严重的bug 弹幕 判断URL 入库 （注释：下次更新直接更新显示播放页片名显示）

2. 重构 弹幕播放器在线人数显示的bug （以前不管是我这边的还是外面泛滥版本一直有这个bug 所有现在完美修复这个问题 （注释：下次更新直接对接统计 来实现显示在线人数））

3. 重构json返回数据响应 优化

4. 重构禁止来路，禁止伪造及跨域 （修复）

5. 重构 多json接口 的优化及使用 （修复）

6. 重构 在使用CDN的情况下缓存出现bug的问题

7. 忘记还有啥了，，，，，，，，，，脑子乱了

 

 

 

 

2021年04月08号

- 1.优化核心代码
- 2.修改远程js代码（实现本地化，因用远程调用各别地区无法访问）
- 3.修复cache文件清理的bug
- 4.增加单独配置json接口 缓存  开关（详细在群共享）
- 5.修复json各别格式的链接 重新定义url
- 6.增加定时广告位
- 7.增加统计位
- 8.增加basuc.php文件 重新定义url


2020年06月10号

- 1.新增功能 可以遮挡外面资源站的跑马灯广告

2020年06月09号

- 1.新增在线解析功能（添加自己的json接口即可） 目前免费赠送一条

- 2.新增可以添加N条 json接口 加固解析稳定性

- 3.修复在线解析记忆播放bug

- 4.修复在线解析各大官方视频判断问题

- 5.新增 在线解析+Mao资源+Acfan解析（支持VIP）整合


2020年06月07号

- 1.修复并优化画中画切换控制台一直报错提示

- 2.修复关闭弹幕会导致颜色代码固定不变

- 3.修复关闭加载动漫浏览器控制台一直报错倒数


2020年06月06号


- 1.美化前端播放页 支持字体大小
- 2.新增画中画
- 3.美化前端播放页图标美化
- 4.美化前端播放页广告 关闭按钮 及标
- 5.美化后端 先择主题颜色 及可视化

2020年06月03号

- 1.修复添加广告代码，播放器被顶开的问题
- 2.修复点击倍速后在点击设置菜单弹出乱码问题
- 3.后台增加 弹幕礼仪文字开关及文字修改
- 4.后台新增 弹幕公用和私用开关
- 5.后台新增 自动播放和点击播放开关
- 6.后台弹幕库 新增reffer来源显示
- 7.后台弹幕库 新增获取B站弹幕ID 显示
- 8.美化前端播放页 支持字体大小
- 9.支持 跳过片头 片尾
- 10.优化更新加载页面动画可自定义 及进度条等主题内容演示切换

- Diy by 黑白 btjson 乐乐 Tim

2020年05月24号

- 1.弹幕Ip reffer入库
- 2.修复主题颜色
- 3.修复后台失效
- 4.修复加载动画失效
- 5.后台添加右键修改
- 6.修复致命Bug
- 7.修改文件 m3u8.php mao.php 以及 DPlayer.de.js

2020年4月23日

- 1.新版本更新版本号1.0.3
- 2.远程js版本号为1.0.7
- 3.增加淘宝口令设置(增加自己额外的收入不显示任何广告)
- 4.增加免费版P2P（去掉对接的 cdnbye的P2P改为免费版P2P）
- 5.其他细节


2020年4月21日

- 修复手机端UC浏览器播放问题


2020年4月13日

- 弹幕库与播放器分离,可分别放独立服务器里


2020年4月12日

- 1.整合播放器后台
- 2.后台适配手机屏幕
- 3.支持弹幕直接安装
- 4.支持弹幕后台管理
- 5.添加播放暂停广告


2020年3月18日

更新如下:

- 1.修复各大浏览器兼容性问题

- 2.修复微信不能播放的问题

- 3.美化播放器

- 4.更新js为远程调用

- 5.修复弹幕屏蔽词功能问题

- 6.修复支持跨域自动下一集播放问题

- 7.修改弹幕库设置问题

- 8.修复IOS微信 不能播放的问题

- 9.加入P2P视频加速功能


技术支持

     乐乐    黑白  Tim  btjson  某毅
