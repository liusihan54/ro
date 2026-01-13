# **BIUH智元机器人智元灵犀x1上位机软件使用指南**  

*如果看完这篇文章还有疑问请移步智元机器人官网：https://www.zhiyuan-robot.com/DOCS/OS/X1-PDG*
---------------------------
## **1：准备工作**

### **1.1：软件准备**

在自己电脑（windows系统）上下载上位机软件:https://www.zhiyuan-robot.com/file/ueditor/php/upload/file/20250114/x1/REF-CLI%20v1.0.3.exe

### **1.2：硬件准备**

USB-TYPEC线，L28推杆需要用4pinUSB线。
<img src="https://github.com/liusihan54/ro/raw/main/webwxgetmsgimg%20(2).jpg" width="500" alt="推杆线示意图">

## **2：调试**

用USB-TYPECL将执行器连接到自己电脑上面。若连接成功，上位机软件会显示软件号，比如说已连接REF xxxxxxxxxxxx 设备作为ref0.若没有任何东西显示出来，则要检查执行器是否成功上电，上电成功正常会闪烁绿灯。若上电成功但仍然没有反应，则换一根数据线。
<img src="https://github.com/liusihan54/ro/raw/main/webwxgetmsgimg.jpg" width="500" alt="连接成功后显示如下">

连接成功后输入对应的设备号，比如上面显示连接的设备为ref3，则输入ref3并按回车，会有一些执行器的基本参数输出。

若要查看执行器内部参数模式，则输入
```python
ref0.motor.config
