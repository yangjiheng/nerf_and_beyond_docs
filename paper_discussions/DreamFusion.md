# Discussion on paper "DreamFusion: Text-to-3D using 2D Diffusion"

## Questions

Q1: Make-It-3D、DREAMFUSION中的分数知识蒸馏，只是学习扩散模型中的DIP梯度，预测更新方向吗

A: 对，本来还有一项U-Net的jacobian，但是被丢掉了
