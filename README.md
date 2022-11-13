# 使用Railway部署Xray高性能代理服务，通过ws传输的 (vmess、vless、trojan shadowsocks、socks)等协议

> 提醒： 滥用可能导致账户被BAN！！！ 

## 概述

用于在 railway 上部署 vless+websocket+tls，每次部署自动选择最新的 alpine linux 和 Xray core 。  
vless 性能更加优秀，占用资源更少。

* 使用[xray](https://github.com/XTLS/Xray-core)+caddy同时部署通过ws传输的vmess vless trojan shadowsocks socks等协议，并默认已配置好伪装网站。
* 支持tor网络，且可通过自定义网络配置文件启动xray和caddy来按需配置各种功能  
* 支持存储自定义文件,目录及账号密码均为UUID,客户端务必使用TLS连接  



### 服务端

fork 之后 ，在railway的dashboard，选择 new project
[![CHIH8A.png](https://www.helloimg.com/images/2021/09/05/CHIH8A.png)](https://www.helloimg.com/image/CHIH8A)
然后在github中选中本仓库
[![5oSpg.png](https://i.w3tt.com/2021/09/05/5oSpg.png)](https://img.tg/image/5oSpg)

### 客户端
* **务必替换所有的`xxx.railway.app`为railway分配的项目域名**  
* **务必替换所有的`b7efbc8a-84d8-4875-a29f-9f707277efe8`为部署时设置的UUID,建议更改,不要每个人都一样**  

**XRay 将在部署时会自动实配安装`最新版本`。**


