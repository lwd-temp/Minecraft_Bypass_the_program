# Minecraft for Windows 10 Bypass the program
绕过Minecraft for Windows 10我的世界UWP验证系统


### 请支持正版！

www.Minecraft.net

一次购买终身享受 请务必支持正版!!!

另一种绕过验证方法请参见 https://github.com/xingchuanzhen/Minecraft-Unlock

### 介绍


傻瓜式一键操作，全自动化执行程序

自动起调MinecraftUWP，自动结束RuntimeBroker.exe

游戏30分钟左右不会出现“解锁完整游戏”

游戏关闭后自动还原注册表，启动服务项

项目开源免费完全公开，火绒、360、管家绝无报毒


### 使用方法:

 1.双击打开软件

 2.单击“启动程序”按钮
 
 3.等待提示“启动完成”即可开始游戏

 注：程序之所以要申请管理员权限，是为了修改部分注册表，在关闭程序后会自动还原修改后的注册表
 
 ### 命令行调用格式
 
         [Implement   |   Reduction]   <Notify_NO>  <Interface_NO>

         命令解释：

         [必须]
         Implement		启动并执行程序
         Reduction		启动程序并执行还原操作

         <可选>
         Notify_NO		隐藏任务栏通知

         <可选>
         Interface_NO    隐藏图形化界面
         
         示例：
         
         Reduction   Interface_NO 

### 软件执行流程(单击“启动程序后”)：

 1.开始释放内嵌入注册表文件到用户临时文件夹

 2.执行导入注册表操作

 3.使用NET命令停止系统ClipSVC 服务

 4.删除释放过程中的注册表文件

 5.通过Process的Start方法调起 MinecraftUWP

 6.后台等待28秒后开始使用Tasklist命令显示Microsoft Store 应用及其关联的进程

 7.开始扫描MinecraftUWP关联的RuntimeBroker进程PID

 8.获取到PID后使用Tasklist命令强制结束进程，此时游戏启动完毕

 9.启动后台每隔10秒自动扫描与Minecraft相关联的RuntimeBroker进程并结束

 10.同时检测Minecraf进程是否退出，绕过退出程序自动关闭，同时还原注册表和服务项


### 注意事项：

 1.游戏运行时不能关闭本程序，关闭游戏后程序会自动退出
  
 2.需要提前下载MinecraftUWP否则会提示没有安装MinecraftUWP
  
 3.启动成功后软件会自动隐藏到托盘，如果结束程序后则将在30分钟内游戏自动失效

 4.本程序仅供学习交流，严禁商用或其他方法用途，严禁非法第三方倒卖，软件永久开源免费

 5.不要在任务栏中，或任务管理器中直接结束本进程，进程检测到退出游戏后10秒内自动退出并还原注册表和服务项，退出完成后会有提示

 6.正常使用情况下不会造成系统故障，如果遇到商店无法下载应用的情况下，或者无法安装UWP应用时，可用尝试打开程序，直接点击“关闭程序”按钮，程序会重新还原系统修改项
  
### 写到最后：

 编译后的程序链接：

 蓝奏云：https://wwe.lanzoui.com/b01ohqixa 密码:1kut

 本程序遵循GPL ( GNU General Public License )开源许可协议，程序仅供学习交流，严禁商用或其他非法用途！
