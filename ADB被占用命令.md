## ADB端口被占用时解决方式  
netstat -aon|findstr "5037"   查找占用5037端口号的PID  

tasklist|findstr "PID值"  根据PID查找对应的程序  

打开任务管理器找到对应的PID或者进程名称关闭进程即可  
