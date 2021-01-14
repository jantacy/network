# 分享一些资源

1. 直接打开raw复制即可
2. 编辑此文件，推荐下载[sublime text](https://www.sublimetext.com/3)
3. 想了解xray相关项目，请戳[xray](https://github.com/XTLS/Xray-core)
4. ClashX相关下载地址，请戳[ClashX](https://github.com/yichengchen/clashX/releases) , 选择最新版即可，下载Assets下的ClashX.dmg


# 安装xray

1.若曾经安装过v2ray-core，先在终端brew uninstall v2ray-core,然后brew untab v2ray/v2ray，否则直接开始第2步 <br>
2.在终端执行brew tap N4FA/xray，然后 brew install xray-core <br>
3.将config.json（先改下UUID成自己的）文件放到小房子下，然后 cat ~/config.json > /usr/local/etc/xray/config.json <br>
4.在终端执行brew services restart xray-core <br>
5.按附件模板更新下ClashX的配置，注意config.json和config.yaml的UUID都需要替换成自己的

# 注意点

1.由于socks对UDP支持不好，故如果要设置终端代理，建议使用1081端口, <br> 如export ALL_PROXY=socks5://127.0.0.1:1081, 即配置文件中的xtls协议，而非mkcp协议 <br>
