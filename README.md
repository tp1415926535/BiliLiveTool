# B站直播工具 [BiliLiveTool]


该程序跨 .Net、 Python、 Html 、JavaScript 开发，考虑到环境问题，使用了独立打包发布，所以体积会显得略大。

支持在主界面、悬浮窗口、网页、其他设备浏览器、OBS、全局飘屏中显示弹幕消息，其中悬浮窗口和网页可以切换 **“常规样式”** 和 **“聊天样式”**   
可设置连接房间，显示消息类型，保存消息类型，收益统计类型，欢迎词，打卡功能，用户备注等。

### 下载（v1.1.2.1）
* [蓝奏云](https://wwvr.lanzn.com/iFxdE2d7fjsf)

### 如何使用
1. 解压后启动`B站直播工具.exe`
2. 切换到左侧标签“功能设置”
3. 在最上方的三种获取cookie方式任选一种（目前浏览器解析限制较多，推荐App扫码登录）
4. 填写目标直播间号（房间号）
5. 点击`连接`

### 演示
多端显示弹幕    
![演示](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E7%A4%BA%E4%BE%8B.jpg)    
全局飘屏效果    
![飘屏](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E9%A3%98%E5%B1%8F.jpg)    

### 说明
![首页](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E9%A6%96%E9%A1%B5.jpg)   
     
![设置1](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E8%AE%BE%E7%BD%AE1.jpg)     
![设置2](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E8%AE%BE%E7%BD%AE2.jpg)

### 版本
* 2024/10/23 v1.1.2.1 增加扫码登录功能；语音播报增加弹幕消息支持；网页的气泡样式显示礼物消息，支持url带`#bubble`直接启用气泡样式
* 2024/9/21 v1.1.2.0 修复进程互斥锁没有正常退出重复程序；chrome更新安全措施，新版浏览器缓存暂时无法读取，增加粘贴Cookie方式导入；支持管理员权限下设置防火墙入站规则
* 2024/7/21 v1.1.1.1 增加语音合成增加微软语音接口模式
* 2024/7/20 v1.1.1.0 增加语音播报功能
* 2024/7/18 v1.1.0.1 修复部分表情过小的问题，修复网页大航海信息显示问题
* 2024/7/14 v1.1.0.0 增加表情图片显示功能，所有显示弹幕的地方可以看见表情包而不是文本了。另外网页列表样式只显示关注直播间，不再显示进入直播间。
* 2024/7/13 v1.0.2.1 飘屏弹幕增加大航海和醒目留言消息，修复移除不当导致慢速或暂停的飘屏弹幕提前消失。
* 2024/7/12 v1.0.2.0 增加全局飘屏弹幕功能
* 2024/6/24 v1.0.1.1 主程序和悬浮窗支持切换新版粉丝牌样式
* 2024/6/15 v1.0.1.0 支持在程序主界面直接发送弹幕。支持给用户添加备注，直接弹幕右键或者在设置新增。备注的用户弹幕在程序主页面和悬浮窗后面显示绿色备注名。可以选择自动回复是否使用备注名
* 2024/6/13 v1.0.0.2 发送弹幕自动缩减过长的用户名，失败仍然显示发送内容
* 2024/6/2 v1.0.0.1 发送弹幕频率强制控制最多一秒一条
* 2024/6/1 v1.0.0.0 基本功能
