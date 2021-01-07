# 分享一些资源

1. 直接打开raw复制即可
2. 编辑此文件，推荐下载[sublime text](https://www.sublimetext.com/3)

# 安装xray

1.若曾经安装过v2ray-core，先在终端brew uninstall v2ray-core,然后brew untab v2ray/v2ray，否则直接开始第2步 <br>
2.在终端执行brew tap N4FA/xray，然后 brew install v2ray-core <br>
3.将config.json文件放到小房子下，然后 cat ~/config.json > /usr/local/etc/xray/config.json <br>
4.在终端执行brew services restart xray-core <br>

# 注意点

1.由于socks对UDP支持不好，故如果要设置终端代理，建议使用1081端口, 如export ALL_PROXY=socks5://127.0.0.1:1081, <br> 即配置文件中的xtls协议，而非mkcp协议 <br>
