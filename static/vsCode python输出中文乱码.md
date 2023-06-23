vcode打开python程序中文乱码

需要找到文件-》偏好-设置=》扩展，找到 run code configration=》execute map

配置setting.json

"python -u",

改成

 "python": "set PYTHONIOENCODING=UTF8 && python -u",

重启vsCode即可



用code runner 执行输出的时候中文乱码。

找到电脑=》设置=》时间和语言=》管理语言设置=》更改系统区域设置=》选择beta版本，使用utf-8提供全球语言支持，改完重启电脑就可以了