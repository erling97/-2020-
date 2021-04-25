# -2021-4-25-
#回归
一、利用梯度下降，可能会陷入局部最优解，但是对于最简单的

![Uploading image.png…](https://github.com/erling97/-2020-/blob/main/photo/1.jpg)

只有全局最优解，因为这是一个凸函数，从二维图看起来就是

![Uploading image.png…](https://github.com/erling97/-2020-/blob/main/photo/2.jpg)

也就是说利用梯度下降会一步步找到这个全局最优解

二、正则化
当参数过多的时候，容易陷入过拟合，因此可以选择加入正则化项，使得模型的函数更加平滑，因为Loss函数里加入了参数的平方和，所以在Loss函数减小的过程中会让参数项尽可能减小，
同时有可能使有些特征的权重为0.

![Uploading image.png…](https://github.com/erling97/-2020-/blob/main/photo/3.jpg)

正则化时只加入了 w 的平方和，而没有加入 b 的平方和，因为 w 对函数平滑与否有影响，而 b 只会影响函数平移，所以无需加入。
