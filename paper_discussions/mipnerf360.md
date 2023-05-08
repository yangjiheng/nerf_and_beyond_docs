# Discussion on "Mip-NeRF 360: Unbounded Anti-Aliased Neural Radiance Fields"

## Question: 以下论述的解释是什么，原理是什么

    The original NeRF paper regularized ambiguous scenes by injecting Gaussian noise into the density headof the NeRF MLP before the rectifier [33], which encourages densities to gravitate towards either zero or infinity. Though this reduces some "floaters" by discouraging semi-transparent densities, we will show that it is insufficient forour more challenging task.

A: 理想的真值应该都是0和inf，半透明物体才理解为过拟合观测图像导致的泛化性不佳。加入噪声可以一定程度上避免过拟合，类似于dropout的效果，也和花书的内容一致。

A: 半透明体一般为floater，加入高斯噪声后，将density推向0或inf，降低半透明体存在的概率，一定程度上提升渲染质量

