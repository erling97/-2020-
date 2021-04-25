######
一、
模型误差的来源，有可能来自两方面  bias或者variance

variance可以认为是模型之间的方差，对于不同的训练集，如果模型越复杂，则模型受数据的影响越大，所以模型之间的variance会更大

![Uploading image.png…](https://github.com/erling97/hylee_2020.github.io/blob/main/photo/4.jpg)



bias则是预测模型f* 和真实函数f之间的偏差大小，一般模型越复杂，平均偏差越小

![Uploading image.png…](https://github.com/erling97/hylee_2020.github.io/blob/main/photo/5.jpg)


黑线是真实函数，然后随机取样5000次，红线为每次模拟的函数，蓝色为5000次建模的平均值，上下三个图，模型的复杂度依次提高

![Uploading image.png…](https://github.com/erling97/hylee_2020.github.io/blob/main/photo/6.jpg)


模型简单，可能bias大，variance小，模型复杂，bias小，但是variance大 

![Uploading image.png…](https://github.com/erling97/hylee_2020.github.io/blob/main/photo/7.jpg)


所以说，一般bias大，是欠拟合，需要考虑增加特征，增加模型复杂度
variance大是过拟合，方法一，需要考虑再去收集数据，如果不行，考虑人为扩增数据，比如图像识别时，可以让图片旋转等等方法，方法二就是正则化，
用来让模型更加平滑 


二、在真正建模的时候，比如比赛，把数据分为训练集、测试集、验证集，尽量少的用到验证集，更不要根据验证集去调整模型，这时候验证集所反映的bias才可能是真实的差值。

![Uploading image.png…](https://github.com/erling97/hylee_2020.github.io/blob/main/photo/8.jpg)
