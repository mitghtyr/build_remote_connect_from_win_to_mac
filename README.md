# build_remote_connect_from_win_to_mac
本来是为了解决mac catalina版本不能PPTP连接VPN问题，利用旧win实现远程连接

## 应用背景
mac端无法用PPTP协议连接到内网VPN，一些VPN客户端又贵又不稳定，一运行mac风扇跟起飞一样。于是就想利用我的古董win10，毕竟win还支持PPTP的VPN。思路是用mac控制win，但由于**不在同一局域网**，因此需要先获得internet上内网地址，再远程连接。

## 工具准备
* 一台macpro，os：Catalina 10.15.7
* 一台八年前的古董win10
* mac端的Microsoft remote desk beta版本
* win10 端的Cpolar内网穿透工具
* win10 的远程控制

## win端
* pptp的VPN连接
* 开启win的远程控制（win版本不支持的话，自行搜索开启方法
* cpolar的隧道分配（24h更新一次，这个要注意）

## mac端
* Microsoft remote desk 安装
* 远程登录

## 缺点
* mac端耗电还是比较高
* cpolar的免费隧道会不断改变地址，还是挺麻烦的 【**待解决**】
* 古董电脑太dumb了，而且远程分辨率没法调，看起来很累眼睛
* win端vpn断了的话，mac端就完全重连不上了 【**待解决**】

## 优点
* 不用专门付费client了
* 可以结合两个系统的优点，无缝切换
* 不用随身背着沉重的古董win

