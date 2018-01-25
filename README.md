# 尼古拉斯-凯奇和特朗普的换脸人生

<p align="center">
<img src="/img/102668242.jpg" height="300">
<img src="/img/115597135.jpg" height="300">
</p>

通过 RussellCloud ,只需一条指令,就能用神经网络实现照片中两人的换脸.

<p align="center">
<img src="/img/115597132.jpg" height="300">
</p>


    russell run --data f3fadfadf6ac417e9f20813603187344:data "python run.py"


# 以下是详细的配置要求

## 在 RussellCloud 平台上实现快速复现
在[RussellCloud](http://russellcloud.com)上新建名为`faceswap`的项目，选择默认容器环境`tensorflow-1.4`

```
git clone git@github.com:RussellCloud/deepfakes_faceswap.git
cd deepfakes_faceswap
russell init --name faceswap
russell run --data f3fadfadf6ac417e9f20813603187344:data "python run.py"
```	

约一分钟左右,就可以在该项目的网页端检查输出. 
---
## 项目背景
本项目起源于 reddit  ,一名网友通过类似思路,把AV的头换成了自己喜爱的某明星 :) 