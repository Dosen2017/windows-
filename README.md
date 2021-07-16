## windows端口查看，进程操作

#### 查看系统当前所有的端口使用情况
  netstat -ano
  
#### 查看某一特定端口，可以查看到进程ID号
  netstat -ano |findstr "端口号"
  
#### 通过进程ID号查找对应的进程名称
  tasklist |findstr "进程id号"
  
#### 通过进程ID号或者进程名称杀掉进程
  taskkill /f /t /im "进程id或者进程名称"
