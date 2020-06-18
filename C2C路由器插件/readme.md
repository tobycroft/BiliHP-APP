# 路由器插件
**luci-app-bilihp适用于openwrt和部分pandorabox**，安装方法如下：
### 方法一
1. 使用ssh登录路由器
2. 下载luci-app-bilihp插件
``` shell
wget -O /tmp/luci-app-bilihp_1.1-2_all.ipk https://raw.githubusercontent.com/tobycroft/BiliHP-APP/master/C2C%E8%B7%AF%E7%94%B1%E5%99%A8%E6%8F%92%E4%BB%B6/luci-app-bilihp_1.1-2_all.ipk
```
3. 安装luci-app-bilihp
``` shell
opkg install /tmp/luci-app-bilihp_1.1-2_all.ipk
```
4. 登录路由器设置页面，在“服务-BiliHP c2c”中进行配置，然后点击"保存&应用"
![image](https://note.youdao.com/yws/public/resource/d59f2d417bea18809b0a4dcfe88ad491/FC337F1C7F48495FB8859B582B97B4CA?ynotemdtimestamp=1591797687564)
### 方法二
1. 下载luci-app-bilihp插件到本地
2. 登录路由器设置页面
3. 进入“系统-文件传输”页面，点击“选择文件”选择luci-app-bilihp插件，然后点击“上传”
![image](https://note.youdao.com/yws/public/resource/d59f2d417bea18809b0a4dcfe88ad491/E1E8DD693188476BA58F68D041BBE84D?ynotemdtimestamp=1591797687564)
4. 在“上传文件列表”内找到luci-app-bilihp插件，点击“安装”
5. 在“服务-BiliHP c2c”中进行配置，然后点击"保存&应用"

### 方法三

1. 登录路由器设置页面
2. 进入“系统-软件包”页面，在“下载并安装软件包”内填入链接`http://raw.githubusercontent.com/tobycroft/BiliHP-APP/master/C2C%E8%B7%AF%E7%94%B1%E5%99%A8%E6%8F%92%E4%BB%B6/luci-app-bilihp_1.1-2_all.ipk`(注意是http，不是https)，点击`确认`。
![image](https://note.youdao.com/yws/public/resource/d59f2d417bea18809b0a4dcfe88ad491/DEBF5D371BAA4106AA145004392D1352?ynotemdtimestamp=1591797687564)
![image](https://note.youdao.com/yws/public/resource/d59f2d417bea18809b0a4dcfe88ad491/7B79089E1E4E4E63A974ED800246C416?ynotemdtimestamp=1591797687564)
3. 安装成功后，在“服务-BiliHP c2c”中进行配置，然后点击"保存&应用"


