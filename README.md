# B站直播工具 [BiliLiveTool]

*该程序跨 .Net、 Python、 Html 、JavaScript 开发，考虑到环境问题，使用了独立打包发布，所以体积会显得略大。*

### 功能
* 多端弹幕消息
     * 主界面、悬浮窗口、网页、其他设备浏览器、OBS、全局飘屏
     * 可切换样式
* 快速登录
* 显示、保存特定类型消息
* 收益根据类型独立统计
* 语音播报
* 打卡
* 欢迎词
* 关注回复
* 礼物和大航海感谢
* 定时弹幕
* 用户备注
* 工具
     * 直播间表情包尺寸转换
* 明暗主题切换

### 下载（v1.3.1.1）
* [蓝奏云](https://wwvr.lanzn.com/iEzff2ryq3xg)

### 如何使用
1. 解压后启动`B站直播工具.exe`
2. 切换到左侧标签“功能设置”
3. 在最上方的三种获取cookie方式任选一种（目前浏览器解析限制较多，推荐App扫码登录）
4. 填写目标直播间号（房间号）
5. 点击`连接`

### 版本间数据迁移
- `Data`文件夹：签到、统计、备注等数据库（重要）
- `appsettings.json`：程序配置（重要）
- `历史记录`文件夹：如果开启保存消息功能，则有该文件夹（可选）
- `导出`文件夹：如果有导出收益统计，则有该文件夹（可选）

### 演示
多端显示弹幕    
![演示](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E5%A4%9A%E7%AB%AF.png)    
全局飘屏效果    
![飘屏](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E9%A3%98%E5%B1%8F.jpg)    

### 说明
![首页](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E9%A6%96%E9%A1%B5.png)   
     
![连接](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E8%BF%9E%E6%8E%A5.png)     
![功能1](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E5%8A%9F%E8%83%BD1.png)
![功能2](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E5%8A%9F%E8%83%BD2.png)
![备注](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E5%A4%87%E6%B3%A8.png)
![工具](https://github.com/tp1415926535/BiliLiveTool/blob/main/%E6%88%AA%E5%9B%BE/%E5%B7%A5%E5%85%B7.png)


### 版本
* 2025/03/25 v1.3.1.1 修复盲盒感谢无效
* 2025/03/25 v1.3.1.0 礼物所属盲盒也作为礼物回复的累计，其他附属页面增加盲盒备注显示；优化导入历史记录，过多内容可以翻页显示；尝试优化主页面大量数据性能
* 2025/03/22 v1.3.0.0 新增主界面导入txt历史记录显示功能，礼物消息增加盲盒备注；引用api的库从16.3升级到17.1.4版本，二维码登录内部重新实现；增加系统设置页面，额外控制启动和隐藏，现在将在托盘显示应用；设置导航样式调整；修复多次二维码登录参数返回异常，修复复制系统消息异常
* 2025/03/16 v1.2.3.2 启动时自动连接增加等待服务启动机制，避免过早连接直接报错；关闭程序时已有连接中的房间则弹窗提醒（功能可配置关闭）
* 2024/12/24 v1.2.3.1 查询收益流水时间排序改为从早到晚，优化求和，补充未及时更新的说明图片。
* 2024/12/23 v1.2.3.0 主界面增加房间在线实时人数显示；收益增加接口查询直播流水数据窗口
* 2024/11/27 v1.2.2.1 取消主程序的端口监听；更改服务打包形式，支持服务的系统消息回显；主页面的复选框样式改进
* 2024/11/26 v1.2.2.0 优化其他名称过长的回复；新增表情包尺寸转换工具；欢迎词改为完全自定义；修复粉丝牌样式配置未正确初始化
* 2024/11/13 v1.2.1.2 优化礼物回复的逻辑，对所有礼物统计后执行；按面板拆分整理代码
* 2024/11/11 v1.2.1.1 修复微软tts接口;修复切换发音后抛空错误
* 2024/11/10 v1.2.1.0 增加关注回复、礼物和大航海回复、定时弹幕；功能页面重布局；修复小bug，提升初始化速度。
* 2024/11/8 v1.2.0.0 界面样式优化：新增明暗主题切换，弹窗现代化适配，标题调整增加图标占比，弹幕显示舰长图标；设置增加语音播报允许忽略自身或主播弹幕，欢迎词可设置舰长限制，关注直播间可播报语音，增加新的语音播报源；调整飘屏并发出现的拥挤情况；增加功能介绍，增加错误日志；用户数据和导出文件单独放入文件夹中；修复欢迎词限制失效，修复关闭窗体未正常等待导致子进程存留；尽可能排除不必要引用减少打包体积
* 2024/11/3 v1.1.2.2 尝试优化签到写数据库和发送弹幕的并发逻辑
* 2024/10/23 v1.1.2.1 增加扫码登录功能；语音播报增加礼物和弹幕消息支持；网页的气泡样式显示礼物消息，支持url带`#bubble`直接启用气泡样式
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


### 引用
- B站相关：[bilibili-api](https://github.com/Nemo2011/bilibili-api)
