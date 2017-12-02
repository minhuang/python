# python

不知何时起，sublime text 的package control 无法安装插件，安装的时候总是弹框

There are no packages available for installation

网上各种办法，说是添加host，根本无效，通过如下方法最有效

最完美的解决方法在下面：

1.去下载https://packagecontrol.io/channel_v3.json  ，官网地址下载比较慢，可以找个其他地址下载

2.修改配置
Package Control.sublime-settings]修改方法：
Preferences > Package Settings > Package Control > Settings - User
添加

    "channels":
    [
        "https://raw.githubusercontent.com/minhuang/python/master/python_channel_v3.json"
    ],
    
这样就可以了，亲测有效
