#方向梯度直方图Histogram of Oriented Gradients

##一、基本概念
###1、概念
它是一种在计算机视觉和图像处理中用来进行物体检测的特征描述子。它通过计算和统计图像局部区域的梯度方向直方图来构成特征。这种方法是类似于边缘方向直方图，尺度不变特征变换描述子，
形状上下文，但不同之处在于它是通过计算密集均匀间隔的网格细胞，应用重叠的局部对比度归一化来提高精度。
###2、主要思想和本质
一副图像中，局部目标的表象和形状能够被梯度或边缘的方向密度分布很好地描述。梯度的直方图统计信息，而梯度主要存在于边缘的地方。
###3、实现方法
首先将图像分成小的连通区域，我们把它叫细胞单元然后采集细胞单元中各像素点的梯度的或边缘的方向直方图，
并分别统计各个细胞直方图的方向特性，最后把这些直方图组合起来就可以构成特征描述器，输送给后端识别算法模块。
###4、实现步骤和参数
![](https://github.com/taoxic/matlab/raw/master/method/img/hogbuzhou.bmp)<br>
![](https://github.com/taoxic/matlab/raw/master/method/img/hogcanshu.bmp)
