[winXray 入门小技巧](./sub/introduce.md)   
[winXray 最新视频教程](https://www.youtube.com/results?search_query=winXray&sp=CAI%253D)  
[网络免费 vmess 服务器订阅链接](https://proxypool.ga/vmess/sub)   
[网络免费 Shadowsocks 服务器订阅链接](https://proxypool.ga/ss/sub)     
[网络免费 clash 服务器订阅链接](https://proxypoolss.tk/clash/proxies?speed=100&type=vmess,trojan)   
可复制上面各种格式订阅链接，在 winXray 中点击「批量导入链接」一键体验 winXray 强大的兼容性。

请认准 winXray.exe 原版 v2.3.0 校验值   
-----------------------------------------------  
MD5:	FC4DA1FA5F915FAF107C248600CFEE4B  
SHA1:	93D73CD90C0508972AAB600A88615B7C63CFF39C  
SHA256:	A745FF902E3D3F4F325FB57D9DC37149A1A6694EAC75E33A0B69D7190AC3E3F5  
CRC32:	B427ED49  
各大主流杀毒软件检测安全，自行编译源码可得到完全相同的EXE。  
编译工具如果版本不同可能生成的二进制文件校验值有变，现在各大杀毒软件只要一个字节变化都可能会误报病毒。  
原版 winXray.exe 永久保持完全公益免费，不会插入任何推广链接。  


关于支持 PAC 代理的说明：
-----------------------------------------------  
先说一下很多客户端 PAC 模式卡顿一直没解决，但 winXray 已经解决了这个问题并且丝滑般的流畅。    
PAC的功能本来就非常简单，**winXray 实现 PAC 服务的代码只有几句代码  - 所以我们没有任何理由不支持 PAC**。  
在 winXray 中管理 PAC 名单非常的简洁方便，如果一个代理客户端 PAC 模式卡顿不稳定，编辑 PAC 麻烦困难，或者根本就不支持 PAC，这时候他们会说是因为 PAC 不好，这有多少可信度我就不多说了。请注意**只有 PAC 能真正的直接支持高效安全的 SOCKS5 协议**，否则就只能改为低版本 SOCKS 或者 HTTP 代理。**PAC 与翻墙软件完全无关并完全独立**，可以保证只有你指定的国外网站与翻墙软件发生关系。**PAC 能避免一些敏感的软件、或者没有被墙的大流量下载软件不会在没经过你手动许可时悄悄流向翻墙软件**，例如迅雷、百度网盘、Steam、Telegram。另外启用 PAC 并不会影响大家使用 Xray-Core 自带的路由规则 - 这与 PAC 并没有任何的矛盾和冲突。  
  

# winXray 
本软件源码已贡献到公共领域并放弃版权，源码可使用 [aardio（开发环境仅6.5MB）](http://www.aardio.com) 编译生成单文件绿色EXE( 不需要.Net等任何外部运行库 ），**[点这里下载](./../../raw/master/release/winXray.7z)** （ [64位版本](./../../raw/master/release/winXray.7z) / [32位版本](./../../raw/master/release/winXray32.7z) ），解压即可直接使用( 仅  **[5.0MB](./../../raw/master/release/winXray.7z)** - 已自带 Xray-core）。

winXray[:loud_sound:](http://dict.youdao.com/dictvoice?audio=winxray&type=2) 是一个简洁稳定的 [Xray/V2Ray(vmess/vless/xtls)、Shadowsocks、Trojan](https://github.com/XTLS/Xray-core) 通用客户端（Windows系统），可自动检测并连接访问速度最快的代理服务器。服务器连接异常时可以自动更换代理服务器 - 再也不用担心服务器抽风了。winXray 也提供一键安装 XRay(V2Ray、Shadowsocks、Trojan) 服务器工具。   
  
之前我用过很多代理客户端，经常用一会就挂掉了，有些测试很久才找到下一个可用的服务器，有时怎么切换都不行，一定要把整个软件退出重启才能恢复。而且在WIN10上都有相同的BUG:PAC代理用一段时间就会卡死( winXray已经通过自行实现PAC服务器解决了这个问题 )，其实这些软件里提供的很多功能我并不需要，我只想愉快地用下 google 找点技术资料提升工作效率。但是在网上找了很久都没找到适合的软件，于是决定自己动手写一个，还好用 aardio 写软件的速度很快 - 大概用了几个小时就完成了 winXray 的主要代码，改进了几个版本以后就很稳定了，**我自己用了 winXray  几个月再也没有遇到 google 抽风访问不了的问题**。    

一些网友对 winXray 的测速功能存在误解，简单的测速不但不必要的消耗流量而且没有什么实用价值，例如Ping通了TCP访问不了，TCP通了但浏览器被阻断，或者下载测速需要连接代理服务器以后长时间测试才能得到下载速度 - 如果有很多服务器需要频繁快速地测速这样显然是不行的。**根据我长时间的实测，我使用一堆的服务器，大多时候 winXray 都能最快的找到其中速度最快、且能正常使用的线路**。要考虑到网络速度与服务器响应速度本来就是波动的，**winXray 能在连接代理服务器以前在零点几秒以内快速地在上百个代理服务器中找出最快的服务器** - 可以节省我们大量手动测试切换的时间，如果你有一个比我们幸福的网络环境，有一堆稳定流畅看4K视频的代理服务器 - 那你确实可以关闭自动切换功能 - 手动切换即可。

![winXray](./screenshots/winXray.png)

winXray支持批量导入 vless、vmess、ss、trojan、trojan-go …… 等格式的分享链接，  
也可以导入v2ray,、Shadowsocks、trojan等通用订阅链接，兼容 base 64、json …… 等不同格式的服务器配置，也可以导入 Clash proxy-provider 配置，winXray将自动转化各种不兼容的配置为统一、规范的格式。winXray 有强大的兼容性，我们甚至可以直接自 github 项目地址导入代理服务器，例如直接复制链接 [https://github.com/winXray/winXray/blob/master/sub/sample.json](./sub/sample.json) 即可一键导入 winXray。

![服务器配置](./screenshots/config.json.png)
**小技巧: JSON里点击任意字段都会显示该字段的用法说明。** 个人认为做很多对话框来配置服务器的参数是非常蠢的，winXray已经把各种代理协议的配置简化为几个统一命名的JSON字段（ **也可以作为一种标准的、统一的、通用的订阅响应格式使用** ），只要稍加学习就可以非常熟练的添加、修改各种代理协议的配置。而且对于大多数用户根本不需要改配置 - 简单的复制导入分享链接就可以，我们不必要把简单的事搞复杂。

可选在 ["/xray-core/winXray-default-servers.json"](./xray-core/winXray-default-servers.json) 文件中添加默认服务器配置（生成EXE后默认配置自动嵌入到EXE文件，可选删除该文件,也可以继续使用该文件覆盖EXE自带的默认服务器列表）。

![PAC配置](./screenshots/pac.png)
**小技巧: PAC编辑器里点击任意域名都会自动关联到单选框，可以直接切换代理或直连。**

软件首次运行时会在当前目录查找 "./xray-core/xray.exe"   
发行文件仅需要 "./winXray.exe"，可选带上 "./xray-core/" 目录（ 如果没有找到会自动到v2ray官网下载，不过没有代理服务器下载有时候非常慢 )。

![端口配置](./screenshots/config.advanced.png)

<img src="./screenshots/telegram.gif" width="1031" alt="Telegram 端口配置">
