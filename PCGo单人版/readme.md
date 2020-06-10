# readme说明
Centos，Ubuntu等Linux系统	：BiliHP_PC_linux

苹果Mac电脑					：BiliHP_Mac_darwin

Openwrt路由器				：BiliHP_Router_linux

Windows32位					：BiliHP_PCWEB_386

Windows64位（一般用这个）	：BiliHP_PCWEB



#

Windows版本和linux等新版本均不会弹出浏览器（因为新增路由器版本），请手动访问

http://127.0.0.1

或者

http://localhost



如果部署在路由器，请访问：

http://127.0.0.1:79


后台运行功能，仅限登陆后使用





# 逼理逼理助手开源地址
GitHUB:github.com/tobycroft/BiliHP-APP
# PC开源地址：
GitHUB:github.com/tobycroft/BiliHP-Local



# 功能列表：
1.自动签到（静态模拟）

2.自动领取银瓜子（2020全模拟）

3.自动应援团签到（2020全模拟）

4.移动端心跳（2019静态模拟）

5.PC端心跳（2020全模拟）

6.自动完成双端等任务（2019静态模拟）

7.自动送礼物（涉及用户隐私，拿掉）

8.自动每日奖励（静态模拟）

9.银瓜子换硬币（静态模拟）


# 自动抽奖：
1.TV/大楼/心动等抽奖（2019V4部分模拟）

2.舰队领奖（2020全模拟）

3.PK/大乐斗领奖（2020全模拟）

4.节奏风暴领奖（2020全模拟）

5.实物/天选抽奖（2020全模拟）

# 模拟类型说明:
全模拟：强模拟方式，从每条的Header-orign-refer到POST-GET值，均和官方接口一致

部分模拟：次级模拟方式，本方式能模拟80%左右的内容，部分内容因为太麻烦所以没有完全模拟

静态模拟：POST内容相同，但Header内容较为一致（本模拟方案和Github上其他项目的模拟方案一样）



### 更新方法，更新很简单


不是windows的设备，例如linux



1.首先停下当前版本

2.执行：



你的版本是c2c_linux，就执行c2c_linux，如果是其他版本，只要把c2c_linux替换成c2c_router_linux就可以更新了

killall BiliHP_PC_linux

curl -O https://pandorabox.tuuz.cc:444/app/BiliHP_PC_linux




如果无法下载也可以用(一般路由器只有wget)

killall BiliHP_PC_linux

rm -rf BiliHP_PC_linux

wget https://pandorabox.tuuz.cc:444/app/BiliHP_PC_linux





