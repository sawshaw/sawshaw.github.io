下载安装nodeJS: [https://nodejs.org](https://nodejs.org)会自动安装python

官网下载安装python: [https://www.python.org](https://www.python.org/)

安装完成验证：python -V

打印当前时间：

```python
print (time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()))  
```

文件读取：
```python
#str = input("请输入：")
# print(str)
import sys
import io
#file=open("D:\data\\ticket\\ResultFile\\CCIP_TEL_2023-03-23.txt","r",encoding='utf-8')
file=open("D:\data\\ticket\\ResultFile\\aa.txt","r",encoding='utf-8')
print(file.readlines())

```
多线程：
```python
#!/usr/bin/python
# -*- coding: UTF-8 -*-

import _thread
import time


# 为线程定义一个函数
def print_time(threadName, delay):
    count = 0
    while count < 5:
        time.sleep(delay)
        count += 1
        print("%s: %s" % (threadName, time.ctime(time.time())))


# 创建两个线程
try:
    _thread.start_new_thread(print_time, ("Thread-1", 2,))
    _thread.start_new_thread(print_time, ("Thread-2", 4,))
except:
    print
    "Error: unable to start thread"

while 1:
    pass
```

