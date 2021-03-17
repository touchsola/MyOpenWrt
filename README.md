# MyOpenWrt  
<a href="https://t.me/my_openwrt" target="_blank">Telegram</a>  
  
## 1. OpenWrt来源：  
    https://github.com/openwrt/openwrt  
      
## 2. 编译包含以下常用工具  
    GodProxy滤广告：https://github.com/project-lede/luci-app-godproxy  
    AdGuardHome：https://github.com/rufengsuixing/luci-app-adguardhome  
    OpenClash：https://github.com/vernesong/OpenClash/  
    HelloWorld：https://github.com/jerrykuku/luci-app-vssr  
    流量监控：https://github.com/brvphoenix/luci-app-wrtbwmon  
    Zerotier设置界面：https://github.com/rufengsuixing/luci-app-zerotier/  
    vlmcsd设置界面：https://github.com/cokebar/luci-app-vlmcsd/  
    Argon主题：https://github.com/jerrykuku/luci-theme-argon/  
    Argon主题设置：https://github.com/jerrykuku/luci-app-argon/  
    Edge主题：https://github.com/jerrykuku/luci-app-argon-config/    
      
## 3. 编译包含以下OpenWrt Package  
    luci-app-banip：外网环境可以禁止风险IP  
    luci-app-ddns：动态DNS客户端  
    luci-app-uhttpd：uHTTPd Web服务器配置  
    luci-app-upnp：upnp配置模块  
    luci-app-wol：局域网唤醒的支持  
      
## 4. 截图  
![Screenshot_2021-03-14 OpenWrt - 概览 - LuCI(1)](https://user-images.githubusercontent.com/72115940/111072058-e9e67700-8513-11eb-836f-877c1bbdd12c.png)  
  
![Screenshot_2021-03-14 OpenWrt - 概览 - LuCI(2)](https://user-images.githubusercontent.com/72115940/111072056-e9e67700-8513-11eb-911e-507df2d408a2.png)  
  
![Screenshot_2021-03-14 OpenWrt - 基础设置 - LuCI](https://user-images.githubusercontent.com/72115940/111072054-e81cb380-8513-11eb-9d9b-ba737aad6bbb.png)  
  
![Screenshot_2021-03-15 OpenWrt - GodProxy滤广告 - LuCI](https://user-images.githubusercontent.com/72115940/111124122-17caca80-85ab-11eb-8ca5-ae6d3cbd77a4.png)
  
## 5. 关于广告拦截说明
    GodProxy滤广告 和 AdGuardHome 均为广告拦截工具，二选一或者双剑合璧。  
    GodProxy滤广告的过滤更强大，可以过滤YT视频广告  
    而AdGuardHome兼容性更好  
    - 同时开启需要修改 AdGuardHome 管理页面端口为3001或其他，避免占用 GodProxy 的3000端口  
    - 开启 AdGuardHome 并使用 OpenClash ：需要在 OpenClash 全局设置-DNS设置-勾选自定义上游DNS服务器-添加127.0.0.1:[AdGuardHome端口]  
    - 开启 AdGuardHome 并使用 HelloWorld ：需要在 HelloWorld DNS解析方式-使用本机端口为[AdGuardHome端口]的DNS服务  
    - 开启 GodProxy滤广告 并使用 OpenClash ：不要勾选自定义上游DNS服务器
    - 开启 GodProxy滤广告 并使用 HelloWorld ：网络-DHCP/DNS-高级设置-DNS 服务器端口-修改为非53的其他数字，以便PDNSD能正常工作
