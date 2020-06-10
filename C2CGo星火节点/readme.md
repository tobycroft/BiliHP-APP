# BiliHP-C2C星火節點



router/mips版本为路由器专用



------------使用方法-------------



打開即可，接下來的操作均在手機和web中完成





第一次打开可能会闪退，是正常的情况



第一次打开可能会闪退，是正常的情况



第一次打开可能会闪退，是正常的情况





因为要生成conf文件



再次打开就行了，然后初始化后，在界面上你会看到jdid和密码



记住这个密码！如果闪屏太快，你可以到conf.ini文件里面找到



然后



到app的c2c里面绑定你的服务器，你就能操作服务器了

------------使用方法-------------





树莓派，香橙派等设备使用：c2c_arm_linux

ubuntu/centos等使用：c2c_linux

AC86，AC3200这些拨通路由器，使用：c2c_mips_linux

MTK的路由器或者开发板，使用：c2c_router_linux

windows：c2c_win32/c2c_win64自行选择





更新方法，更新很简单



不是windows的设备，例如linux

1.首先停下当前版本

2.执行：



你的版本是c2c_linux，就执行c2c_linux，如果是其他版本，只要把c2c_linux替换成c2c_router_linux就可以更新了



curl -O https://pandorabox.tuuz.cc:444/app/c2c_linux



如果无法下载也可以用(一般路由器只有wget)



wget https://pandorabox.tuuz.cc:444/app/c2c_linux





windows版本



https://pandorabox.tuuz.cc:444/app/c2c_win64



上面的直接下载覆盖就好了





版本站永远都只会保留最新的一个版本



或者可以做一个自动升级脚本如下，这个脚本只能在screen下运行



--------------复制如下内容------------------

#!/bin/sh

while :;do

	killall c2c_linux

	echo [`date "+%Y-%m-%d %H:%M:%S"`] Downloading...

	curl -O https://pandorabox.tuuz.cc:444/app/c2c_linux

	chmod +x /root/c2c_linux

	/root/c2c_linux

done

--------------复制如上内容------------------





如果是openwrt系统，请根据你的CPU类型选择，一般MTK的那种（100多200多的都是MTK的二手除外）

选择router版本



如果是400多的，选择MIPS或者ARM版本，自己测试，理论上所有的路由器都是支持的



安装的时候记得安装（不安装其实也能跑，但是不能写守护脚本，掉了没办法自动重启）

curl和ca-bundle还有screen，尤其是screen，这个可以在路由器的软件安装列表里面安装，如果你没有安装潘多拉那些的系统，那可能没办法下载这些插件



路由器的话



--------------复制如下内容------------------

    #!/bin/sh
    
    while :;do
        killall c2c_router_linux
        echo [`date "+%Y-%m-%d %H:%M:%S"`] Downloading...
        curl -O https://pandorabox.tuuz.cc:444/app/c2c_router_linux
        chmod +x /root/c2c_router_linux
        /root/c2c_router_linux
    done

--------------复制如上内容------------------



用这个就可以了

