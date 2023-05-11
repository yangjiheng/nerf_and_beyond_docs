# Discussion on "HumanRF: High-Fidelity Neural Radiance Fields for Humans in Motion"

## Summary

Highlight:
1. HumanRF，一个4D动态神经场表达，它可以通过多视角采集视频为输入，重建高质量人体运动效果，可以捕捉逼真的细节效果，保持时域和空域的一致性
2. 分辨率支持到1200万
3. 为了解决在内存约束情况下长序列处理问题，设计了一个自适应切分技术，在帧间尽可能共享feature，提高内存应用率
4. 提出ActorsHQ，一个使用160个相机拍摄的16个高清晰度，逐帧3D重建序列的数据集
5. 计划开源代码和数据集

Limitations:
1. Still do not have explicit control over articulation of the actor outside the training poses.
2. There is also significant room to speed up render times of our method
3. The foreground masks are not necessarily consistent across different time frames

## Questions

