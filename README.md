# CV2-Yolov3
这是我们实验室关于人工智能图像识别的资料包 下面就来介绍一下每一个文件的功能：

我把每一个样品收集程序以及用它收集的对应样品写在一起了，方便查看

1.Lacry-64x3-CNN.model
这个文件夹里有一个tensorflow的程序（格式为.pb），这个程序是我们自己写的一个识别微生物活跃期和休眠期的训练模型，能够跑起来，但是并没有用太多样本训练导致没有太高精度。
我们目前的问题是并不知道如何把这个模型作为参数放入我们网上得到的一个yolo3的图像/视频/摄像头识别的程序里面，因为参数格式的原因（我们这个模型是.pb，我们网上找的程序使用的样本模型是以.weight的格式作为参数传输进来的）

2.792020x.pickle/792020y.pickle
这两个是程序的附属产物 可以忽略

3.videoCategoryAnnotator_v2.py 和 LacryProject.zip
videoCategoryAnnotator_v2.py是实验室教授写的收集活跃期和休眠期图片样品的程序 
LacryProject.zip是用这个程序收集的样品图片 上千张休眠期和几百张活跃期

4.NewAnnotator.py 和 三个YOLO格式样本文件
NewAnnotator.py是实验室教授写的收集yolo格式样品的python程序，收集的内容为一整张图片以及各个微生物在图中的状态（0是活跃1是休眠）和位置坐标
编号为123的三个YOLO格式样本是用这个程序收集的一系列样本

5.以tutorial打头的教程文件
这些是制作人工智能识别程序的教程，附带代码样例 有23456号，分别是 2-将你自己收集的数据载入神经网络 3-为微生物lacry建立图像识别神经网络模型 4-用TensorBoard分析神经网络模型
5-优化神经网络模型 6-如何使用训练好了的模型

6.testYolo.ipynb
这是我们在网上收集的yolo程序案例，可以识别图像中的人和日常物品


