# Raspberry-Pi-CPU-GPU-Temperature-Check
通过py向yeelink上传CPU、GPU温度，用于检测树莓派状态.

**yeelink** 是一个物联网服务网站，可以将传感器的数据上传到yeelink上，将数据更好的展示出来.

主要步骤：

> * 注册eeLink账户 并拥有一部 树莓派 开发板.
> * 在主页中，通过按照开发指南添加设备、添加传感器.
> * 获取*API Key*以及传感器URL.
- 添加的传感器URL，共有两个，分别是树莓派CPU、GPU传感器URL.


使用yeelink API开始上传数:

我是用的是 Raspberry Lite的版本..所以...需要 requests （通过pip安装）

> sudo apt install python-pip && pip install requests

我将收集来的脚本已经上传github中，所以用git下载即可.

> git clone XX

修改 yeelink api Key 、 apiurl_gpu 、 apiurl_cpu 成自己对应的即可.

定时任务设置

> crontab -e     //新建一个定时任务

> */5 * * * * python ~/yeelink.py    //路径用自己的即可


这是我搭建好的...
（不一定常开）[http://www.yeelink.net/devices/352548]

-------
企鹅群：
树莓派社区 250568697
