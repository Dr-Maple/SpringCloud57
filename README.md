# 小程序源码开发工具包
注意本库只能作为学习用途, 造成的任何问题与本库开发者无关, 如侵犯到你的权益，请联系删除。

注意本库只能作为学习用途, 造成的任何问题与本库开发者无关, 如侵犯到你的权益，请联系删除。

注意本库只能作为学习用途, 造成的任何问题与本库开发者无关, 如侵犯到你的权益，请联系删除。

目录

1. 支持版本列表

2. 如何查看当前运行版本?

windows
mac
3. 食用方法

开启小程序F12

开启微信内置浏览器F12

4. 常见问题

支持版本列表

感谢志远大佬的WeChatOpenDevTool开源 代码只是把node改用python3重写，简单实现了一些自动化问题，重要代码都是原作者的。
Windows 微信版本	小程序版本	是否为最新版
11275_x64	✅
11253_x64	✅
11205_x64	✅
11159_x64	✅
3.9.10.19_x64	9129_x64	✅
3.9.10.19_x64	9115_x64	✅
3.9.10.19_x64	8555_x64	❌
3.9.10.19_x64	9105_x64	❌
3.9.9.43_x64	8555_x64	❌
3.9.9.43_x64	9079_x64	❌
3.9.8.25_x64	8531_x64	❌
3.9.8.25_x64	8529_x64	❌
3.9.8.25_x64	8519_x64	❌
3.9.8.25_x64	8501_x64	❌
3.9.8.25_x64	8461_x64	❌
3.9.8.25_x64	8447_x64	❌
Mac x64微信版本	是否为最新版	x
MacWechat/3.8.8(0x13080811)	✅	源码运行
MacWechat/3.8.8(0x13080812)	✅	源码运行
如何查看当前运行版本？

windows

image

image image

mac

ps aux | grep 'WeChatAppEx' |  grep -v 'grep' | grep  "wmpf-mojo-handle" 
食用方法

开启小程序F12

只支持windows版本微信，运行前先启动微信运行前先启动微信（建议小号,别被封了。。。)
安装python3版本
下载WeChatOpenDevTools-Python或直接下载编译好的exe WeChatOpenDevTools_64.exe
安装依赖

pip3  install -r requirements.txt
运行✅

python main.py -x
image image

开启微信内置浏览器F12

python  main.py -c
1709657739316

1709657739316

image

常见问题

无法修改中文

yes
提示找不到版本或微信未运行❌

请先看支持的微信版本和小程序版本
如果还有问题看：微信版本和小程序版本都是符合要求的，但是仍然显示“未找到匹配版本的微信进程或微信未运行”
如果微信版本相同小程序版本不同，就删除小程序版本目录并重启微信，直到刷出支持的小程序版本目录
最后回到上级目录，设置文件夹权限为只读，这样就能一直保持小程序版本一致 image
怎么回退版本？

https://weixin.qq.com/cgi-bin/readtemplate?lang=zh_CN&t=weixin_faq_list&head=true
https://github.com/tom-snow/wechat-windows-versions/releases
mac版本闪退

macOS版本不能和windows版本一样随时hook小程序修改F12，只能先加载小程序后再hook（必须是有小程序缓存了，不然会闪退）
可以先启动多个需要调试的小程序后再运行软件然后再刷新小程序
mac版本提示 Error: Unable to access process with pid xxx from the current user account

Star History
