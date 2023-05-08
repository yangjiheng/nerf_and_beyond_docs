# Discussion on "FreeNeRF: Improving Few-shot Neural Rendering with Free Frequency Regularization"

## Questions:

Q1: 完成这个工作的Intuition是什么？

Answer from Author:我们先是注意到了DietNeRF paper里的一个观察，就是用simplified nerf表现会比正常nerf好一些，之后进一步地看了下simplified NeRF起作用的模块是稍微降低了点最大的频率范围。后来我们干脆想着把高频全去掉，就有了paper里观察的现象，只保留低频信号的时候nerf除了过平滑的问题外，它的geometry就能学得很好。最后设计了从低到高逐渐放出高频信号的策略.

Q2: 作者有在ngp上试过类似的想法吗

Answer from Author: 还没有尝试，只是ngp上还没有frequency encoding的地方，后面准备拓展一下

Q3: 论文的第二个去floater的loss在更稠密视角下挺影响density分布学习的，怎么看？

Answer from Author: 是的，我们也观察到这个现象，有在limitation和appendix里讨论了这个问题。然后我们发现最近的nerfbuster里的visibility loss和freenerf里的occlusion loss形式很类似，但是惩罚的范围不太一样。后面也想详细看看对比一下。