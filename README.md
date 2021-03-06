# MyOpenWrt  
<a href="https://t.me/my_openwrt" target="_blank">Telegram</a>  
  
## 1. OpenWrt来源：  
    https://github.com/openwrt/openwrt  
      
## 2. 编译包含以下常用工具  
    GodProxy滤广告：https://github.com/project-lede/luci-app-godproxy  
    AdGuardHome：https://github.com/rufengsuixing/luci-app-adguardhome  
    OpenClash：https://github.com/vernesong/OpenClash  
    Bypass：https://github.com/garypang13/luci-app-bypass  
    PassWall：https://github.com/xiaorouji/openwrt-passwall/  
    Helloworld（需要切换Argon主题后使用）：https://github.com/jerrykuku/luci-app-vssr
    解锁网易云灰色歌曲：https://github.com/maxlicheng/luci-app-unblockmusic  
    京东签到服务：https://github.com/jerrykuku/luci-app-jd-dailybonus  
    流量监控：https://github.com/brvphoenix/luci-app-wrtbwmon  
    Zerotier设置界面：https://github.com/rufengsuixing/luci-app-zerotier  
    vlmcsd设置界面：https://github.com/cokebar/luci-app-vlmcsd  
    定时设置插件：https://github.com/sirpdboy/luci-app-autotimeset
    Argon主题：https://github.com/jerrykuku/luci-theme-argon  
    Argon主题设置：https://github.com/jerrykuku/luci-app-argon  
    Edge主题：https://github.com/jerrykuku/luci-app-argon-config
    网络唤醒Plus：https://github.com/siwind/luci-app-wolplus  
    高级设置+文件管理：https://github.com/sirpdboy/luci-app-advanced  
      
## 3. 编译包含以下OpenWrt Package  
    luci-app-ddns：对动态DNS客户端的设置  
    luci-app-uhttpd：uHTTPd Web服务器配置  
    luci-app-upnp：upnp配置模块  
    luci-app-sqm：智能队列管理配置  
      
## 4. 截图  
![Screenshot_2021-03-14 OpenWrt - 概览 - LuCI(1)](https://user-images.githubusercontent.com/72115940/111072058-e9e67700-8513-11eb-836f-877c1bbdd12c.png)  
  
![Screenshot_2021-04-18 OpenWrt - 概览 - LuCI](https://user-images.githubusercontent.com/72115940/115141803-d8434280-a070-11eb-8a29-01b304b418ef.png)
  
![Screenshot_2021-03-14 OpenWrt - 基础设置 - LuCI](https://user-images.githubusercontent.com/72115940/111072054-e81cb380-8513-11eb-9d9b-ba737aad6bbb.png)  
  
![Screenshot_2021-03-15 OpenWrt - GodProxy滤广告 - LuCI](https://user-images.githubusercontent.com/72115940/111124122-17caca80-85ab-11eb-8ca5-ae6d3cbd77a4.png)
  
![Screenshot_2021-04-18 OpenWrt - 基本设置 - LuCI(1)](https://user-images.githubusercontent.com/72115940/115140589-96170280-a06a-11eb-988d-f6084e08317a.png)
  
## 5. 关于广告拦截说明
    GodProxy滤广告 和 AdGuardHome 均为广告拦截工具，二选一或者双剑合璧。  
    GodProxy滤广告的过滤更强大，可以过滤YT视频广告  
    而AdGuardHome兼容性更好  
    - 同时开启需要修改 AdGuardHome 管理页面端口为3001或其他，避免占用 GodProxy 的3000端口  
    - 开启 AdGuardHome 并使用 OpenClash ：需要在 OpenClash 全局设置-DNS设置-勾选自定义上游DNS服务器-添加127.0.0.1:[AdGuardHome端口]  
    - 开启 GodProxy滤广告 并使用 OpenClash ：不要勾选自定义上游DNS服务器
