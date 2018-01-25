# 尼古拉斯-凯奇和特朗普的换脸人生
[!img](/img/102668242.jpg)

[!img](/img/115597135.jpg)

通过 RussellCloud ,只需一条指令,就能用神经网络实现照片中两人的换脸.

[!img](/img/115597132.jpg)

    russell run --data f3fadfadf6ac417e9f20813603187344:data "python run.py"


# 以下是详细的配置要求

## 在RussellCloud平台上实现快速复现
在[RussellCloud](http://russellcloud.com)上新建名为`faceswap`的项目，选择默认容器环境`tensorflow-1.4`

```
git clone git@github.com:RussellCloud/deepfakes_faceswap.git
cd deepfakes_faceswap
russell init --name faceswap
russell run --data f3fadfadf6ac417e9f20813603187344:data "python run.py"
```	

约一分钟左右,就可以在该项目的网页端检查输出. 
---
# deepfakes_faceswap
This is the code from [deepfakes' faceswap project](https://www.reddit.com/user/deepfakes/).
Hope we can improve it together, HAVE FUN!

Message from deepfakes:

**Whole project with training images and trained model (~300MB):**  
anonfile.com/p7w3m0d5be/face-swap.zip or [click here to download](anonfile.com/p7w3m0d5be/face-swap.zip)

**Source code only:**  
anonfile.com/f6wbmfd2b2/face-swap-code.zip or [click here to download](anonfile.com/f6wbmfd2b2/face-swap-code.zip)

**Requirements:**

    Python 3
    Opencv 3
    Tensorflow 1.3+(?)
    Keras 2

you also need a modern GPU with CUDA support for best performance

**How to run:**

    russell run --data f3fadfadf6ac417e9f20813603187344:data "python run.py"


As you can see, the code is embarrassingly simple. I don't think it's worth the trouble to keep it secret from everyone.
I believe the community are smart enough to finish the rest of the owl.

If there is any question, welcome to discuss here.

**Some tips:**

Reuse existing models will train much faster than start from nothing.  
If there are not enough training data, start with someone looks similar, then switch the data.
