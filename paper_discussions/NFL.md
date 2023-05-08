# Discussion over paper: "Neural LiDAR Fields for Novel View Synthesis"

## Summarization
* Highlight
    1. NFL: Neural Fields for LiDAR，一个NeRF形式的场景表达，用来解决LiDAR NVS问题
    2. 结合了NeRF的体渲染能力和LiDAR的物理采集模型，提升了生成质量
    3. 可用来增强下游任务，如point cloud registration, semantic segmentation等

* Limitation
    1. LiDAR的物理属性与semantic feature and learning的balance还有继续优化空间
    2. Prediction of the second return mask的优化将会继续提升效果
    3. 因依赖NeRF，所以需要per-scene optimization，Generalization accross scenes和处理动态场景将是未来工作方向
    