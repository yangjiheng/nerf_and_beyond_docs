# Discussion on "Multi-Space Neural Radiance Fields"

## Summary

Highlights:
1. MS-NeRF，解决场景中反射和折射物体的理解和表达方法，对现有NeRF模型是一种增强。对相应场景的渲染效果提升极明显
2. 仅修改体渲染输出部分，输出层给出成对的densities和features（对应于多个平行的feature fields），然后使用体渲染得到多个feature map。最后使用两个小MLP输出RGB和weights
3. 相比基础NeRF，训练和推理的overhead增加较小
4. 相比Mip-NeRF 360，参数量提升0.5%，但PSNR提升3.46dB
5. 专门设计了一组新的镜面、折射类数据集，25个合成场景和7个自然采集场景
