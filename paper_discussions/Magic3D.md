# Discussion over paper: "Magic3D: High-Resolution Text-to-3D Content Creation"

## Questions

Q1: Magic3D里面从density得到sdf的方法，收敛了的RF的density field应该和sdf field的形状应该非常不接近，直接减去一个非零常数感觉不太对，感觉一个不太正确的初始化可能会导致模型会收敛到次优解

A：只是为了初始化吧，质量肯定不咋好，但比随机要好，然后在再优化

A: sdf对初始化真的敏感

**不知是否这里有优化空间**