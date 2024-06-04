# <p align='center'>NeRF and Beyond Docs</p>

This is a collection of documents and topics NeRF & Beyond channel accumulated, as well as papers in literaure. This is still far from complete info regarding to this active research area. 

Some papers we discussed in the group, will be added to the back of the paper with a **Notes** link. You can follow the link to check whether there is topic you are interested in. If not, welcome to join us and ask the question to the crowd. The mighty community might have your answers.

We are actively maintaining this page trying to stay up-to-date and gather important works in a daily basis. We would also like to put as many notes as possible to some works, trying to make it easier to catch up. 

Please feel free to join us on WeChat group or start a discussion topic here.

## How to join us

For now, you can join us in the following ways

* [Bilibili Channel](https://space.bilibili.com/455056488) where we post near daily updates (primarily) on NeRF.
* WeChat group, due to the limitation of WeChat group, you can add my personal account: `jiheng_yang`, and I will add you to the chat groups.
* If you want to view this from a timeline perspective, please refer to this [ProcessOn Diagram](https://www.processon.com/view/link/643f8907f1144c215788f3e2)
* If you think something is not correct or you think we could do better in some way, please write to us through all possible channels or drop an issue. All suggestions are appreciated!
* For other discussed techniques that's related to 3D reconstruction and NeRF, please refer to [link](./NeRF_Related_Tech.md), we are constantly trying to add more resource to this document.
* We are trying to gradually setup Discord channels, join the [Discord Channel](https://discord.gg/AF2uMWGc) if you want to, we will certainly look forward to talk with you guys!

Recently there are lots of 3D Gaussian Splatting related work released. We move all related work to a new document for tracking in parallel.

## 3DGS Progresses
- [3D Gaussian Splatting Related Progresses](./3DGS.md)

## NeRF progresses

<summary>Table of Content</summary>

- [NeRF and Beyond Docs](#nerf-and-beyond-docs)
  - [How to join us](#how-to-join-us)
  - [3DGS Progresses](#3dgs-progresses)
  - [NeRF progresses](#nerf-progresses)
    - [New to NeRF](#new-to-nerf)
      - [**Begin of NeRF, Always Start Here**](#begin-of-nerf-always-start-here)
      - [**NeRF Related Surveys**](#nerf-related-surveys)
      - [**NeRF Tutorials**](#nerf-tutorials)
      - [**NeRF OpenSource Tools**](#nerf-opensource-tools)
    - [NeRF Fundamental Enhancements](#nerf-fundamental-enhancements)
    - [Robust Reconstruction \& Depth Supervised Reconstruction](#robust-reconstruction--depth-supervised-reconstruction)
    - [Activation Function Optimization](#activation-function-optimization)
    - [Positional Encoding](#positional-encoding)
    - [Deformable \& Dynamic NeRF](#deformable--dynamic-nerf)
    - [NeRF Training and Rendering Speed Enhancements](#nerf-training-and-rendering-speed-enhancements)
    - [One-Shot/Few-Shot Sparse View Reconstruction](#one-shotfew-shot-sparse-view-reconstruction)
    - [NeRF Based SLAM](#nerf-based-slam)
    - [Camera Pose Estimation \& Weak Camera Pose Reconstruction](#camera-pose-estimation--weak-camera-pose-reconstruction)
    - [Text to 3D](#text-to-3d)
      - [Survey](#survey)
      - [Progresses](#progresses)
    - [Diffusion Based NeRF Reconstruction](#diffusion-based-nerf-reconstruction)
    - [Generalization](#generalization)
    - [Model Compression](#model-compression)
    - [NeRF Based 2D High Quality Image Synthesis](#nerf-based-2d-high-quality-image-synthesis)
    - [SDF Based Reconstruction / Other Geometry Based Reconstruction](#sdf-based-reconstruction--other-geometry-based-reconstruction)
    - [NeRF + Hardware Acceleration](#nerf--hardware-acceleration)
    - [NeRF + Point Cloud / LiDAR](#nerf--point-cloud--lidar)
    - [NeRF + Auto Data Collection](#nerf--auto-data-collection)
    - [NeRF + Avatar/Talking Head](#nerf--avatartalking-head)
    - [NeRF + Imaging Tasks](#nerf--imaging-tasks)
    - [NeRF + Large Scale Scenes \& Urban Scenes](#nerf--large-scale-scenes--urban-scenes)
    - [NeRF + Autonomous Driving](#nerf--autonomous-driving)
    - [NeRF + Editing](#nerf--editing)
    - [NeRF + Open Surface Reconstruction and Cloth Simulation](#nerf--open-surface-reconstruction-and-cloth-simulation)
    - [NeRF + Segmentation](#nerf--segmentation)
    - [NeRF + Semantic](#nerf--semantic)
    - [NeRF + Mesh Extraction](#nerf--mesh-extraction)
    - [NeRF + Codec/Streaming](#nerf--codecstreaming)
    - [NeRF + Model Conversion](#nerf--model-conversion)
    - [NeRF + Medical/Biology](#nerf--medicalbiology)
    - [NeRF + Inverse Rendering](#nerf--inverse-rendering)
    - [NeRF + Texture Synthesis](#nerf--texture-synthesis)
    - [NeRF + Transparent Object](#nerf--transparent-object)
    - [NeRF + Transparent Object](#nerf--transparent-object-1)
  - [NeRF + Robotics](#nerf--robotics)
    - [NeRF + Transparent and Specular](#nerf--transparent-and-specular)
    - [Other 3D Generative Work](#other-3d-generative-work)
    - [NeRF + Other applications](#nerf--other-applications)
    - [NeRF + Quality Metric](#nerf--quality-metric)
    - [NeRF + CAD](#nerf--cad)
    - [NeRF + GIS](#nerf--gis)
    - [NeRF + Satellite Images](#nerf--satellite-images)
    - [NeRF + Copyright protection and Security](#nerf--copyright-protection-and-security)
    - [NeRF + Motion Detection](#nerf--motion-detection)
    - [Datasets](#datasets)
    - [Neural Surface Reconstruction](#neural-surface-reconstruction)
  - [Other Important Related Work](#other-important-related-work)
    - [Depth Estimation](#depth-estimation)
  - [Contributors](#contributors)
  - [License](#license)

### New to NeRF

#### **Begin of NeRF, Always Start Here**

:fire:**NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis**<br>
*Ben Mildenhall, Pratul P. Srinivasan, Matthew Tancik, Jonathan T. Barron, Ravi Ramamoorthi, Ren Ng*<br>
ECCV 2020, 19 Mar 2020 <br>
[[arXiv](https://arxiv.org/abs/2003.08934)] [[Project](https://www.matthewtancik.com/nerf)] [[Code](https://github.com/bmild/nerf)] [[PyTorch Impl](https://github.com/yenchenlin/nerf-pytorch)] [[Notes](./paper_discussions/NeRF.md)]

#### **NeRF Related Surveys**

:fire:**State of the Art on Neural Rendering**<br>
*Ayush Tewari, Ohad Fried, Justus Thies, Vincent Sitzmann, Stephen Lombardi, Kalyan Sunkavalli, Ricardo Martin-Brualla, Tomas Simon, Jason Saragih, Matthias Nießner, Rohit Pandey, Sean Fanello, Gordon Wetzstein, Jun-Yan Zhu, Christian Theobalt, Maneesh Agrawala, Eli Shechtman, Dan B Goldman, Michael Zollhöfer*<br>
ECCV 2020,8 Apr 2020<br>
[[arXiv](https://arxiv.org/abs/2004.03805)]

:fire:**Advances in Neural Rendering**<br>
*Ayush Tewari, Justus Thies, Ben Mildenhall, Pratul Srinivasan, Edgar Tretschk, Yifan Wang, Christoph Lassner, Vincent Sitzmann, Ricardo Martin-Brualla, Stephen Lombardi, Tomas Simon, Christian Theobalt, Matthias Niessner, Jonathan T. Barron, Gordon Wetzstein, Michael Zollhoefer, Vladislav Golyanik*<br>
ECCV 2022, 10 Nov 2021<br>
[[arXiv](https://arxiv.org/abs/2111.05849)]

:fire:**NeRF: Neural Radiance Field in 3D Vision, A Comprehensive Review**<br>
*Kyle Gao, Yina Gao, Hongjie He, Dening Lu, Linlin Xu, Jonathan Li*<br>
TPAMI 2022, 1 Oct 2022<br>
[[arXiv](https://arxiv.org/abs/2210.00379)]

**Neural Radiance Fields: Past, Present, and Future**<br>
*Ansh Mittal*<br>
In Progress,20 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.10050)]

#### **NeRF Tutorials**

:fire:**Neural Rendering Course**<br>
SIGGRAPH 2021 [[BiliBili](https://www.bilibili.com/video/BV1B3411q7hy)]

:fire:**Neural Volumetric Rendering for Computer Vision**<br>
ECCV 2022 Tutorial [[Website](https://sites.google.com/berkeley.edu/nerf-tutorial/home)]

:fire:**Scaling NeRF Up and Down: Big Scenes and Real-Time View Synthesis**<br>
I3D 2023 Keynote [[Video](https://www.bilibili.com/video/BV1fh4y1t7rW/)]

#### **NeRF OpenSource Tools**

:fire:**Nerfstudio: A Modular Framework for Neural Radiance Field Development**<br>
*Matthew Tancik, Ethan Weber, Evonne Ng, Ruilong Li, Brent Yi, Justin Kerr, Terrance Wang, Alexander Kristoffersen, Jake Austin, Kamyar Salahi, Abhik Ahuja, David McAllister, Angjoo Kanazawa*<br>
arXiv preprint, 8 Feb 2023<br>
>Nerfstudio provides a simple API that allows for a simplified end-to-end process of creating, training, and visualizing NeRFs. The library supports an interpretable implementation of NeRFs by modularizing each component.<br>

[[arXiv](https://arxiv.org/abs/2302.04264)] [[Website](https://docs.nerf.studio/en/latest/#)] [[Github](https://github.com/nerfstudio-project/nerfstudio)] 

:fire:**NerfAcc: Efficient Sampling Accelerates NeRFs**<br>
*Ruilong Li, Hang Gao, Matthew Tancik, Angjoo Kanazawa*<br>
arXiv preprint, 8 May 2023<br>
>NerfAcc is a PyTorch Nerf acceleration toolbox for both training and inference. It focus on efficient sampling in the volumetric rendering pipeline of radiance fields, which is universal and plug-and-play for most of the NeRFs. With minimal modifications to the existing codebases, Nerfacc provides significant speedups in training various recent NeRF papers. And it is pure Python interface with flexible APIs!<br>

[[arXiv](https://arxiv.org/abs/2305.04966)] [[Website](https://www.nerfacc.com/en/latest/index.html)]  [[Github](https://github.com/KAIR-BAIR/nerfacc)]

:fire:**threestudio: A unified framework for 3D content generation**<br>
*Yuan-Chen Guo and Ying-Tian Liu and Chen Wang and Zi-Xin Zou and Guan Luo and Chia-Hao Chen and Yan-Pei Cao and Song-Hai Zhang*<br>
Github repo,2023<br>
>threestudio is a unified framework for 3D content creation from text prompts, single images, and few-shot images, by lifting 2D text-to-image generation models.

[[Github](https://github.com/threestudio-project/threestudio)]

### NeRF Fundamental Enhancements

:fire:**NeRF in the Wild: Neural Radiance Fields for Unconstrained Photo Collections**<br>
*Ricardo Martin-Brualla, Noha Radwan, Mehdi S. M. Sajjadi, Jonathan T. Barron, Alexey Dosovitskiy, Daniel Duckworth*<br>
CVPR 2021, 5 Aug 2020 <br>
[[arXiv](https://arxiv.org/abs/2008.02268)] [[Project](https://nerf-w.github.io/)]

:fire:**Mip-NeRF: A Multiscale Representation for Anti-Aliasing Neural Radiance Fields**<br>
*Jonathan T. Barron, Ben Mildenhall, Matthew Tancik, Peter Hedman, Ricardo Martin-Brualla, Pratul P. Srinivasan*<br>
ICCV 2021, 24 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.13415)] [[Project](http://jonbarron.info/mipnerf)] [[Github](https://github.com/google/mipnerf)] [[Notes](./paper_discussions/mipnerf.md)]

:fire:**Mip-NeRF 360: Unbounded Anti-Aliased Neural Radiance Fields**<br>
*Jonathan T. Barron, Ben Mildenhall, Dor Verbin, Pratul P. Srinivasan, Peter Hedman*<br>
CVPR 2022, 23 Nov 2021<br>
[[arXiv](https://arxiv.org/abs/2111.12077)] [[Project](https://jonbarron.info/mipnerf360/)] [[Github](https://github.com/google-research/multinerf)] [[Notes](./paper_discussions/mipnerf360.md)]

:fire:**Ref-NeRF: Structured View-Dependent Appearance for Neural Radiance Fields**<br>
*Dor Verbin, Peter Hedman, Ben Mildenhall, Todd Zickler, Jonathan T. Barron, Pratul P. Srinivasan*<br>
CVPR 2022, 7 Dec 2021<br>
[[arXiv](https://arxiv.org/abs/2112.03907)] [[Project](https://dorverbin.github.io/refnerf/)] [[Github](https://github.com/google-research/multinerf)]

:fire:**PS-NeRF: Neural Inverse Rendering for Multi-view Photometric Stereo**<br>
*Wenqi Yang, Guanying Chen, Chaofeng Chen, Zhenfang Chen, Kwan-Yee K. Wong*<br>
ECCV 2022, 23 Jul 2022<br>
[[arXiv](https://arxiv.org/abs/2207.11406)] [[Project](https://ywq.github.io/psnerf/)] [[Github](https://github.com/ywq/psnerf)]

**4K-NeRF: High Fidelity Neural Radiance Fields at Ultra High Resolutions**<br>
*Zhongshu Wang, Lingzhi Li, Zhen Shen, Li Shen, Liefeng Bo*<br>
arXiv preprint, 9 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.04701)] [[Project](https://frozoul.github.io/4knerf/)] [[Github](https://github.com/frozoul/4K-NeRF)]

:fire:**Zip-NeRF: Anti-Aliased Grid-Based Neural Radiance Fields**<br>
*Jonathan T. Barron, Ben Mildenhall, Dor Verbin, Pratul P. Srinivasan, Peter Hedman*<br>
arXiv preprint, 13 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.06706)] [[Project](https://jonbarron.info/zipnerf/)] [[Unofficial Impl](https://github.com/SuLvXiangXin/zipnerf-pytorch)] [[Notes](./paper_discussions/Zip-NeRF.md)]

**Nerfbusters: Removing Ghostly Artifacts from Casually Captured NeRFs**<br>
*Frederik Warburg, Ethan Weber, Matthew Tancik, Aleksander Holynski, Angjoo Kanazawa*<br>
arXiv preprint, 20 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.10532)] [[Project](https://ethanweber.me/nerfbusters//)] [[Github](https://github.com/ethanweber/nerfbusters)] [[Video](https://www.bilibili.com/video/BV1hs4y197iN/)]

**Multi-Space Neural Radiance Fields**<br>
*Ze-Xin Yin, Jiaxiong Qiu, Ming-Ming Cheng, Bo Ren*<br>
CVPR 2023, 7 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.04268)] [[Project](https://zx-yin.github.io/msnerf/)] [[Github](https://github.com/ZX-Yin/ms-nerf)] [[Video](https://www.bilibili.com/video/BV1NX4y117mL/)] [[Notes](./paper_discussions/ms-nerf.md)]

**NeuManifold: Neural Watertight Manifold Reconstruction with Efficient and High-Quality Rendering Support**<br>
*Xinyue Wei, Fanbo Xiang, Sai Bi, Anpei Chen, Kalyan Sunkavalli, Zexiang Xu, Hao Su*<br>
arXiv preprint, 26 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.17134)] [[Project](https://sarahweiii.github.io/neumanifold/)] [[Video](https://www.bilibili.com/video/BV1qX4y1h7ku/)]

**Analyzing the Internals of Neural Radiance Fields**<br>
*Lukas Radl, Andreas Kurz, Markus Steinberger*<br>
arXiv preprint, 1 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.00696)] [[Project](http://nerfinternals.github.io/)]

**GANeRF: Leveraging Discriminators to Optimize Neural Radiance Fields**<br>
*Barbara Roessle, Norman Müller, Lorenzo Porzi, Samuel Rota Bulò, Peter Kontschieder, Matthias Nießner*<br>
arXiv preprint, 9 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.06044)] [[Video](https://www.bilibili.com/video/BV1fW4y1X7JU/)]

**HyP-NeRF: Learning Improved NeRF Priors using a HyperNetwork**<br>
*Bipasha Sen, Gaurav Singh, Aditya Agarwal, Rohith Agaram, K Madhava Krishna, Srinath Sridhar*<br>
arXiv preprint, 9 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.06093)]

:fire:**Tri-MipRF: Tri-Mip Representation for Efficient Anti-Aliasing Neural Radiance Fields**<br>
*Wenbo Hu, Yuling Wang, Lin Ma, Bangbang Yang, Lin Gao, Xiao Liu, Yuewen Ma*<br>
ICCV 2023, 21 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.11335)] [[Project](https://wbhu.github.io/projects/Tri-MipRF/)] [[Video](https://www.bilibili.com/video/BV1Lu41157Yj/)]

**Bayes' Rays: Uncertainty Quantification for Neural Radiance Fields**<br>
*Lily Goli, Cody Reading, Silvia Selllán, Alec Jacobson, Andrea Tagliasacchi*<br>
arXiv preprint, 6 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.03185)] [[Project](https://bayesrays.github.io/)]

**ResFields: Residual Neural Fields for Spatiotemporal Signals**<br>
*Marko Mihajlovic, Sergey Prokudin, Marc Pollefeys, Siyu Tang*<br>
arXiv preprint, 1 Oct 2023
[[arXiv](https://arxiv.org/abs/2309.03160#)] [[Project](https://markomih.github.io/ResFields/)] [[Github](https://github.com/markomih/ResFields)]

**NeuRBF: A Neural Fields Representation with Adaptive Radial Basis Functions**<br>
*Zhang Chen, Zhong Li, Liangchen Song, Lele Chen, Jingyi Yu, Junsong Yuan, Yi Xu*<br>
ICCV 2023, 27 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.15426)] [[Project](https://oppo-us-research.github.io/NeuRBF-website/)] [[Github](https://github.com/oppo-us-research/NeuRBF)]

**Multi-task View Synthesis with Neural Radiance Fields**<br>
*Shuhong Zheng, Zhipeng Bao, Martial Hebert, Yu-Xiong Wang*<br>
ICCV 2023, 29 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.17450)] [[Project](https://zsh2000.github.io/mtvs.github.io/)] [[Github](https://github.com/zsh2000/MuvieNeRF)]

**Hyb-NeRF: A Multiresolution Hybrid Encoding for Neural Radiance Fields**<br>
*Yifan Wang, Yi Gong, Yuan Zeng*<br>
arXiv preprint, 21 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.12490)]

**VQ-NeRF: Vector Quantization Enhances Implicit Neural Representations**<br>
*Yiying Yang, Wen Liu, Fukun Yin, Xin Chen, Gang Yu, Jiayuan Fan, Tao Chen*<br>
AAAI 2024, 23 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.14487)] 

**Rethinking Directional Integration in Neural Radiance Fields**<br>
*Congyue Deng, Jiawei Yang, Leonidas Guibas, Yue Wang*<br>
arXiv preprint, 28 Nov, 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16504)]

**RING-NeRF: A Versatile Architecture based on Residual Implicit Neural Grids**<br>
*Doriand Petit, Steve Bourgeois, Dumitru Pavel, Vincent Gay-Bellile, Florian Chabot, Loic Barthe*<br>
arXiv preprint, 6 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.03357)]

### Robust Reconstruction & Depth Supervised Reconstruction

:fire:**Depth-supervised NeRF: Fewer Views and Faster Training for Free**<br>
*Kangle Deng, Andrew Liu, Jun-Yan Zhu, Deva Ramanan*<br>
CVPR 2022, 6 Jul 2021<br>
[[arXiv](https://arxiv.org/abs/2107.02791)] [[Project](http://www.cs.cmu.edu/~dsnerf/)] [[Github](https://github.com/dunbar12138/DSNeRF)]

:fire:**NerfingMVS: Guided Optimization of Neural Radiance Fields for Indoor Multi-view Stereo**<br>
*Yi Wei, Shaohui Liu, Yongming Rao, Wang Zhao, Jiwen Lu, Jie Zhou*<br>
ICCV 2021, 2 Sep 2021<br>
[[arXiv](https://arxiv.org/abs/2109.01129)] [[Project](https://weiyithu.github.io/NerfingMVS)] [[Github](https://github.com/weiyithu/NerfingMVS)]

**Dense Depth Priors for Neural Radiance Fields from Sparse Input Views**<br>
*Barbara Roessle, Jonathan T. Barron, Ben Mildenhall, Pratul P. Srinivasan, Matthias Nießner*<br>
CVPR 2022, 6 Dec 2021<br>
[[arXiv](https://arxiv.org/abs/2112.03288)] [[Project](https://barbararoessle.github.io/dense_depth_priors_nerf/)] [[Github](https://github.com/barbararoessle/dense_depth_priors_nerf)]

**RobustNeRF: Ignoring Distractors with Robust Losses**<br>
*Sara Sabour, Suhani Vora, Daniel Duckworth, Ivan Krasin, David J. Fleet, Andrea Tagliasacchi*<br>
arXiv preprint, 2 Feb 2023<br>
[[arXiv](https://arxiv.org/abs/2302.00833)] [[Project](https://robustnerf.github.io/public/)]

**Digging into Depth Priors for Outdoor Neural Radiance Fields**<br>
*Chen Wang, Jiadai Sun, Lina Liu, Chenming Wu, Zhelun Shen, Dayan Wu, Yuchao Dai, Liangjun Zhang*<br>
ACMMM 2023, 8 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.04413)] [[Project](https://cwchenwang.github.io/outdoor-nerf-depth/)]

**AltNeRF: Learning Robust Neural Radiance Field via Alternating Depth-Pose Optimization**<br>
*Kun Wang, Zhiqiang Yan, Huang Tian, Zhenyu Zhang, Xiang Li, Jun Li, Jian Yang*<br>
arXiv preprint, 19 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.10001)]

### Activation Function Optimization

:fire:**Implicit Neural Representations with Periodic Activation Functions**<br>
*Vincent Sitzmann, Julien N. P. Martel, Alexander W. Bergman, David B. Lindell, Gordon Wetzstein*<br>
NeurIPS 2020, 17 Jun 2020<br>
[[arXiv](https://arxiv.org/abs/2006.09661)]

**Multiplicative Filter Networks**<br>
*Rizal Fathony, Anit Kumar Sahu, Devin Willmott, J Zico Kolter*<br>
ICLR 2021, 13 Jan 2021<br>
[[OpenReview](https://openreview.net/forum?id=OmtmcPkkhT)]

**PREF: Phasorial Embedding Fields for Compact Neural Representations**<br>
*Binbin Huang, Xinhao Yan, Anpei Chen, Shenghua Gao, Jingyi Yu*<br>
arXiv preprint, 26 May 2022<br>
[[avXiv](https://arxiv.org/abs/2205.13524)]

### Positional Encoding

**Fourier Features Let Networks Learn High Frequency Functions in Low Dimensional Domains**<br>
*Matthew Tancik, Pratul P. Srinivasan, Ben Mildenhall, Sara Fridovich-Keil, Nithin Raghavan, Utkarsh Singhal, Ravi Ramamoorthi, Jonathan T. Barron, Ren Ng*<br>
arXiv preprint, 18 Jun 2020<br>
[[arXiv](https://arxiv.org/abs/2006.10739)]

**BACON: Band-limited Coordinate Networks for Multiscale Scene Representation**<br>
*David B. Lindell, Dave Van Veen, Jeong Joon Park, Gordon Wetzstein*<br>
CVPR 2022, 9 Dec 2021<br>
[[arXiv](https://arxiv.org/abs/2112.04645)] [[Project](https://www.computationalimaging.org/publications/bacon/)] 

### Deformable & Dynamic NeRF

:fire:**Nerfies: Deformable Neural Radiance Fields**<br>
*Keunhong Park, Utkarsh Sinha, Jonathan T. Barron, Sofien Bouaziz, Dan B Goldman, Steven M. Seitz, Ricardo Martin-Brualla*<br>
ICCV 2021, 25 Nov 2020<br>
[[arXiv](https://arxiv.org/abs/2011.12948)] [[Project](https://nerfies.github.io/)] [[Github](https://github.com/google/nerfies)]

**Neural Scene Flow Fields for Space-Time View Synthesis of Dynamic Scenes**<br>
*Zhengqi Li, Simon Niklaus, Noah Snavely, Oliver Wang*<br>
CVPR 2021, 26 Nov 2020<br>
[[arXiv](https://arxiv.org/abs/2011.13084)] [[Project](http://www.cs.cornell.edu/~zl548/NSFF/)] [[Github](https://github.com/zhengqili/Neural-Scene-Flow-Fields)]

**HyperNeRF: A Higher-Dimensional Representation for Topologically Varying Neural Radiance Fields**<br>
*Keunhong Park, Utkarsh Sinha, Peter Hedman, Jonathan T. Barron, Sofien Bouaziz, Dan B Goldman, Ricardo Martin-Brualla, Steven M. Seitz*<br>
CVPR 2021, 24 Jun 2021<br>
[[arXiv](https://arxiv.org/abs/2106.13228)] [[Project](https://hypernerf.github.io/)] [[Github](https://github.com/google/hypernerf)]

**CodeNeRF: Disentangled Neural Radiance Fields for Object Categories**<br>
*Wonbong Jang, Lourdes Agapito*<br>
ICCV 2021, 3 Sep 2021<br>
[[arXiv](https://arxiv.org/abs/2109.01750)] [[Project](https://sites.google.com/view/wbjang/home/codenerf)] [[Github](https://github.com/wbjang/code-nerf)]

**Panoptic Neural Fields: A Semantic Object-Aware Neural Scene Representation**<br>
*Abhijit Kundu, Kyle Genova, Xiaoqi Yin, Alireza Fathi, Caroline Pantofaru, Leonidas Guibas, Andrea Tagliasacchi, Frank Dellaert, Thomas Funkhouser*<br>
CVPR 2022, 9 May 2022<br>
[[arXiv](https://arxiv.org/abs/2205.04334)] [[Project](https://abhijitkundu.info/projects/pnf/)]

**D2NeRF: Self-Supervised Decoupling of Dynamic and Static Objects from a Monocular Video**<br>
*Tianhao Wu, Fangcheng Zhong, Andrea Tagliasacchi, Forrester Cole, Cengiz Oztireli*<br>
CVPR 2022, 31 May 2022<br>
[[arXiv](https://arxiv.org/abs/2205.15838)] [[Project](https://d2nerf.github.io/)] [[Github](https://github.com/ChikaYan/d2nerf)]

:fire:**Deforming Radiance Fields with Cages**<br>
*Tianhan Xu, Tatsuya Harada*<br>
ECCV 2022, 25 Jul 2022<br>
[[arXiv](https://arxiv.org/abs/2207.12298)] [[Project](https://xth430.github.io/deforming-nerf/)] [[Github](https://github.com/xth430/deforming-nerf)]

:fire:**NeRFPlayer: A Streamable Dynamic Scene Representation with Decomposed Neural Radiance Fields**<br>
*Liangchen Song, Anpei Chen, Zhong Li, Zhang Chen, Lele Chen, Junsong Yuan, Yi Xu, Andreas Geiger*<br>
IEEE TVCG, 28 Oct 2022<br>
[[arXiv](https://arxiv.org/abs/2210.15947)] [[Project](https://lsongx.github.io/projects/nerfplayer.html)] [[Github(in nerfstudio)](https://github.com/nerfstudio-project/nerfstudio)]

**Robust Dynamic Radiance Fields**<br>
*Yu-Lun Liu, Chen Gao, Andreas Meuleman, Hung-Yu Tseng, Ayush Saraf, Changil Kim, Yung-Yu Chuang, Johannes Kopf, Jia-Bin Huang*<br>
CVPR 2023, 5 Jan 2023<br>
[[arXiv](https://arxiv.org/abs/2301.02239)] [[Project](https://robust-dynrf.github.io/)]

:fire:**HyperReel: High-Fidelity 6-DoF Video with Ray-Conditioned Sampling**<br>
*Benjamin Attal, Jia-Bin Huang, Christian Richardt, Michael Zollhoefer, Johannes Kopf, Matthew O'Toole, Changil Kim*<br>
arXiv preprint, 5 Jan 2023<br>
[[arXiv](https://arxiv.org/abs/2301.02238)] [[Project](https://hyperreel.github.io/)] [[Github](https://github.com/facebookresearch/hyperreel)]

**CageNeRF: Cage-based Neural Radiance Field for Generalized 3D Deformation and Animation**<br>
*Yicong Peng, Yichao Yan, Shengqi Liu, Yuhao Cheng, Shanyan Guan, Bowen Pan, Guangtao Zhai, Xiaokang Yang*<br>
NeurIPS 2022, 01 Nov 2022<br>
[[OpenReview](https://openreview.net/forum?id=kUnHCGiILeU)] [[Zhihu](https://zhuanlan.zhihu.com/p/581808674)] [[Github](https://github.com/PengYicong/CageNeRF)]

**DynIBaR: Neural Dynamic Image-Based Rendering**<br>
*Zhengqi Li, Qianqian Wang, Forrester Cole, Richard Tucker, Noah Snavely*<br>
CVPR 2023, 20 Nov 2022<br>
[[arXiv](https://arxiv.org/abs/2211.11082)] [[Project](https://dynibar.github.io/)] [[Github](https://github.com/google/dynibar)] [[Video](https://www.bilibili.com/video/BV1hM4y1v77P/)]

**MonoNeRF: Learning a Generalizable Dynamic Radiance Field from Monocular Videos**<br>
*Fengrui Tian, Shaoyi Du, Yueqi Duan*<br>
ICCV 2023, 26 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.13056)] [[Github](https://github.com/tianfr/MonoNeRF)]

**Robust Dynamic Radiance Fields**<br>
*Yu-Lun Liu, Chen Gao, Andreas Meuleman, Hung-Yu Tseng, Ayush Saraf, Changil Kim, Yung-Yu Chuang, Johannes Kopf, Jia-Bin Huang*<br>
CVPR 2023,  5 Jan 2023 <br>
[[arXiv](https://arxiv.org/abs/2301.02239)] [[Project](https://robust-dynrf.github.io/)] [[Video](https://www.bilibili.com/video/BV15z4y1B7QZ/)]

:fire:**HexPlane: A Fast Representation for Dynamic Scenes**<br>
*Ang Cao, Justin Johnson*<br>
CVPR 2023, 23 Jan 2023<br>
[[arXiv](https://arxiv.org/abs/2301.09632)] [[Project](https://caoang327.github.io/HexPlane)] [[Github](https://github.com/Caoang327/HexPlane)]

:fire:**K-Planes: Explicit Radiance Fields in Space, Time, and Appearance**<br>
*Sara Fridovich-Keil, Giacomo Meanti, Frederik Warburg, Benjamin Recht, Angjoo Kanazawa*<br>
CVPR 2023, 24 Jan 2023<br>
[[arXiv](https://arxiv.org/abs/2301.10241)] [[Project](https://sarafridov.github.io/K-Planes/)] [[Github](https://github.com/sarafridov/K-Planes)] [[Notes](./paper_discussions/KPlane.md)]

**PAC-NeRF: Physics Augmented Continuum Neural Radiance Fields for Geometry-Agnostic System Identification**<br>
*Xuan Li, Yi-Ling Qiao, Peter Yichen Chen, Krishna Murthy Jatavallabhula, Ming Lin, Chenfanfu Jiang, Chuang Gan*<br>
ICLR 2023, 02 Feb 2023<br>
[[OpenReview](https://openreview.net/forum?id=tVkrbkz42vc)] [[Project](https://xuan-li.github.io/PAC-NeRF/)] [[Github](https://github.com/xuan-li/PAC-NeRF)]

**Temporal Interpolation Is All You Need for Dynamic Neural Radiance Fields**<br>
*Sungheon Park, Minjung Son, Seokhwan Jang, Young Chun Ahn, Ji-Yeon Kim, Nahyup Kang*<br>
CVPR 2023, 18 Feb 2023<br>
[[arXiv](https://arxiv.org/abs/2302.09311)] [[Project](https://sungheonpark.github.io/tempinterpnerf/)] [[Video](https://www.bilibili.com/video/BV19u4y1Z7rk/)]

**OD-NeRF: Efficient Training of On-the-Fly Dynamic Neural Radiance Fields**<br>
*Zhiwen Yan, Chen Li, Gim Hee Lee*<br>
arXiv preprint, 24 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.14831)]

**SceNeRFlow: Time-Consistent Reconstruction of General Dynamic Scenes**<br>
*Authors: Edith Tretschk, Vladislav Golyanik, Michael Zollhoefer, Aljaz Bozic, Christoph Lassner, Christian Theobalt*<br>
arXiv preprint, 16 August, 2023<br>
[[arXiv](https://arxiv.org/abs/2308.08258)] [[Project](https://vcai.mpi-inf.mpg.de/projects/scenerflow/)] [[Video](https://www.bilibili.com/video/BV1v94y167So/)]

**ResFields: Residual Neural Fields for Spatiotemporal Signals**<br>
*Marko Mihajlovic, Sergey Prokudin, Marc Pollefeys, Siyu Tang*<br>
arXiv preprint, 6 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.03160)] [[Project](https://markomih.github.io/ResFields/)] [[Github](https://github.com/markomih/ResFields)]

**Dynamic Mesh-Aware Radiance Fields**<br>
*Yi-Ling Qiao, Alexander Gao, Yiran Xu, Yue Feng, Jia-Bin Huang, Ming C. Lin*<br>
ICCV 2023, 8 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.04581)] [[Project](https://mesh-aware-rf.github.io/)] [[Github](https://github.com/YilingQiao/DMRF/tree/cleaning)]

**DynaMoN: Motion-Aware Fast And Robust Camera Localization for Dynamic NeRF**<br>
*Mert Asim Karaoglu, Hannah Schieber, Nicolas Schischka, Melih Görgülü, Florian Grötzner, Alexander Ladikos, Daniel Roth, Nassir Navab, Benjamin Busam*<br>
arXiv preprint, 16 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.08927)]

**Point-DynRF: Point-based Dynamic Radiance Fields from a Monocular Video**<br>
*Byeongjun Park, Changick Kim*<br>
WACV 2024, 14 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.09647)]

**Sync-NeRF: Generalizing Dynamic NeRFs to Unsynchronized Videos**<br>
*Seoha Kim, Jeongmin Bae, Youngsik Yun, Hahyun Lee, Gun Bang, Youngjung Uh*<br>
arXiv preprint, 20 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.13356)] [[Project](https://seoha-kim.github.io/sync-nerf)]

**DreaMo: Articulated 3D Reconstruction From A Single Casual Video**<br>
*Tao Tu, Ming-Feng Li, Chieh Hubert Lin, Yen-Chi Cheng, Min Sun, Ming-Hsuan Yang*<br>
arXiv preprint, 5 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02617)] [[Project](https://ttaoretw.github.io/DreaMo/)]

**NeVRF: Neural Video-based Radiance Fields for Long-duration Sequences**<br>
*Minye Wu, Tinne Tuytelaars*<br>
arXiv preprint, 10 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.05855)]

### NeRF Training and Rendering Speed Enhancements

:fire:**Neural Sparse Voxel Fields**<br>
*Lingjie Liu, Jiatao Gu, Kyaw Zaw Lin, Tat-Seng Chua, Christian Theobalt*<br>
NeurIPS 2020, 22 Jul 2020<br>
[[arXiv](https://arxiv.org/abs/2007.11571)]

:fire:**NeRF++: Analyzing and Improving Neural Radiance Fields**<br>
*Kai Zhang, Gernot Riegler, Noah Snavely, Vladlen Koltun*<br>
arXiv Preprint 2020, 15 Oct 2020<br>
[[arXiv](https://arxiv.org/abs/2010.07492)] [[Github](https://github.com/Kai-46/nerfplusplus)]

**DeRF: Decomposed Radiance Fields**<br>
*Daniel Rebain, Wei Jiang, Soroosh Yazdani, Ke Li, Kwang Moo Yi, Andrea Tagliasacchi*<br>
CVPR 2021, 25 Nov 2020<br>
[[arXiv](https://arxiv.org/abs/2011.12490)] [[Project](https://ubc-vision.github.io/derf/)] [[Github](https://github.com/ubc-vision/derf/)]

:fire:**AutoInt: Automatic Integration for Fast Neural Volume Rendering**<br>
*David B. Lindell, Julien N. P. Martel, Gordon Wetzstein*<br>
CVPR 2021, 15 Oct 2020<br>
[[arXiv](https://arxiv.org/abs/2012.01714)] [[Github](https://github.com/computational-imaging/automatic-integration)]

**DONeRF: Towards Real-Time Rendering of Compact Neural Radiance Fields using Depth Oracle Networks**<br>
*Thomas Neff, Pascal Stadlbauer, Mathias Parger, Andreas Kurz, Joerg H. Mueller, Chakravarty R. Alla Chaitanya, Anton Kaplanyan, Markus Steinberger*<br>
EGSR 2021, 4 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.03231)] [[Project](https://depthoraclenerf.github.io/)] [[Github](https://github.com/facebookresearch/DONERF)]

**FastNeRF: High-Fidelity Neural Rendering at 200FPS**<br>
*Stephan J. Garbin, Marek Kowalski, Matthew Johnson, Jamie Shotton, Julien Valentin*<br>
ICCV 2021, 18 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.10380)] [[Project](https://microsoft.github.io/FastNeRF/)] 

**KiloNeRF: Speeding up Neural Radiance Fields with Thousands of Tiny MLPs**<br>
*Christian Reiser, Songyou Peng, Yiyi Liao, Andreas Geiger*<br>
ICCV 2021, 25 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.13744)] [[Github](https://github.com/creiser/kilonerf/)]

:fire:**PlenOctrees for Real-time Rendering of Neural Radiance Fields**<br>
*Alex Yu, Ruilong Li, Matthew Tancik, Hao Li, Ren Ng, Angjoo Kanazawa*<br>
ICCV 2021, 25 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.14024)] [[Project](https://alexyu.net/plenoctrees/)] [[Github](https://github.com/sxyu/plenoctree)] [[Viewer Github](https://github.com/sxyu/volrend)]

:fire:**Baking Neural Radiance Fields for Real-Time View Synthesis**<br>
*Peter Hedman, Pratul P. Srinivasan, Ben Mildenhall, Jonathan T. Barron, Paul Debevec*<br>
ICCV 2021, 26 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.14645)] [[Project](https://phog.github.io/snerg/)] [[Github](https://github.com/google-research/google-research/tree/master/snerg)]

**Direct Voxel Grid Optimization: Super-fast Convergence for Radiance Fields Reconstruction**<br>
*Cheng Sun, Min Sun, Hwann-Tzong Chen*<br>
CVPR 2022, 22 Nov 2021<br>
[[arXiv](https://arxiv.org/abs/2111.11215)] [[Project](https://sunset1995.github.io/dvgo/)] [[Github](https://github.com/sunset1995/DirectVoxGO)]

**VaxNeRF: Revisiting the Classic for Voxel-Accelerated Neural Radiance Field**<br>
*Naruya Kondo, Yuya Ikeda, Andrea Tagliasacchi, Yutaka Matsuo, Yoichi Ochiai, Shixiang Shane Gu*<br>
arXiv preprint, 25 Nov 2021<br>
[[arXiv](https://arxiv.org/abs/2111.13112)] [[Github](https://github.com/naruya/VaxNeRF)]

**NeuSample: Neural Sample Field for Efficient View Synthesis**<br>
*Naruya Kondo, Yuya Ikeda, Andrea Tagliasacchi, Yutaka Matsuo, Yoichi Ochiai, Shixiang Shane Gu*<br>
arXiv preprint, 30 Nov 2021<br>
[[arXiv](https://arxiv.org/abs/2111.15552)] [[Project](https://jaminfong.cn/neusample)] [[Github](https://github.com/hustvl/NeuSample)]

:fire:**Plenoxels: Radiance Fields without Neural Networks**<br>
*Alex Yu, Sara Fridovich-Keil, Matthew Tancik, Qinhong Chen, Benjamin Recht, Angjoo Kanazawa*<br>
arXiv preprint, 30 Nov 2021<br>
[[arXiv](https://arxiv.org/abs/2112.05131)] [[Project](https://alexyu.net/plenoxels/)] [[Github](https://github.com/sxyu/svox2)]

:fire:**Instant Neural Graphics Primitives with a Multiresolution Hash Encoding**<br>
*Thomas Müller, Alex Evans, Christoph Schied, Alexander Keller*<br>
SIGGRAPH 2022, 16 Jan 2022<br>
[[arXiv](https://arxiv.org/abs/2201.05989)] [[Project](https://nvlabs.github.io/instant-ngp/)] [[Github](https://github.com/NVlabs/instant-ngp)]

:fire:**TensoRF: Tensorial Radiance Fields**<br>
*Anpei Chen, Zexiang Xu, Andreas Geiger, Jingyi Yu, Hao Su*<br>
ECCV 2022, 17 Mar 2022<br>
[[arXiv](https://arxiv.org/abs/2203.09517)] [[Project](https://apchenstu.github.io/TensoRF/)] [[Github](https://github.com/apchenstu/TensoRF)] [[Notes](./paper_discussions/TensoRF.md)]

**SqueezeNeRF: Further factorized FastNeRF for memory-efficient inference**<br>
*Krishna Wadhwani, Tamaki Kojima*<br>
arXiv preprint, 6 Apr 2022<br>
[[arXiv](https://arxiv.org/abs/2204.02585)]

**AdaNeRF: Adaptive Sampling for Real-Time Rendering of Neural Radiance Fields**<br>
*Andreas Kurz, Thomas Neff, Zhaoyang Lv, Michael Zollhöfer, Markus Steinberger*<br>
ECCV 2022, 21 Jul 2022<br>
[[arXiv](https://arxiv.org/abs/2207.10312)] [[Project](https://thomasneff.github.io/adanerf/)] [[Github](https://github.com/thomasneff/AdaNeRF)]

:fire:**MobileNeRF: Exploiting the Polygon Rasterization Pipeline for Efficient Neural Field Rendering on Mobile Architectures**<br>
*Zhiqin Chen, Thomas Funkhouser, Peter Hedman, Andrea Tagliasacchi*<br>
CVPR 2023, 30 Jul 2022<br>
[[arXiv](https://arxiv.org/abs/2208.00277)] [[Project](https://mobile-nerf.github.io/)] [[Github](https://github.com/google-research/jax3d/tree/main/jax3d/projects/mobilenerf)]

**Real-Time Neural Light Field on Mobile Devices**<br>
*Junli Cao, Huan Wang, Pavlo Chemerys, Vladislav Shakhrai, Ju Hu, Yun Fu, Denys Makoviichuk, Sergey Tulyakov, Jian Ren*<br>
CVPR 2023, 15 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.08057)] [[Project](https://snap-research.github.io/MobileR2L/)] [[Github](https://github.com/snap-research/MobileR2L)]

**Factor Fields: A Unified Framework for Neural Fields and Beyond**
*Anpei Chen, Zexiang Xu, Xinyue Wei, Siyu Tang, Hao Su, Andreas Geiger*<br>
arXiv preprint, 2 Feb 2023<br>
[[arXiv](https://arxiv.org/abs/2302.01226)] [[Project](https://apchenstu.github.io/FactorFields/)] [[Github](https://github.com/autonomousvision/factor-fields)]

:fire:**MERF: Memory-Efficient Radiance Fields for Real-time View Synthesis in Unbounded Scenes**<br>
*Christian Reiser, Richard Szeliski, Dor Verbin, Pratul P. Srinivasan, Ben Mildenhall, Andreas Geiger, Jonathan T. Barron, Peter Hedman*<br>
arXiv preprint, 23 Feb 2023<br>
[[arXiv](https://arxiv.org/abs/2302.12249)] [[Project](https://merf42.github.io/)]

:fire:**BakedSDF: Meshing Neural SDFs for Real-Time View Synthesis**<br>
*Lior Yariv, Peter Hedman, Christian Reiser, Dor Verbin, Pratul P. Srinivasan, Richard Szeliski, Jonathan T. Barron, Ben Mildenhall*<br>
arXiv preprint, 28 Feb 2023<br>
[[arXiv](https://arxiv.org/abs/2302.14859)] [[Project](https://bakedsdf.github.io/)]

**Volume Feature Rendering for Fast Neural Radiance Field Reconstruction**<br>
*Kang Han, Wei Xiang, Lu Yu*<br>
arXiv preprint, 29 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.17916)]

**Compact Real-time Radiance Fields with Neural Codebook**<br>
*Lingzhi Li, Zhongshu Wang, Zhen Shen, Li Shen, Ping Tan*<br>
ICME 2023, 29 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.18163)]

**Dictionary Fields: Learning a Neural Basis Decomposition**<br>
*Anpei Chen, Zexiang Xu, Xinyue Wei, Siyu Tang, Hao Su, Andreas Geiger*<br>
SIGGRAPH 2023<br>
[[Paper](https://apchenstu.github.io/FactorFields/Dictionary_Fields.pdf)] [[Github](https://github.com/autonomousvision/factor-fields)]

**NAS-NeRF: Generative Neural Architecture Search for Neural Radiance Fields**<br>
*NAS-NeRF: Generative Neural Architecture Search for Neural Radiance Fields*<br>
arXiv preprint, 25 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.14293)] [[Project](https://saeejithnair.github.io/NAS-NeRF/)]

**Adaptive Multi-NeRF: Exploit Efficient Parallelism in Adaptive Multiple Scale Neural Radiance Field Rendering**<br>
*Tong Wang, Shuichi Kurabayashi*<br>
arXiv preprint, 3 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.01881)]

**MIMO-NeRF: Fast Neural Rendering with Multi-input Multi-output Neural Radiance Fields**<br>
*Takuhiro Kaneko*<br>
ICCV 2023,  3 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.01821)] [[Project](https://www.kecl.ntt.co.jp/people/kaneko.takuhiro/projects/mimo-nerf/)]

**Neural Processing of Tri-Plane Hybrid Neural Fields**<br>
*Adriano Cardace, Pierluigi Zama Ramirez, Francesco Ballerini, Allan Zhou, Samuele Salti, Luigi Di Stefano*<br>
arXiv preprint, 2 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.01140)]

**CAwa-NeRF: Instant Learning of Compression-Aware NeRF Features**<br>
*Omnia Mahmoud, Théo Ladune, Matthieu Gendrin*<br>
arXiv preprint, 23 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.14695)]

**Efficient Encoding of Graphics Primitives with Simplex-based Structures**<br>
*Yibo Wen, Yunfan Yang*<br>
arXiv preprint, 26 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.15439)]

**ProNeRF: Learning Efficient Projection-Aware Ray Sampling for Fine-Grained Implicit Neural Radiance Fields**<br>
*Juan Luis Gonzalez Bello, Minh-Quan Viet Bui, Munchurl Kim*<br>
arXiv preprint, 13 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.08136)] [[Project](https://kaist-viclab.github.io/pronerf-site/)] [[Code](https://github.com/KAIST-VICLab/pronerf)]


### One-Shot/Few-Shot Sparse View Reconstruction

:fire:**pixelNeRF: Neural Radiance Fields from One or Few Images**<br>
*Alex Yu, Vickie Ye, Matthew Tancik, Angjoo Kanazawa*<br>
CVPR 2021, 3 Dec 2020<br>
[[arXiv](https://arxiv.org/abs/2012.02190)] [[Project](https://alexyu.net/pixelnerf/)] [[Github](https://github.com/sxyu/pixel-nerf)]

**IBRNet: Learning Multi-View Image-Based Rendering**<br>
*Qianqian Wang, Zhicheng Wang, Kyle Genova, Pratul Srinivasan, Howard Zhou, Jonathan T. Barron, Ricardo Martin-Brualla, Noah Snavely, Thomas Funkhouser*<br>
CVPR 2021, 25 Feb 2021<br>
[[arXiv](https://arxiv.org/abs/2102.13090)] [[Project](https://ibrnet.github.io/)] [[Github](https://github.com/googleinterns/IBRNet)]

:fire:**Putting NeRF on a Diet: Semantically Consistent Few-Shot View Synthesis**<br>
*Ajay Jain, Matthew Tancik, Pieter Abbeel*<br>
arXiv preprint, 1 Apr 2021<br>
[[arXiv](https://arxiv.org/abs/2104.00677)] [[Project](https://www.ajayj.com/dietnerf)] [[Github](https://github.com/ajayjain/DietNeRF)]

**MINE: Towards Continuous Depth MPI with NeRF for Novel View Synthesis**<br>
*Jiaxin Li, Zijian Feng, Qi She, Henghui Ding, Changhu Wang, Gim Hee Lee*<br>
ICCV 2021, 27 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.14910)] [[Project](https://vincentfung13.github.io/projects/nemi/)] [[Github](https://github.com/vincentfung13/MINE)]

:fire:**MVSNeRF: Fast Generalizable Radiance Field Reconstruction from Multi-View Stereo**<br>
*Anpei Chen, Zexiang Xu, Fuqiang Zhao, Xiaoshuai Zhang, Fanbo Xiang, Jingyi Yu, Hao Su*<br>
ICCV 2021, 29 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.15595)] [[Project](https://apchenstu.github.io/mvsnerf/)] [[Github](https://github.com/apchenstu/mvsnerf)]

**Common Objects in 3D: Large-Scale Learning and Evaluation of Real-life 3D Category Reconstruction**<br>
*Jeremy Reizenstein, Roman Shapovalov, Philipp Henzler, Luca Sbordone, Patrick Labatut, David Novotny*<br>
ICCV 2021, 29 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2109.00512)] [[Co3D Dataset](https://github.com/facebookresearch/co3d)]

**RegNeRF: Regularizing Neural Radiance Fields for View Synthesis from Sparse Inputs**<br>
*Michael Niemeyer, Jonathan T. Barron, Ben Mildenhall, Mehdi S. M. Sajjadi, Andreas Geiger, Noha Radwan*<br>
CVPR 2022, 1 Dec 2021<br>
[[arXiv](https://arxiv.org/abs/2112.00724)] [[Project](https://m-niemeyer.github.io/regnerf/index.html)] [[Code](https://github.com/google-research/google-research/tree/master/regnerf)] [[Notes](./paper_discussions/RegNeRF.md)]

:fire:**ViewFormer: NeRF-free Neural Rendering from Few Images Using Transformers**<br>
*Jonáš Kulhánek, Erik Derner, Torsten Sattler, Robert Babuška*<br>
ECCV 2022, 18 Mar 2022<br>
[[arXiv](https://arxiv.org/abs/2203.10157)] [[Project](https://jkulhanek.github.io/viewformer)] [[Github](https://github.com/jkulhanek/viewformer)]

**S3-NeRF: Neural Reflectance Field from Shading and Shadow under a Single Viewpoint**<br>
*Wenqi Yang, Guanying Chen, Chaofeng Chen, Zhenfang Chen, Kwan-Yee K. Wong*<br>
NeurIPS 2022, 17 Oct 2022<br>
[[arXiv](https://arxiv.org/abs/2210.08936)] [[Project](https://ywq.github.io/s3nerf/)] [[Github](https://github.com/ywq/s3nerf)]

**NeuralLift-360: Lifting An In-the-wild 2D Photo to A 3D Object with 360° Views**<br>
*Wenqi Yang, Guanying Chen, Chaofeng Chen, Zhenfang Chen, Kwan-Yee K. Wong*<br>
arXiv preprint, 29 Nov 2022<br>
[[arXiv](https://arxiv.org/abs/2211.16431)] [[Project](https://vita-group.github.io/NeuralLift-360/)] [[Github](https://github.com/VITA-Group/NeuralLift-360)]

**SPARF: Large-Scale Learning of 3D Sparse Radiance Fields from Few Input Images**<br>
*Abdullah Hamdi, Bernard Ghanem, Matthias Nießner*<br>
arXiv preprint, 18 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.09100)] [[Project](https://abdullahamdi.com/sparf/)] [[Github](https://github.com/ajhamdi/sparf_pytorch)]

**Geometry-biased Transformers for Novel View Synthesis**<br>
*Naveen Venkat, Mayank Agarwal, Maneesh Singh, Shubham Tulsiani*<br>
arXiv preprint, 11 Jan 2023<br>
[[arXiv](https://arxiv.org/abs/2301.04650)] [[Project](https://mayankgrwl97.github.io/gbt/)] [[Github](https://github.com/mayankgrwl97/gbt)]

**Behind the Scenes: Density Fields for Single View Reconstruction**<br>
*Felix Wimbauer, Nan Yang, Christian Rupprecht, Daniel Cremers*<br>
CVPR 2023, 18 Jan 2023<br>
[[arXiv](https://arxiv.org/abs/2301.07668)] [[Project](https://fwmb.github.io/bts/)] [[Github](https://github.com/Brummi/BehindTheScenes)] [[Video](https://www.bilibili.com/video/BV1Pc411V7aP/)]

**NerfDiff: Single-image View Synthesis with NeRF-guided Distillation from 3D-aware Diffusion**<br>
*Jiatao Gu, Alex Trevithick, Kai-En Lin, Josh Susskind, Christian Theobalt, Lingjie Liu, Ravi Ramamoorthi*<br>
arXiv preprint, 20 Feb 2023 <br>
[[arXiv](https://arxiv.org/abs/2302.10109)] [[Project](https://jiataogu.me/nerfdiff/)]

**DiffusioNeRF: Regularizing Neural Radiance Fields with Denoising Diffusion Models**<br>
*Jamie Wynn, Daniyar Turmukhambetov*<br>
arXiv preprint, 23 Feb 2023 <br>
[[arXiv](https://arxiv.org/abs/2302.12231)] [[Github](https://github.com/nianticlabs/diffusionerf)]

:fire:**FreeNeRF: Improving Few-shot Neural Rendering with Free Frequency Regularization**<br>
*Jiawei Yang, Marco Pavone, Yue Wang*<br>
CVPR 2023, 13 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.07418)] [[Project](https://jiawei-yang.github.io/FreeNeRF/)] [[Github](https://github.com/Jiawei-Yang/FreeNeRF)] [[Notes](./paper_discussions/FreeNeRF.md)]

**Zero-1-to-3: Zero-shot One Image to 3D Object**<br>
*Jiawei Yang, Marco Pavone, Yue Wang*<br>
CVPR 2023, 20 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.11328)] [[Project](https://zero123.cs.columbia.edu/)] [[Github](https://github.com/cvlab-columbia/zero123)]

**SparseNeRF: Distilling Depth Ranking for Few-shot Novel View Synthesis**<br>
*Guangcong Wang, Zhaoxi Chen, Chen Change Loy, Ziwei Liu*<br>
ICCV 2023, 28 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.16196)] [[Project](https://sparsenerf.github.io/)] [[Github](https://sparsenerf.github.io/)]

**VGOS: Voxel Grid Optimization for View Synthesis from Sparse Inputs**<br>
*Jiakai Sun, Zhanjie Zhang, Jiafu Chen, Guangyuan Li, Boyan Ji, Lei Zhao, Wei Xing*<br>
IJCAI 2023, 26 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.13386)] [[Github](https://github.com/SJoJoK/VGOS)]

**ViP-NeRF: Visibility Prior for Sparse Input Neural Radiance Fields**<br>
*Nagabhushan Somraj, Rajiv Soundararajan*<br>
SIGGRAPH 2023, 28 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2305.00041)] [[Project](https://nagabhushansn95.github.io/publications/2023/ViP-NeRF.html)] [[Github](https://github.com/NagabhushanSN95/ViP-NeRF)] [[Video](https://www.bilibili.com/video/BV1gg4y1K7QV/)]

**DäRF: Boosting Radiance Fields from Sparse Inputs with Monocular Depth Adaptation**<br>
*Jiuhn Song, Seonghoon Park, Honggyu An, Seokju Cho, Min-Seop Kwak, Sungjin Cho, Seungryong Kim*<br>
arXiv preprint, 30 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.19201)] [[Project](https://ku-cvlab.github.io/DaRF/)]

**ZIGNeRF: Zero-shot 3D Scene Representation with Invertible Generative Neural Radiance Fields**<br>
*Kanghyeok Ko, Minhyeok Lee*<br>
arXiv preprint, 5 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.02741)]

**Car-Studio: Learning Car Radiance Fields from Single-View and Endless In-the-wild Images**<br>
*Tianyu Liu, Hao Zhao, Yang Yu, Guyue Zhou, Ming Liu*<br>
IEEE RA-L, 26 Jul, 2023<br>
[[arXiv](https://arxiv.org/abs/2307.14009)] [[Project](https://lty2226262.github.io/car-studio/)]

**Where and How: Mitigating Confusion in Neural Radiance Fields from Sparse Inputs**<br>
*Yanqi Bao, Yuxin Li, Jing Huo, Tianyu Ding, Xinyue Liang, Wenbin Li, Yang Gao*<br>
ACMMM 2023, 5 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.02908)] [[Github](https://github.com/bbbbby-99/WaH-NeRF)]

**Novel-view Synthesis and Pose Estimation for Hand-Object Interaction from Sparse Views**<br>
*Wentian Qu, Zhaopeng Cui, Yinda Zhang, Chenyu Meng, Cuixia Ma, Xiaoming Deng, Hongan Wang*<br>
arXiv preprint, 22 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.11198)] [[Project](https://iscas3dv.github.io/HO-NeRF)]

**PERF: Panoramic Neural Radiance Field from a Single Panorama**<br>
*Guangcong Wang, Peng Wang, Zhaoxi Chen, Wenping Wang, Chen Change Loy, Ziwei Liu*<br>
arXir preprint, 25 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.16831)] [[Project](https://perf-project.github.io/)] [[Github](https://github.com/perf-project/PeRF)]

**ManifoldNeRF: View-dependent Image Feature Supervision for Few-shot Neural Radiance Fields**<br>
*Daiju Kanaoka, Motoharu Sonogashira, Hakaru Tamukoh, Yasutomo Kawanishi*<br>
BMVC2023, 20 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.13670)] [[Github](https://github.com/haganelego/ManifoldNeRF_BMVC2023)]

**How Many Views Are Needed to Reconstruct an Unknown Object Using NeRF?**<br>
*Sicong Pan, Liren Jin, Hao Hu, Marija Popović, Maren Bennewitz*<br>
ICRA 2024, 1 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.00684)]

**CaesarNeRF: Calibrated Semantic Representation for Few-shot Generalizable Neural Rendering**<br>
*Haidong Zhu, Tianyu Ding, Tianyi Chen, Ilya Zharkov, Ram Nevatia, Luming Liang*<br>
arXiv preprint, 27 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.15510)] [[Project](https://haidongz-usc.github.io/project/caesarnerf)]

**CorresNeRF: Image Correspondence Priors for Neural Radiance Fields**<br>
*Yixing Lao, Xiaogang Xu, Zhipeng Cai, Xihui Liu, Hengshuang Zhao*<br>
NeurIPS 2023, 11 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.06642)] [[Project](https://yxlao.github.io/corres-nerf/)] [[Code](https://github.com/yxlao/corres-nerf)]
 
**Novel View Synthesis with View-Dependent Effects from a Single Image**<br>
*Juan Luis Gonzalez Bello, Munchurl Kim*<br>
arXiv preprint, 13 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.08071)] [[Project](https://kaist-viclab.github.io/monovde-site/)]



### NeRF Based SLAM

:fire:**NICE-SLAM: Neural Implicit Scalable Encoding for SLAM**<br>
*Zihan Zhu, Songyou Peng, Viktor Larsson, Weiwei Xu, Hujun Bao, Zhaopeng Cui, Martin R. Oswald, Marc Pollefeys*<br>
CVPR 2022, 22 Dec 2021<br>
[[arXiv](https://arxiv.org/abs/2112.12130)] [[Project](https://pengsongyou.github.io/nice-slam)] [[Github](https://github.com/cvg/nice-slam)] [[Notes](./paper_discussions/NICE-SLAM.md)]

**H2-Mapping: Real-time Dense Mapping Using Hierarchical Hybrid Representation**<br>
*Chenxing Jiang, Hanwen Zhang, Peize Liu, Zehuan Yu, Hui Cheng, Boyu Zhou, Shaojie Shen*<br>
IEEE Robotics and Automation Letters,  5 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.03207)] [[Github](https://github.com/SYSU-STAR/H2-Mapping)] [[Video](https://www.bilibili.com/video/BV1Ku411Y7JU/)]

**PNeRFLoc: Visual Localization with Point-based Neural Radiance Fields**<br>
*Boming Zhao, Luwei Yang, Mao Mao, Hujun Bao, Zhaopeng Cui*<br>
AAAI 2024, 17 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.10649)]

**CaLDiff: Camera Localization in NeRF via Pose Diffusion**<br>
*Rashik Shrestha, Bishad Koju, Abhigyan Bhusal, Danda Pani Paudel, François Rameau*<br>
arXiv preprint, 23 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.15242)]

### Camera Pose Estimation & Weak Camera Pose Reconstruction

**INeRF: Inverting Neural Radiance Fields for Pose Estimation**<br>
*Lin Yen-Chen, Pete Florence, Jonathan T. Barron, Alberto Rodriguez, Phillip Isola, Tsung-Yi Lin*<br>
IROS 2021, 10 Dec 2020 <br>
[[arXiv](https://arxiv.org/abs/2012.05877)] [[Github](https://github.com/huzi96/NVFPCC/)]

:fire:**NeRF--: Neural Radiance Fields Without Known Camera Parameters**<br>
*Zirui Wang, Shangzhe Wu, Weidi Xie, Min Chen, Victor Adrian Prisacariu*<br>
arXiv preprint, 14 Feb 2021<br>
[[arXiv](https://arxiv.org/abs/2102.07064)] [[Project](https://nerfmm.active.vision)] [[Github](https://github.com/ActiveVisionLab/nerfmm)]

**iMAP: Implicit Mapping and Positioning in Real-Time**<br>
*Edgar Sucar, Shikun Liu, Joseph Ortiz, Andrew J. Davison*<br>
ICCV 2021, 23 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.12352)] [[Project](https://edgarsucar.github.io/iMAP/)]

**GNeRF: GAN-based Neural Radiance Field without Posed Camera**<br>
*Quan Meng, Anpei Chen, Haimin Luo, Minye Wu, Hao Su, Lan Xu, Xuming He, Jingyi Yu*<br>
ICCV 2021, 29 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.15606)] [[Github](https://github.com/MQ66/gnerf)]

:fire:**BARF: Bundle-Adjusting Neural Radiance Fields**<br>
*Chen-Hsuan Lin, Wei-Chiu Ma, Antonio Torralba, Simon Lucey*<br>
ICCV 2021, 13 Apr 2021<br>
[[arXiv](https://arxiv.org/abs/2104.06405)] [[Project](https://chenhsuanlin.bitbucket.io/bundle-adjusting-NeRF)] [[Github](https://github.com/chenhsuanlin/bundle-adjusting-NeRF)]

**Self-Calibrating Neural Radiance Fields**<br>
*Yoonwoo Jeong, Seokjun Ahn, Christopher Choy, Animashree Anandkumar, Minsu Cho, Jaesik Park*<br>
ICCV 2021, 13 Apr 2021<br>
[[arXiv](https://arxiv.org/abs/2108.13826)] [[Project](https://postech-cvlab.github.io/SCNeRF/)] [[Github](https://github.com/POSTECH-CVLab/SCNeRF)]

**Local-to-Global Registration for Bundle-Adjusting Neural Radiance Fields**<br>
*Yue Chen, Xingyu Chen, Xuan Wang, Qi Zhang, Yu Guo, Ying Shan, Fei Wang*<br>
CVPR 2023, 21 Nov 2022<br>
[[arXiv](https://arxiv.org/abs/2211.11505)] [[Project](https://rover-xingyu.github.io/L2G-NeRF/)] [[Github](https://github.com/rover-xingyu/L2G-NeRF)]

:fire:**NoPe-NeRF: Optimising Neural Radiance Field with No Pose Prior**<br>
*Wenjing Bian, Zirui Wang, Kejie Li, Jia-Wang Bian, Victor Adrian Prisacariu*<br>
CVPR 2023, 14 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.07388)] [[Project](https://nope-nerf.active.vision/)] [[Github](https://github.com/ActiveVisionLab/nope-nerf/)]

**Towards Open World NeRF-Based SLAM**<br>
*Daniil Lisus, Connor Holmes, Steven Waslander*<br>
CRV 2023, 8 Jan 2023<br>
[[arXiv](https://arxiv.org/abs/2301.03102)]

**F2-NeRF: Fast Neural Radiance Field Training with Free Camera Trajectories**<br>
*Peng Wang, Yuan Liu, Zhaoxi Chen, Lingjie Liu, Ziwei Liu, Taku Komura, Christian Theobalt, Wenping Wang*<br>
CVPR 2023, 28 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.15951)] [[Project](https://totoro97.github.io/projects/f2-nerf/)] [[Github](https://github.com/totoro97/f2-nerf)]

**Neural Lens Modeling**<br>
*Wenqi Xian, Aljaž Božič, Noah Snavely, Christoph Lassner*<br>
CVPR 2023, 10 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.04848)] [[Project](https://neural-lens.github.io/)]


**LU-NeRF: Scene and Pose Estimation by Synchronizing Local Unposed NeRFs**<br>
*Zezhou Cheng, Carlos Esteves, Varun Jampani, Abhishek Kar, Subhransu Maji, Ameesh Makadia*<br>
arXiv preprint, 8 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.05410)] [[Project](https://people.cs.umass.edu/~zezhoucheng/lu-nerf/)]

**CamP: Camera Preconditioning for Neural Radiance Fields**<br>
*Keunhong Park, Philipp Henzler, Ben Mildenhall, Jonathan T. Barron, Ricardo Martin-Brualla*<br>
Siggraph Asia 2023, 21 Aug, 2023<br>
[[arXiv](https://arxiv.org/abs/2308.10902)] [[Project](https://camp-nerf.github.io/)]

**MC-NeRF: Muti-Camera Neural Radiance Fields for Muti-Camera Image Acquisition Systems**<br>
*Yu Gao, Lutong Su, Hao Liang, Yufeng Yue, Yi Yang, Mengyin Fu*<br>
arXiv preprint, 14 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.07846)] [[Github](https://in2-viaun.github.io/MC-NeRF)]

**BID-NeRF: RGB-D image pose estimation with inverted Neural Radiance Fields**<br>
*Ágoston István Csehi, Csaba Máté Józsa*<br>
Nerf4ADR of ICCV 2023, 5 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.03563)]

**NeRFtrinsic Four: An End-To-End Trainable NeRF Jointly Optimizing Diverse Intrinsic and Extrinsic Camera Parameters**<br>
*Hannah Schieber, Fabian Deuser, Bernhard Egger, Norbert Oswald, Daniel Roth*<br>
arXiv preprint, 26 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2303.09412)]

**PoRF: Pose Residual Field for Accurate Neural Surface Reconstruction**<br>
*Jia-Wang Bian, Wenjing Bian, Victor Adrian Prisacariu, Philip Torr*<br>
arXiv preprint, 11 Oct 2023
[[arXiv](https://arxiv.org/abs/2310.07449)]

**CBARF: Cascaded Bundle-Adjusting Neural Radiance Fields from Imperfect Camera Poses**<br>
*Hongyu Fu, Xin Yu, Lincheng Li, Li Zhang*<br>
arXiv preprint, 15 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.09776)]

**Continuous Pose for Monocular Cameras in Neural Implicit Representation**<br>
*Qi Ma, Danda Pani Paudel, Ajad Chhatkuli, Luc Van Gool*<br>
arXiv preprint, 28 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.17119)]

**IL-NeRF: Incremental Learning for Neural Radiance Fields with Camera Pose Alignment**<br>
*Letian Zhang, Ming Li, Chen Chen, Jie Xu*<br>
arXiv preprint, 10 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.05748)]

**Unifying Correspondence, Pose and NeRF for Pose-Free Novel View Synthesis from Stereo Pairs**<br>
*Sunghwan Hong, Jaewoo Jung, Heeseong Shin, Jiaolong Yang, Seungryong Kim, Chong Luo*<br>
CVPR 2024, 12 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.07246)] [[Project](https://ku-cvlab.github.io/CoPoNeRF/)] [[Code](https://github.com/KU-CVLAB/CoPoNeRF)]

### Text to 3D

#### Survey

**Generative AI meets 3D: A Survey on Text-to-3D in AIGC Era**<br>
*Chenghao Li, Chaoning Zhang, Atish Waghwase, Lik-Hang Lee, Francois Rameau, Yang Yang, Sung-Ho Bae, Choong Seon Hong*<br>
arXiv prepring, 10 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.06131)]

#### Progresses

**Zero-Shot Text-Guided Object Generation with Dream Fields**<br>
*Ajay Jain, Ben Mildenhall, Jonathan T. Barron, Pieter Abbeel, Ben Poole*<br>
CVPR 2022, 2 Dec 2021<br>
[[arXiv](https://arxiv.org/abs/2112.01455)] [[Project](https://ajayj.com/dreamfields)] [[Github](https://github.com/google-research/google-research/tree/master/dreamfields)]

**CLIP-NeRF: Text-and-Image Driven Manipulation of Neural Radiance Fields**<br>
*Can Wang, Menglei Chai, Mingming He, Dongdong Chen, Jing Liao*<br>
CVPR 2022, 9 Dec 2021<br>
[[arXiv](https://arxiv.org/abs/2112.05139)] [[Project](https://cassiepython.github.io/clipnerf)] [[Github](https://github.com/cassiePython/CLIPNeRF)]

**LaTeRF: Label and Text Driven Object Radiance Fields**<br>
*Ashkan Mirzaei, Yash Kant, Jonathan Kelly, Igor Gilitschenski*<br>
CVPR 2022, 4 Jul 2022<br>
[[arXiv](https://arxiv.org/abs/2207.01583)] [[Project](https://tisl.cs.toronto.edu/publication/202210-eccv-laterf/)]

**DreamFusion: Text-to-3D using 2D Diffusion**<br>
*Ben Poole, Ajay Jain, Jonathan T. Barron, Ben Mildenhall*<br>
arXiv preprint, 29 Sep 2022<br>
[[arXiv](https://arxiv.org/abs/2209.14988)] [[Project](https://dreamfusion3d.github.io/)] [[Unofficial Impl](https://github.com/ashawkey/stable-dreamfusion)] [[threeStudio](https://github.com/threestudio-project/threestudio)] [[Notes](./paper_discussions/DreamFusion.md)]

**Latent-NeRF for Shape-Guided Generation of 3D Shapes and Textures**<br>
*Gal Metzer, Elad Richardson, Or Patashnik, Raja Giryes, Daniel Cohen-Or*<br>
arXiv preprint, 14 Nov 2022<br>
[[arXiv](https://arxiv.org/abs/2211.07600)] [[Github](https://github.com/eladrich/latent-nerf)] [[threeStudio](https://github.com/threestudio-project/threestudio)]

:fire:**Magic3D: High-Resolution Text-to-3D Content Creation**<br>
*Chen-Hsuan Lin, Jun Gao, Luming Tang, Towaki Takikawa, Xiaohui Zeng, Xun Huang, Karsten Kreis, Sanja Fidler, Ming-Yu Liu, Tsung-Yi Lin*<br>
CVPR 2023, 18 Nov 2022<br>
[[arXiv](https://arxiv.org/abs/2211.10440)] [[Project](https://research.nvidia.com/labs/dir/magic3d/)] [[threeStudio](https://github.com/threestudio-project/threestudio)] [[Notes](./paper_discussions/Magic3D.md)]

**Score Jacobian Chaining: Lifting Pretrained 2D Diffusion Models for 3D Generation**<br>
*Haochen Wang, Xiaodan Du, Jiahao Li, Raymond A. Yeh, Greg Shakhnarovich*<br>
CVPR 2023, 1 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.00774)] [[Project](https://pals.ttic.edu/p/score-jacobian-chaining)] [[Github](https://github.com/pals-ttic/sjc/)] [[threeStudio](https://github.com/threestudio-project/threestudio)]

**SparseFusion: Distilling View-conditioned Diffusion for 3D Reconstruction**<br>
*Zhizhuo Zhou, Shubham Tulsiani*<br>
CVPR 2023, 1 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.00792)] [[Project](https://sparsefusion.github.io/)] [[Github](https://github.com/zhizdev/sparsefusion)]

:fire:**Dream3D: Zero-Shot Text-to-3D Synthesis Using 3D Shape Prior and Text-to-Image Diffusion Models**<br>
*Jiale Xu, Xintao Wang, Weihao Cheng, Yan-Pei Cao, Ying Shan, Xiaohu Qie, Shenghua Gao*<br>
CVPR 2023, 28 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.14704)] [[Project](https://bluestyle97.github.io/dream3d/)]

**Text-To-4D Dynamic Scene Generation**<br>
*Jiale Xu, Xintao Wang, Weihao Cheng, Yan-Pei Cao, Ying Shan, Xiaohu Qie, Shenghua Gao*<br>
arXiv preprint, 26 Jan 2023<br>
[[arXiv](https://arxiv.org/abs/2301.11280)] [[Project](https://make-a-video3d.github.io/)]

:fire:**LERF: Language Embedded Radiance Fields**<br>
*Justin Kerr, Chung Min Kim, Ken Goldberg, Angjoo Kanazawa, Matthew Tancik*<br>
arXiv preprint, 16 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.09553)] [[Project](https://www.lerf.io/)] [[Github](https://github.com/kerrj/lerf)]

:fire:**Shap-E: Generating Conditional 3D Implicit Functions**<br>
*Heewoo Jun, Alex Nichol*<br>
arXiv preprint, 3 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.02463)] [[Github](https://github.com/openai/shap-e)]

:fire:**DreamBooth3D: Subject-Driven Text-to-3D Generation**<br>
*Amit Raj, Srinivas Kaza, Ben Poole, Michael Niemeyer, Nataniel Ruiz, Ben Mildenhall, Shiran Zada, Kfir Aberman, Michael Rubinstein, Jonathan Barron, Yuanzhen Li, Varun Jampani*<br>
arXiv preprint, 23 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.13508)] [[Project](https://dreambooth3d.github.io/)]

**Fantasia3D: Disentangling Geometry and Appearance for High-quality Text-to-3D Content Creation**<br>
*Rui Chen, Yongwei Chen, Ningxin Jiao, Kui Jia*<br>
arXiv preprint, 24 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.13873)] [[Project](https://fantasia3d.github.io/)] [[Github](https://github.com/Gorilla-Lab-SCUT/Fantasia3D)] [[threeStudio](https://github.com/threestudio-project/threestudio)]

**DITTO-NeRF: Diffusion-based Iterative Text To Omni-directional 3D Model**<br>
*Hoigi Seo, Hayeon Kim, Gwanghyun Kim, Se Young Chun*<br>
CVPR 2023, 6 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.02827)] [[Project](https://janeyeon.github.io/ditto-nerf/)] [[Github](https://github.com/janeyeon/ditto-nerf-code)]

:fire:**ProlificDreamer: High-Fidelity and Diverse Text-to-3D Generation with Variational Score Distillation**<br>
*Zhengyi Wang, Cheng Lu, Yikai Wang, Fan Bao, Chongxuan Li, Hang Su, Jun Zhu*<br>
arXiv preprint, 25 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.16213)] [[Project](https://ml.cs.tsinghua.edu.cn/prolificdreamer/)] [[Unofficial Implementation](https://github.com/threestudio-project/threestudio/tree/prolific-dreamer)]

**ATT3D: Amortized Text-to-3D Object Synthesis**<br>
*Jonathan Lorraine, Kevin Xie, Xiaohui Zeng, Chen-Hsuan Lin, Towaki Takikawa,Nicholas Sharp, Tsung-Yi Lin, Ming-Yu Liu, Sanja Fidler, James Lucas*<br>
nVidia release<br>
[[Project](https://research.nvidia.com/labs/toronto-ai/ATT3D/?=&linkId=100000204660845)]

**One-2-3-45: Any Single Image to 3D Mesh in 45 Seconds without Per-Shape Optimization**<br>
*Minghua Liu, Chao Xu, Haian Jin, Linghao Chen, Mukund Varma T, Zexiang Xu, Hao Su*<br>
arXiv preprint, 29 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.16928)] [[Project](http://one-2-3-45.com/)] [[Github](https://github.com/One-2-3-45/One-2-3-45)]

**Points-to-3D: Bridging the Gap between Sparse Points and Shape-Controllable Text-to-3D Generation**<br>
*Chaohui Yu, Qiang Zhou, Jingliang Li, Zhe Zhang, Zhibin Wang, Fan Wang*<br>
ACMMM 2023, 26 Jul, 2023<br>
[[arXiv](https://arxiv.org/abs/2307.13908)]

**HD-Fusion: Detailed Text-to-3D Generation Leveraging Multiple Noise Estimation**<br>
*Jinbo Wu, Xiaobo Gao, Xing Liu, Zhengyang Shen, Chen Zhao, Haocheng Feng, Jingtuo Liu, Errui Ding*<br>
arXiv preprint, 30 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.16183)]

**AvatarVerse: High-quality & Stable 3D Avatar Creation from Text and Pose**<br>
*Huichao Zhang, Bowen Chen, Hao Yang, Liao Qu, Xu Wang, Li Chen, Chao Long, Feida Zhu, Kang Du, Min Zheng*<br>
arXiv preprint, 7 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.03610)] [[Project](https://avatarverse3d.github.io/)]

**Animate124: Animating One Image to 4D Dynamic Scene**<br>
*Yuyang Zhao, Zhiwen Yan, Enze Xie, Lanqing Hong, Zhenguo Li, Gim Hee Lee*<br>
arXiv preprint, 24 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.14603)] [[Project](https://animate124.github.io/)]

**Prompt2NeRF-PIL: Fast NeRF Generation via Pretrained Implicit Latent**<br>
*Jianmeng Liu, Yuyao Zhang, Zeyuan Meng, Yu-Wing Tai, Chi-Keung Tang*<br>
arXiv preprint, 5 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02568)]

**DreamControl: Control-Based Text-to-3D Generation with 3D Self-Prior**<br>
*Tianyu Huang, Yihan Zeng, Zhilu Zhang, Wan Xu, Hang Xu, Songcen Xu, Rynson W. H. Lau, Wangmeng Zuo*<br>
CVPR 2024, 11 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.06439)] [[Code](https://github.com/tyhuang0428/DreamControl)]

**Carve3D: Improving Multi-view Reconstruction Consistency for Diffusion Models with RL Finetuning**<br>
*Desai Xie, Jiahao Li, Hao Tan, Xin Sun, Zhixin Shu, Yi Zhou, Sai Bi, Sören Pirk, Arie E. Kaufman*<br>
CVPR 2024, 21 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.13980)] [[Project](https://desaixie.github.io/carve-3d/)] [[Code](https://github.com/desaixie/carve3d)]

### Diffusion Based NeRF Reconstruction

**DiffRF: Rendering-Guided 3D Radiance Field Diffusion**<br>
*Ashkan Mirzaei, Yash Kant, Jonathan Kelly, Igor Gilitschenski*<br>
CVPR 2023, 2 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.01206)] [[Project](https://sirwyver.github.io/DiffRF/)]

:fire:**3DGen: Triplane Latent Diffusion for Textured Mesh Generation**<br>
*Anchit Gupta, Wenhan Xiong, Yixin Nie, Ian Jones, Barlas Oğuz*<br>
arXiv preprint, 9 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.05371)]

:fire:**MeshDiffusion: Score-based Generative 3D Mesh Modeling**<br>
*Zhen Liu, Yao Feng, Michael J. Black, Derek Nowrouzezahrai, Liam Paull, Weiyang Liu*<br>
ICLR 2023, 14 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.08133)] [[Project](https://meshdiffusion.github.io/)] [[Github](https://github.com/lzzcd001/MeshDiffusion/)]

**Single-Stage Diffusion NeRF: A Unified Approach to 3D Generation and Reconstruction**<br>
*Hansheng Chen, Jiatao Gu, Anpei Chen, Wei Tian, Zhuowen Tu, Lingjie Liu, Hao Su*<br>
arXiv preprint, 13 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.06714)] [[Project](https://lakonik.github.io/ssdnerf/)] [[Github](https://github.com/Lakonik/SSDNeRF)]

:fire:**Make-It-3D: High-Fidelity 3D Creation from A Single Image with Diffusion Prior**<br>
*Junshu Tang, Tengfei Wang, Bo Zhang, Ting Zhang, Ran Yi, Lizhuang Ma, Dong Chen*<br>
arXiv preprint, 23 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.14184)] [[Project](https://make-it-3d.github.io/)] [[Github](https://github.com/junshutang/Make-It-3D)] [[Notes](./paper_discussions/Make-It-3D.md)]

**Deceptive-NeRF: Enhancing NeRF Reconstruction using Pseudo-Observations from Diffusion Models**<br>
*Xinhang Liu, Shiu-hong Kao, Jiaben Chen, Yu-Wing Tai, Chi-Keung Tang*<br>
arXiv preprint, 24 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.15171)]

**ReconFusion: 3D Reconstruction with Diffusion Priors**<br>
*Rundi Wu, Ben Mildenhall, Philipp Henzler, Keunhong Park, Ruiqi Gao, Daniel Watson, Pratul P. Srinivasan, Dor Verbin, Jonathan T. Barron, Ben Poole, Aleksander Holynski*<br>
CVPR 2024, 5 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02981)] [[Project](https://reconfusion.github.io/)]

**Text-Image Conditioned Diffusion for Consistent Text-to-3D Generation**<br>
*Yuze He, Yushi Bai, Matthieu Lin, Jenny Sheng, Yubin Hu, Qi Wang, Yu-Hui Wen, Yong-Jin Liu*<br>
arXiv preprint, 19 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.11774)]

### Generalization

**Local Implicit Ray Function for Generalizable Radiance Field Representation**<br>
*Xin Huang, Qi Zhang, Ying Feng, Xiaoyu Li, Xuan Wang, Qing Wang*<br>
CVPR 2023, 25 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.12746)] [[Project](https://xhuangcv.github.io/lirf/)] [[Video](https://www.bilibili.com/video/BV1nm4y14743/)]

**MuRF: Multi-Baseline Radiance Fields**<br>
*Haofei Xu, Anpei Chen, Yuedong Chen, Christos Sakaridis, Yulun Zhang, Marc Pollefeys, Andreas Geiger, Fisher Yu*<br>
CVPR 2024, 7 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.04565)] [[Project](https://haofeixu.github.io/murf/)] [[Code](https://github.com/autonomousvision/murf)]

### Model Compression

**HollowNeRF: Pruning Hashgrid-Based NeRFs with Trainable Collision Mitigation**<br>
*Xiufeng Xie, Riccardo Gherardi, Zhihong Pan, Stephen Huang*<br>
ICCV 2023, 19 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.10122)]

### NeRF Based 2D High Quality Image Synthesis

**GIRAFFE: Representing Scenes as Compositional Generative Neural Feature Fields**<br>
*Michael Niemeyer, Andreas Geiger*<br>
CVPR 2012, 24 Nov 2020<br>
[[arXiv](https://arxiv.org/abs/2011.12100)] [[Project](http://bit.ly/giraffe-project)] [[Github](https://github.com/autonomousvision/giraffe)]

### SDF Based Reconstruction / Other Geometry Based Reconstruction

**Neural Point-Based Graphics**<br>
*Kara-Ali Aliev, Artem Sevastopolsky, Maria Kolos, Dmitry Ulyanov, Victor Lempitsky*<br>
arXiv preprint, 19 Jun 2019<br>
[[arXiv](https://arxiv.org/abs/1906.08240v3)] [[Github](https://github.com/alievk/npbg)] [[Video](https://www.youtube.com/watch?v=2uIe4iD4gSY)]

**Multiview Neural Surface Reconstruction by Disentangling Geometry and Appearance**<br>
*Lior Yariv, Yoni Kasten, Dror Moran, Meirav Galun, Matan Atzmon, Ronen Basri, Yaron Lipman*<br>
NeurIPS 2020, 22 Mar 2020<br>
[[arXiv](https://arxiv.org/abs/2003.09852)] [[Project](https://lioryariv.github.io/idr/)] [[Github](https://github.com/lioryariv/idr)]

**Neural RGB-D Surface Reconstruction**<br>
*Dejan Azinović, Ricardo Martin-Brualla, Dan B Goldman, Matthias Nießner, Justus Thies*<br>
CVPR 2022,  9 Apr 2021<br>
[[arXiv](https://arxiv.org/abs/2104.04532)] [[Project](https://dazinovic.github.io/neural-rgbd-surface-reconstruction/)] [[Github](https://github.com/dazinovic/neural-rgbd-surface-reconstruction)]

:fire:**NeuS: Learning Neural Implicit Surfaces by Volume Rendering for Multi-view Reconstruction**<br>
*Peng Wang, Lingjie Liu, Yuan Liu, Christian Theobalt, Taku Komura, Wenping Wang*<br>
NeurIPS 2021, 20 Jun 2021  <br>
[[arXiv](https://arxiv.org/abs/2106.10689)] [[Project](https://lingjie0206.github.io/papers/NeuS/)] [[Github](https://github.com/Totoro97/NeuS)]

**Volume Rendering of Neural Implicit Surfaces**<br>
*Lior Yariv, Jiatao Gu, Yoni Kasten, Yaron Lipman*<br>
NeurIPS 2021, 22 Jun 2021 <br>
[[arXiv](https://arxiv.org/abs/2106.12052)] [[Project](https://lioryariv.github.io/volsdf/)] [[Github](https://github.com/lioryariv/volsdf)]

**HF-NeuS: Improved Surface Reconstruction Using High-Frequency Details**<br>
*Yiqun Wang, Ivan Skorokhodov, Peter Wonka*<br>
NeurIPS 2022, 15 Jun 2022 <br>
[[arXiv](https://arxiv.org/abs/2206.07850)] [[Github](https://github.com/yiqun-wang/HFS)] [[Notes](./paper_discussions/HF-NeuS.md)]

**NPBG++: Accelerating Neural Point-Based Graphics**<br>
*Ruslan Rakhimov, Andrei-Timotei Ardelean, Victor Lempitsky, Evgeny Burnaev*<br>
CVPR 2022,  24 Mar 2022<br>
[[arXiv](https://arxiv.org/abs/2203.13318)] [[Project](https://rakhimovv.github.io/npbgpp/)] [[Github](https://github.com/rakhimovv/npbgpp)] 

**NeuS2: Fast Learning of Neural Implicit Surfaces for Multi-view Reconstruction**<br>
*Yiming Wang, Qin Han, Marc Habermann, Kostas Daniilidis, Christian Theobalt, Lingjie Liu*<br>
ICCV 2023, 10 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.05231)] [[Project](https://vcai.mpi-inf.mpg.de/projects/NeuS2/)] [[Github](https://github.com/19reborn/NeuS2)]

**PET-NeuS: Positional Encoding Tri-Planes for Neural Surfaces**<br>
*Yiqun Wang, Ivan Skorokhodov, Peter Wonka*<br>
CVPR 2023, 9 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.05594)] [[Github](https://github.com/yiqun-wang/PET-NeuS)]

**NeuManifold: Neural Watertight Manifold Reconstruction with Efficient and High-Quality Rendering Support**<br>
*Xinyue Wei, Fanbo Xiang, Sai Bi, Anpei Chen, Kalyan Sunkavalli, Zexiang Xu, Hao Su*<br>
arXiv preprint, 26 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.17134)] [[Project](https://sarahweiii.github.io/neumanifold/)]

**NeuRIS: Neural Reconstruction of Indoor Scenes Using Normal Priors**<br>
*Jiepeng Wang, Peng Wang, Xiaoxiao Long, Christian Theobalt, Taku Komura, Lingjie Liu, Wenping Wang*<br>
arXiv preprint, 27 Jun 2022<br>
[[arXiv](https://arxiv.org/abs/2206.13597)] [[Project](https://jiepengwang.github.io/NeuRIS/)] [[Github](https://github.com/jiepengwang/NeuRIS)]

### NeRF + Hardware Acceleration

**EventNeRF: Neural Radiance Fields from a Single Colour Event Camera**<br>
*Viktor Rudnev, Mohamed Elgharib, Christian Theobalt, Vladislav Golyanik*<br>
CVPR 2023, 23 Jun 2022  <br>
[[arXiv](https://arxiv.org/abs/2206.11896)] [[Project](https://4dqv.mpi-inf.mpg.de/EventNeRF)] [[Github](https://github.com/r00tman/EventNeRF)]

**Instant-3D: Instant Neural Radiance Field Training Towards On-Device AR/VR 3D Reconstruction**<br>
*Sixu Li, Chaojian Li, Wenbo Zhu, Boyang (Tony)Yu, Yang (Katie)Zhao, Cheng Wan, Haoran You, Huihong Shi, Yingyan (Celine)Lin*<br>
ISCA 2023, 24 Apr 2023  <br>
[[arXiv](https://arxiv.org/abs/2304.12467)]

**Robust e-NeRF: NeRF from Sparse & Noisy Events under Non-Uniform Motion**<br>
*Weng Fei Low, Gim Hee Lee*<br>
ICCV 2023, 15 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.08596)] [[Project](https://wengflow.github.io/robust-e-nerf)] [[Github](https://github.com/wengflow/robust-e-nerf)]

**Deformable Neural Radiance Fields using RGB and Event Cameras**<br>
*Qi Ma, Danda Pani Paudel, Ajad Chhatkuli, Luc Van Gool*<br>
arXiv preprint, 25 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.08416)]

**USB-NeRF: Unrolling Shutter Bundle Adjusted Neural Radiance Fields**<br>
*Moyang Li, Peng Wang, Lingzhe Zhao, Bangyan Liao, Peidong Liu*<br>
arXiv preprint, 4 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.02687)]

### NeRF + Point Cloud / LiDAR

:fire:**Point-NeRF: Point-based Neural Radiance Fields**<br>
*Qiangeng Xu, Zexiang Xu, Julien Philip, Sai Bi, Zhixin Shu, Kalyan Sunkavalli, Ulrich Neumann*<br>
CVPR 2022, 21 Jan 2022 <br>
[[arXiv](https://arxiv.org/abs/2201.08845)] [[Project](https://xharlie.github.io/projects/project_sites/pointnerf/index.html)] [[Github](https://github.com/Xharlie/pointnerf)]

**Tetra-NeRF: Representing Neural Radiance Fields Using Tetrahedra**<br>
*Qiangeng Xu, Zexiang Xu, Julien Philip, Sai Bi, Zhixin Shu, Kalyan Sunkavalli, Ulrich Neumann*<br>
arXiv preprint, 19 Apr 2023 <br>
[[arXiv](https://arxiv.org/abs/2304.09987)] [[Project](https://jkulhanek.com/tetra-nerf/)] [[Github](https://github.com/jkulhanek/tetra-nerf/)] [[Notes](./paper_discussions/Tetra-NeRF.md)]

**Neural LiDAR Fields for Novel View Synthesis**<br>
*Shengyu Huang, Zan Gojcic, Zian Wang, Francis Williams, Yoni Kasten, Sanja Fidler, Konrad Schindler, Or Litany*<br>
arXiv preprint, 2 May 2023 <br>
[[arXiv](https://arxiv.org/abs/2305.01643)] [[Project](https://research.nvidia.com/labs/toronto-ai/nfl/)] [[Notes](./paper_discussions/NFL.md)]

**Point2Pix: Photo-Realistic Point Cloud Rendering via Neural Radiance Fields**<br>
*Tao Hu, Xiaogang Xu, Shu Liu, Jiaya Jia*<br>
arXiv preprint, 29 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.16482)] [[Video](https://www.bilibili.com/video/BV1hh4y1s7LT/)]

### NeRF + Auto Data Collection

**AutoNeRF: Training Implicit Scene Representations with Autonomous Agents**<br>
*Pierre Marza, Laetitia Matignon, Olivier Simonin, Dhruv Batra, Christian Wolf, Devendra Singh Chaplot*<br>
arXiv preprint, 21 Apr 2023 <br>
[[arXiv](https://arxiv.org/abs/2304.11241)] [[Project](https://pierremarza.github.io/projects/autonerf/)] [[Video](https://www.bilibili.com/video/BV1iX4y1m7op/)]

**NerfBridge: Bringing Real-time, Online Neural Radiance Field Training to Robotics**<br>
*Javier Yu, Jun En Low, Keiko Nagami, Mac Schwager*<br>
ICRA 2023, 16 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.09761)] [[Github](https://github.com/javieryu/nerf_bridge)] [[Video](https://www.bilibili.com/video/BV1Bg4y1F7gD/)]


### NeRF + Avatar/Talking Head

:fire:**AD-NeRF: Audio Driven Neural Radiance Fields for Talking Head Synthesis**<br>
*Yudong Guo, Keyu Chen, Sen Liang, Yong-Jin Liu, Hujun Bao, Juyong Zhang*<br>
ICCV 2021, 20 Mar 2021 <br>
[[arXiv](https://arxiv.org/abs/2103.11078)] [[Project](https://yudongguo.github.io/ADNeRF/)] [[Github](https://github.com/YudongGuo/AD-NeRF/)]

**MoFaNeRF: Morphable Facial Neural Radiance Field**<br>
*Yiyu Zhuang, Hao Zhu, Xusen Sun, Xun Cao*<br>
ECCV 2022, 4 Dec 2021 <br>
[[arXiv](https://arxiv.org/abs/2112.02308)] [[Project](https://yiyuzhuang.github.io/mofanerf/)] [[Github](https://github.com/zhuhao-nju/mofanerf)] [[Video](https://www.bilibili.com/video/BV1GM41167Vo/)]

**AutoAvatar: Autoregressive Neural Fields for Dynamic Avatar Modeling**<br>
*Ziqian Bai, Timur Bagautdinov, Javier Romero, Michael Zollhöfer, Ping Tan, Shunsuke Saito*<br>
ECCV 2022, 25 Mar 2022 <br>
[[arXiv](https://arxiv.org/abs/2203.13817)] [[Project](https://zqbai-jeremy.github.io/autoavatar/)] [[Github](https://github.com/facebookresearch/AutoAvatar)] [[Video](https://www.bilibili.com/video/BV1FW4y1u7xX/)]

**UV Volumes for Real-time Rendering of Editable Free-view Human Performance**<br>
*Yue Chen, Xuan Wang, Xingyu Chen, Qi Zhang, Xiaoyu Li, Yu Guo, Jue Wang, Fei Wang*<br>
CVPR 2023, 27 Mar 2022<br>
[[arXiv](https://arxiv.org/abs/2203.14402)] [[Project](https://fanegg.github.io/UV-Volumes/)] [[Github](https://github.com/fanegg/UV-Volumes)]

**Learning Dynamic Facial Radiance Fields for Few-Shot Talking Head Synthesis**<br>
*Shuai Shen, Wanhua Li, Zheng Zhu, Yueqi Duan, Jie Zhou, Jiwen Lu*<br>
ECCV 2022, 24 Jul 2022 <br>
[[arXiv](https://arxiv.org/abs/2207.11770)] [[Project](https://sstzal.github.io/DFRF/)] [[Github](https://github.com/sstzal/DFRF)] [[Video](https://www.bilibili.com/video/BV1TW4y1g7HB/)]

**EVA3D: Compositional 3D Human Generation from 2D Image Collections**<br>
*Fangzhou Hong, Zhaoxi Chen, Yushi Lan, Liang Pan, Ziwei Liu*<br>
ICLR 2023, 10 Oct 2022 <br>
[[arXiv](https://arxiv.org/abs/2210.04888)] [[Project](https://hongfz16.github.io/projects/EVA3D.html)] [[Github](https://github.com/hongfz16/EVA3D)] [[Video](https://www.bilibili.com/video/BV1GT411U7kk/)]

:fire:**Rodin: A Generative Model for Sculpting 3D Digital Avatars Using Diffusion**<br>
*Tengfei Wang, Bo Zhang, Ting Zhang, Shuyang Gu, Jianmin Bao, Tadas Baltrusaitis, Jingjing Shen, Dong Chen, Fang Wen, Qifeng Chen, Baining Guo*<br>
arXiv preprint, 12 Dec 2022 <br>
[[arXiv](https://arxiv.org/abs/2212.06135)] [[Project](https://3d-avatar-diffusion.microsoft.com/)] [[Video](https://www.bilibili.com/video/BV1m44y1Z7gr/)]

**InstantAvatar: Learning Avatars from Monocular Video in 60 Seconds**<br>
*Tianjian Jiang, Xu Chen, Jie Song, Otmar Hilliges*<br>
arXiv preprint, 20 Dec 2022 <br>
[[arXiv](https://arxiv.org/abs/2212.10550)] [[Project](https://tijiang13.github.io/InstantAvatar/)] [[Github](https://github.com/tijiang13/InstantAvatar)] [[Video](https://www.bilibili.com/video/BV1j84y1s7ZF/)]

**PersonNeRF: Personalized Reconstruction from Photo Collections**<br>
*Chung-Yi Weng, Pratul P. Srinivasan, Brian Curless, Ira Kemelmacher-Shlizerman*<br>
arXiv preprint, 16 Feb 2023 <br>
[[arXiv](https://arxiv.org/abs/2302.08504)] [[Project](https://grail.cs.washington.edu/projects/personnerf/)] [[Video](https://www.bilibili.com/video/BV1Vg4y1W7yJ/)]

**Learning Neural Volumetric Representations of Dynamic Humans in Minutes**<br>
*Chen Geng, Sida Peng, Zhen Xu, Hujun Bao, Xiaowei Zhou*<br>
CVPR 2023, 23 Feb 2023 <br>
[[arXiv](https://arxiv.org/abs/2302.12237)] [[Project](https://zju3dv.github.io/instant_nvr/)] [[Video](https://www.bilibili.com/video/BV1Rs4y1j7DW/)]

**NeuFace: Realistic 3D Neural Face Rendering from Multi-view Images**<br>
*Mingwu Zheng, Haiyu Zhang, Hongyu Yang, Di Huang*<br>
CVPR 2023, 24 Mar 2023 <br>
[[arXiv](https://arxiv.org/abs/2303.14092)] [[Github](https://github.com/aejion/NeuFace)] [[Notes](./paper_discussions/NeuFace.md)]

:fire:**HumanRF: High-Fidelity Neural Radiance Fields for Humans in Motion**<br>
*Mustafa Işık, Martin Rünz, Markos Georgopoulos, Taras Khakhulin, Jonathan Starck, Lourdes Agapito, Matthias Nießner*<br>
SIGGRAPH 2023, 10 May 2023 <br>
[[arXiv](https://arxiv.org/abs/2305.06356)] [[Project](https://synthesiaresearch.github.io/humanrf/)] [[Github](https://github.com/synthesiaresearch/humanrf)] [[Video](https://www.bilibili.com/video/BV1ug4y1V7cy/)] [[Notes](./paper_discussions/HumanRF.md)]

**BlendFields: Few-Shot Example-Driven Facial Modeling**<br>
*Kacper Kania, Stephan J. Garbin, Andrea Tagliasacchi, Virginia Estellers, Kwang Moo Yi, Julien Valentin, Tomasz Trzciński, Marek Kowalski*<br>
arXiv preprint, 12 May 2023 <br>
[[arXiv](https://arxiv.org/abs/2305.07514)] [[Project](https://blendfields.github.io/)] [[Video](https://www.bilibili.com/video/BV1xs4y1M7dZ/)] 

**Neural Face Rigging for Animating and Retargeting Facial Meshes in the Wild**<br>
*Dafei Qin, Jun Saito, Noam Aigerman, Thibault Groueix, Taku Komura*<br>
arXiv preprint, 15 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.08296)]

**NCHO: Unsupervised Learning for Neural 3D Composition of Humans and Objects**<br>
*Taeksoo Kim, Shunsuke Saito, Hanbyul Joo*<br>
arXiv preprint, 23 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.14345)] [[Project](https://taeksuu.github.io/ncho/)]

**FDNeRF: Semantics-Driven Face Reconstruction, Prompt Editing and Relighting with Diffusion Models**<br>
*Hao Zhang, Yanbo Xu, Tianyuan Dai, Yu-Wing, Tai Chi-Keung Tang*<br>
arXiv preprint, 1 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.00783)] [[Github](https://github.com/BillyXYB/FDNeRF)]

**PixelHuman: Animatable Neural Radiance Fields from Few Images**<br>
*Gyumin Shim, Jaeseong Lee, Junha Hyung, Jaegul Choo*<br>
arXiv preprint, 18 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.09070)]

**Efficient Region-Aware Neural Radiance Fields for High-Fidelity Talking Portrait Synthesis**<br>
*Jiahe Li, Jiawei Zhang, Xiao Bai, Jun Zhou, Lin Gu*<br>
ICCV 2023, 18 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.09323)] [[Github](https://github.com/fictionarry/er-nerf)]

**FaceCLIPNeRF: Text-driven 3D Face Manipulation using Deformable Neural Radiance Fields**<br>
*Sungwon Hwang, Junha Hyung, Daejin Kim, Min-Jung Kim, Jaegul Choo*<br>
ICCV 2023, 21 July, 2023<br>
[[arXiv](https://arxiv.org/abs/2307.11418)]

**TransHuman: A Transformer-based Human Representation for Generalizable Neural Human Rendering**<br>
*Xiao Pan, Zongxin Yang, Jianxin Ma, Chang Zhou, Yi Yang*<br>
ICCV 2023, 23 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.12291)] [[Project](https://pansanity666.github.io/TransHuman/)]

**HAvatar: High-fidelity Head Avatar via Facial Model Conditioned Neural Radiance Field**<br>
*Xiaochen Zhao, Lizhen Wang, Jingxiang Sun, Hongwen Zhang, Jinli Suo, Yebin Liu*<br>
arXiv preprint, 29 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.17128)]

**Point-Based Radiance Fields for Controllable Human Motion Synthesis**<br>
*Haitao Yu, Deheng Zhang, Peiyuan Xie, Tianyi Zhang*<br>
arXiv preprint, 5 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.03375)]

**DynVideo-E: Harnessing Dynamic NeRF for Large-Scale Motion- and View-Change Human-Centric Video Editing**<br>
*Jia-Wei Liu, Yan-Pei Cao, Jay Zhangjie Wu, Weijia Mao, Yuchao Gu, Rui Zhao, Jussi Keppo, Ying Shan, Mike Zheng Shou*<br>
arXiv preprint, 16 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.10624)] [[Project](https://showlab.github.io/DynVideo-E/)]

**CosAvatar: Consistent and Animatable Portrait Video Tuning with Text Prompt**<br>
*Haiyao Xiao, Chenglai Zhong, Xuan Gao, Yudong Guo, Juyong Zhang*<br>
arXiv preprint, 30 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.18288)] [[Project](https://ustc3dv.github.io/CosAvatar/)]

**Artist-Friendly Relightable and Animatable Neural Heads**<br>
*Yingyan Xu, Prashanth Chandran, Sebastian Weiss, Markus Gross, Gaspard Zoss, Derek Bradley*<br>
arXiv preprint, 6 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.03420)]

**FaceStudio: Put Your Face Everywhere in Seconds**<br>
*Yuxuan Yan, Chi Zhang, Rui Wang, Yichao Zhou, Gege Zhang, Pei Cheng, Gang Yu, Bin Fu*<br>
arXiv preprint, 6 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02663)] [[Project](https://icoz69.github.io/facestudio/)] [[code](https://github.com/TencentQQGYLab/FaceStudio)]

**Identity-Obscured Neural Radiance Fields: Privacy-Preserving 3D Facial Reconstruction**<br>
*Jiayi Kong, Baixin Xu, Xurui Song, Chen Qian, Jun Luo, Ying He*<br>
arXiv preprint, 7 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.04106)]

**TriHuman : A Real-time and Controllable Tri-plane Representation for Detailed Human Geometry and Appearance Synthesis**<br>
*Heming Zhu, Fangneng Zhan, Christian Theobalt, Marc Habermann*<br>
arXiv preprint, 8 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.05161)]

**R2-Talker: Realistic Real-Time Talking Head Synthesis with Hash Grid Landmarks Encoding and Progressive Multilayer Conditioning**<br>
*Zhiling Ye, LiangGuo Zhang, Dingheng Zeng, Quan Lu, Ning Jiang*<br>
arXiv preprint, 9 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.05572)]

**SIFU: Side-view Conditioned Implicit Function for Real-world Usable Clothed Human Reconstruction**<br>
*Zechuan Zhang, Zongxin Yang, Yi Yang*<br>
CVPR 2024, 10 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.06704)] [[Project](https://river-zhang.github.io/SIFU-projectpage/)] [[Code](https://github.com/River-Zhang/SIFU)]

### NeRF + Imaging Tasks

:fire:**NeRF in the Dark: High Dynamic Range View Synthesis from Noisy Raw Images**<br>
*Ben Mildenhall, Peter Hedman, Ricardo Martin-Brualla, Pratul Srinivasan, Jonathan T. Barron*<br>
CVPR 2022, 26 Nov 2021 <br>
[[arXiv](https://arxiv.org/abs/2111.13679)] [[Project](https://bmild.github.io/rawnerf/)] [[Github](https://github.com/google-research/multinerf)]

**Deblur-NeRF: Neural Radiance Fields from Blurry Images**<br>
*Li Ma, Xiaoyu Li, Jing Liao, Qi Zhang, Xuan Wang, Jue Wang, Pedro V. Sander*<br>
CVPR 2022, 29 Nov 2021 <br>
[[arXiv](https://arxiv.org/abs/2111.14292)] [[Project](https://limacv.github.io/deblurnerf/)] [[Github](https://github.com/limacv/Deblur-NeRF)]

**HDR-NeRF: High Dynamic Range Neural Radiance Fields**<br>
*Xin Huang, Qi Zhang, Ying Feng, Hongdong Li, Xuan Wang, Qing Wang*<br>
CVPR 2022, 29 Nov 2021 <br>
[[arXiv](https://arxiv.org/abs/2111.14451)] [[Project](https://xhuangcv.github.io/hdr-nerf/)] [[Github](https://github.com/xhuangcv/hdr-nerf/)]

**NeRF-SR: High-Quality Neural Radiance Fields using Supersampling**<br>
*Chen Wang, Xian Wu, Yuan-Chen Guo, Song-Hai Zhang, Yu-Wing Tai, Shi-Min Hu*<br>
MM 2022, 3 Dec 2021 <br>
[[arXiv](https://arxiv.org/abs/2112.01759)] [[Project](https://cwchenwang.github.io/NeRF-SR/)] [[Github](https://github.com/cwchenwang/NeRF-SR)]

**Aleth-NeRF: Low-light Condition View Synthesis with Concealing Fields**<br>
*Ziteng Cui, Lin Gu, Xiao Sun, Yu Qiao, Tatsuya Harada*<br>
arXiv preprint, 10 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.05807)] [[Project](https://cuiziteng.github.io/Aleth_NeRF_web/)] [[Github](https://github.com/cuiziteng/Aleth-NeRF)]

**Lighting up NeRF via Unsupervised Decomposition and Enhancement**<br>
**Haoyuan Wang, Xiaogang Xu, Ke Xu, Rynson WH. Lau*<br>
ICCV 2023, 20 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.10664)] [[Project](https://whyy.site/paper/llnerf)] [[Github](https://github.com/onpix/LLNeRF)]

### NeRF + Large Scale Scenes & Urban Scenes

:fire:**Urban Radiance Fields**<br>
*Konstantinos Rematas, Andrew Liu, Pratul P. Srinivasan, Jonathan T. Barron, Andrea Tagliasacchi, Thomas Funkhouser, Vittorio Ferrari*<br>
CVPR 2022, 29 Nov 2021 <br>
[[arXiv](https://arxiv.org/abs/2111.14643)] [[Project](https://urban-radiance-fields.github.io/)]

**Hallucinated Neural Radiance Fields in the Wild**<br>
*Xingyu Chen, Qi Zhang, Xiaoyu Li, Yue Chen, Ying Feng, Xuan Wang, Jue Wang*<br>
CVPR 2022, 30 Nov 2021 <br>
[[arXiv](https://arxiv.org/abs/2111.15246)] [[Project](https://rover-xingyu.github.io/Ha-NeRF/)] [[Github](https://github.com/rover-xingyu/Ha-NeRF)]

**NeRF for Outdoor Scene Relighting**<br>
*Viktor Rudnev, Mohamed Elgharib, William Smith, Lingjie Liu, Vladislav Golyanik, Christian Theobalt*<br>
ECCV 2022, 9 Dec 2021 <br>
[[arXiv](https://arxiv.org/abs/2112.05140)] [[Project](https://4dqv.mpi-inf.mpg.de/NeRF-OSR/)] [[Github](https://github.com/r00tman/NeRF-OSR)]

**BungeeNeRF: Progressive Neural Radiance Field for Extreme Multi-scale Scene Rendering**<br>
*Viktor Rudnev, Mohamed Elgharib, William Smith, Lingjie Liu, Vladislav Golyanik, Christian Theobalt*<br>
ECCV 2022, 10 Dec 2021 <br>
[[arXiv](https://arxiv.org/abs/2112.05504)] [[Project](https://city-super.github.io/citynerf/)] [[Github](https://github.com/city-super/BungeeNeRF)]

:fire:**Mega-NeRF: Scalable Construction of Large-Scale NeRFs for Virtual Fly-Throughs**<br>
*Haithem Turki, Deva Ramanan, Mahadev Satyanarayanan*<br>
CVPR 2022, 20 Dec 2021 <br>
[[arXiv](https://arxiv.org/abs/2112.10703)] [[Project](https://meganerf.cmusatyalab.org/)] [[Github](https://github.com/cmusatyalab/mega-nerf)]

:fire:**Block-NeRF: Scalable Large Scene Neural View Synthesis**<br>
*Matthew Tancik, Vincent Casser, Xinchen Yan, Sabeek Pradhan, Ben Mildenhall, Pratul P. Srinivasan, Jonathan T. Barron, Henrik Kretzschmar*<br>
CVPR 2022, 10 Feb 2022 <br>
[[arXiv](https://arxiv.org/abs/2202.05263)] [[Project](https://waymo.com/intl/zh-cn/research/block-nerf/)]

**DisCoScene: Spatially Disentangled Generative Radiance Fields for Controllable 3D-aware Scene Synthesis**<br>
*Yinghao Xu, Menglei Chai, Zifan Shi, Sida Peng, Ivan Skorokhodov, Aliaksandr Siarohin, Ceyuan Yang, Yujun Shen, Hsin-Ying Lee, Bolei Zhou, Sergey Tulyakov*<br>
arXiv preprint, 22 Dec 2022 <br>
[[arXiv](https://arxiv.org/abs/2212.11984)] [[Prject](https://snap-research.github.io/discoscene/)] [[Github](https://github.com/snap-research/discoscene)] [[Video](https://www.bilibili.com/video/BV11G4y1f7DF/)]

**S-NeRF: Neural Radiance Fields for Street Views**<br>
*Ziyang Xie, Junge Zhang, Wenye Li, Feihu Zhang, Li Zhang*<br>
ICLR 2023, 1 Mar 2023 <br>
[[arXiv](https://arxiv.org/abs/2303.00749)] [[Prject](https://ziyang-xie.github.io/s-nerf/)] [[Video](https://www.bilibili.com/video/BV1No4y1k7iR/)]

**Progressively Optimized Local Radiance Fields for Robust View Synthesis**<br>
*Andreas Meuleman, Yu-Lun Liu, Chen Gao, Jia-Bin Huang, Changil Kim, Min H. Kim, Johannes Kopf*<br>
CVPR 2023, 24 Mar 2023 <br>
[[arXiv](https://arxiv.org/abs/2303.13791)] [[Prject](https://localrf.github.io/)] [[Video](https://www.bilibili.com/video/BV12c411V7Dz/)]

**SUDS: Scalable Urban Dynamic Scenes**<br>
*Haithem Turki, Jason Y. Zhang, Francesco Ferroni, Deva Ramanan*<br>
CVPR 2023, 25 Mar 2023 <br>
[[arXiv](https://arxiv.org/abs/2303.14536)] [[Prject](https://haithemturki.com/suds/)] [[Github](https://github.com/hturki/suds)] [[Video](https://www.bilibili.com/video/BV1xj411w7XE/)]

**Neural Fields meet Explicit Geometric Representations for Inverse Rendering of Urban Scenes**<br>
*Zian Wang, Tianchang Shen, Jun Gao, Shengyu Huang, Jacob Munkberg, Jon Hasselgren, Zan Gojcic, Wenzheng Chen, Sanja Fidler*<br>
CVPR 2023, 6 Apr 2023 <br>
[[arXiv](https://arxiv.org/abs/2304.03266)] [[Prject](https://nv-tlabs.github.io/fegr/)] [[Video](https://www.bilibili.com/video/BV1kh411M7rd/)]

**NeuralField-LDM: Scene Generation with Hierarchical Latent Diffusion Models**<br>
*Seung Wook Kim, Bradley Brown, Kangxue Yin, Karsten Kreis, Katja Schwarz, Daiqing Li, Robin Rombach, Antonio Torralba, Sanja Fidler*<br>
CVPR 2023, 19 Apr 2023 <br>
[[arXiv](https://arxiv.org/abs/2304.09787)] [[Prject](https://research.nvidia.com/labs/toronto-ai/NFLDM/)] [[Video](https://www.bilibili.com/video/BV1FP411D7D5/)]

**PlaNeRF: SVD Unsupervised 3D Plane Regularization for NeRF Large-Scale Scene Reconstruction**<br>
*Fusang Wang, Arnaud Louys, Nathan Piasco, Moussab Bennehar, Luis Roldão, Dzmitry Tsishkou*<br>
arXiv preprint, 26 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.16914)]

**Urban Radiance Field Representation with Deformable Neural Mesh Primitives**<br>
*Fan Lu, Yan Xu, Guang Chen, Hongsheng Li, Kwan-Yee Lin, Changjun Jiang*<br>
ICCV 2023, 20 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.10776)] [[Project](https://dnmp.github.io/)] [[Github](https://github.com/DNMP/DNMP)]

**Federated Learning for Large-Scale Scene Modeling with Neural Radiance Fields**<br>
*Teppei Suzuki*<br>
arXiv preprint, 12 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.06030)]

**UE4-NeRF:Neural Radiance Field for Real-Time Rendering of Large-Scale Scene**<br>
*Jiaming Gu, Minchao Jiang, Hongsheng Li, Xiaoyuan Lu, Guangming Zhu, Syed Afaq Ali Shah, Liang Zhang, Mohammed Bennamoun*<br>
NeurIPS 2023, 20 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.13263)] [[Project](https://jamchaos.github.io/UE4-NeRF/)] [[Github](https://github.com/JamChaos/UE4-NeRF)]

**PanopticNeRF-360: Panoramic 3D-to-2D Label Transfer in Urban Scenes**<br>
*Xiao Fu, Shangzhan Zhang, Tianrun Chen, Yichong Lu, Xiaowei Zhou, Andreas Geiger, Yiyi Liao*<br>
arXiv preprint, 19 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.10815)] [[Project](https://fuxiao0719.github.io/projects/panopticnerf360/)] [[Github](https://github.com/fuxiao0719/PanopticNeRF)]

**MMPI: a Flexible Radiance Field Representation by Multiple Multi-plane Images Blending**<br>
*Yuze He, Peng Wang, Yubin Hu, Wang Zhao, Ran Yi, Yong-Jin Liu, Wenping Wang*<br>
arXiv preprint, 30 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2310.00249)]


**SCALAR-NeRF: SCAlable LARge-scale Neural Radiance Fields for Scene Reconstruction**<br>
*Yu Chen, Gim Hee Lee*<br>
arXiv preprint, 28 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16657)] [[Project](https://aibluefisher.github.io/SCALAR-NeRF/)]

**EvE: Exploiting Generative Priors for Radiance Field Enrichment**<br>
*Karim Kassab, Antoine Schnepf, Jean-Yves Franceschi, Laurent Caraffa, Jeremie Mary, Valérie Gouet-Brunet*<br>
arXiv preprint, 1 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.00639)] [[Project](https://eve-nvs.github.io/)]

**LightSim: Neural Lighting Simulation for Urban Scenes**<br>
*Ava Pun, Gary Sun, Jingkang Wang, Yun Chen, Ze Yang, Sivabalan Manivasagam, Wei-Chiu Ma, Raquel Urtasun*<br>
NeurIPS 2023, 11 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.06654)] [[Project](https://waabi.ai/lightsim/)]


**SMERF: Streamable Memory Efficient Radiance Fields for Real-Time Large-Scene Exploration**<br>
*Daniel Duckworth, Peter Hedman, Christian Reiser, Peter Zhizhin, Jean-François Thibert, Mario Lučić, Richard Szeliski, Jonathan T. Barron*<br>
arXir preprint, 12 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.07541)] [[Project](https://smerf-3d.github.io/)] [[Video](https://www.youtube.com/watch?v=zhO8iUBpnCc&feature=youtu.be)]

**City-on-Web: Real-time Neural Rendering of Large-scale Scenes on the Web**<br>
*Kaiwen Song, Juyong Zhang*<br>
arXiv preprint, 27 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.16457)] [[Project](https://ustc3dv.github.io/City-on-Web/)]


### NeRF + Autonomous Driving

**READ: Large-Scale Neural Scene Rendering for Autonomous Driving**<br>
*Zhuopeng Li, Lu Li, Zeyu Ma, Ping Zhang, Junbo Chen, Jianke Zhu*<br>
AAAI 2023, 11 May 2022 <br>
[[arXiv](https://arxiv.org/abs/2205.05509)] [[Github](https://github.com/JOP-Lee/READ)] [[Video](https://www.bilibili.com/video/BV1124y1Q781/)]

**PC-NeRF: Parent-Child Neural Radiance Fields under Partial Sensor Data Loss in Autonomous Driving Environments**<br>
*Xiuzhong Hu, Guangming Xiong, Zheng Zang, Peng Jia, Yuxuan Han, Junyi Ma*<br>
arXiv preprint, 2 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.00874)] [[Github](https://github.com/biter0088/pc-nerf)]

**UC-NeRF: Neural Radiance Field for Under-Calibrated multi-view cameras in autonomous driving**<br>
*Kai Cheng, Xiaoxiao Long, Wei Yin, Jin Wang, Zhiqiang Wu, Yuexin Ma, Kaixuan Wang, Xiaozhi Chen, Xuejin Chen*<br>
arXiv preprint, 28 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16945)] [[Project](https://kcheng1021.github.io/ucnerf.github.io/)]

**DGNR: Density-Guided Neural Point Rendering of Large Driving Scenes**<br>
*Zhuopeng Li, Chenming Wu, Liangjun Zhang, Jianke Zhu*<br>
arXiv preprint, 28 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16664)]

**Dynamic LiDAR Re-simulation using Compositional Neural Fields**<br>
*Hanfeng Wu, Xingxing Zuo, Stefan Leutenegger, Or Litany, Konrad Schindler, Shengyu Huang*<br>
CVPR 2024, 8 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.05247)] [[Project](https://shengyuh.github.io/dynfl/)] [[Code](https://github.com/prs-eth/Dynamic-LiDAR-Resimulation)] [[Video](https://shengyuh.github.io/dynfl/assets/Main_videos.m4v)]

### NeRF + Editing

**Recolorable Posterization of Volumetric Radiance Fields Using Visibility-Weighted Palette Extraction**<br>
*Seung Wook Kim, Bradley Brown, Kangxue Yin, Karsten Kreis, Katja Schwarz, Daiqing Li, Robin Rombach, Antonio Torralba, Sanja Fidler*<br>
CVPR 2023, 19 Apr 2022 <br>
[[Paper](https://drive.google.com/file/d/1HjAVDBiainhDAEejmDPH8WrvRxk-Fbtw/view?usp=sharing)] [[Project](https://kenji-tojo.github.io/publications/posternerf/)] [[Github](https://github.com/kenji-tojo/posternerf)]

**ClimateNeRF: Physically-based Neural Rendering for Extreme Climate Synthesis**<br>
*Yuan Li, Zhi-Hao Lin, David Forsyth, Jia-Bin Huang, Shenlong Wang*<br>
CVPR 2023, 19 Apr 2022 <br>
[[arXiv](https://arxiv.org/abs/2211.13226)] [[Project](https://climatenerf.github.io/)] [[Video](https://www.bilibili.com/video/BV1B8411J7vV/)]

**NeuMesh: Learning Disentangled Neural Mesh-based Implicit Field for Geometry and Texture Editing**<br>
*Bangbang Yang, Chong Bao, Junyi Zeng, Hujun Bao, Yinda Zhang, Zhaopeng Cui, Guofeng Zhang*<br>
CVPR 2022, 25 Jul 2022<br>
[[arXiv](https://arxiv.org/abs/2207.11911)] [[Project](https://zju3dv.github.io/neumesh/)] [[Github](https://github.com/zju3dv/neumesh)]

:fire:**SPIn-NeRF: Multiview Segmentation and Perceptual Inpainting with Neural Radiance Fields**<br>
*Ashkan Mirzaei, Tristan Aumentado-Armstrong, Konstantinos G. Derpanis, Jonathan Kelly, Marcus A. Brubaker, Igor Gilitschenski, Alex Levinshtein*<br>
CVPR 2023, 22 Nov 2022 <br>
[[arXiv](https://arxiv.org/abs/2211.12254)] [[Project](https://spinnerf3d.github.io/)] [[Github](https://github.com/SamsungLabs/SPIn-NeRF)] [[Video](https://www.bilibili.com/video/BV1Fm4y127TW/)] [[Notes](./paper_discussions/SPIn-NeRF.md)]

**NeRF-Art: Text-Driven Neural Radiance Fields Stylization**<br>
*Can Wang, Ruixiang Jiang, Menglei Chai, Mingming He, Dongdong Chen, Jing Liao*<br>
arXiv preprint, 15 Dec 2022 <br>
[[arXiv](https://arxiv.org/abs/2212.08070)] [[Project](https://cassiepython.github.io/nerfart/)] [[Github](https://github.com/cassiePython/NeRF-Art)] [[Video](https://www.bilibili.com/video/BV1b44y1Z7U3/)]

**PaletteNeRF: Palette-based Appearance Editing of Neural Radiance Fields**<br>
*Zhengfei Kuang, Fujun Luan, Sai Bi, Zhixin Shu, Gordon Wetzstein, Kalyan Sunkavalli*<br>
arXiv preprint, 21 Dec 2022 <br>
[[arXiv](https://arxiv.org/abs/2212.10699)] [[Project](https://palettenerf.github.io/)] [[Github](https://github.com/zfkuang/PaletteNeRF)] [[Video](https://www.bilibili.com/video/BV1Fv4y1B7De/)]

**RecolorNeRF: Layer Decomposed Radiance Fields for Efficient Color Editing of 3D Scenes**<br>
*Bingchen Gong, Yuehao Wang, Xiaoguang Han, Qi Dou*<br>
arXiv preprint, 19 Jan 2023 <br>
[[arXiv](https://arxiv.org/abs/2301.07958)] [[Project](https://sites.google.com/view/recolornerf)] [[Github](https://github.com/yuehaowang/RecolorNeRF)] [[Video](https://www.bilibili.com/video/BV1qT411X7Y6/)]

:fire:**Interactive Geometry Editing of Neural Radiance Fields**<br>
*Shaoxu Li, Ye Pan*<br>
I3D 2023, 21 Mar 2023 <br>
[[arXiv](https://arxiv.org/abs/2303.11537)] [[Project](https://repo-sam.inria.fr/fungraph/nerfshop/)] [[Github](https://github.com/graphdeco-inria/nerfshop)] [[Video](https://www.bilibili.com/video/BV1qk4y1b7L4/)] [[Notes](./paper_discussions/NeRFShop.md)]

:fire:**Instruct-NeRF2NeRF: Editing 3D Scenes with Instructions**<br>
*Ayaan Haque, Matthew Tancik, Alexei A. Efros, Aleksander Holynski, Angjoo Kanazawa*<br>
arXiv preprint, 22 Mar 2023 <br>
[[arXiv](https://arxiv.org/abs/2303.12789)] [[Project](https://instruct-nerf2nerf.github.io/)] [[Github](https://github.com/ayaanzhaque/instruct-nerf2nerf)] [[Video](https://www.bilibili.com/video/BV1rb411o7gR/)]

**SINE: Semantic-driven Image-based NeRF Editing with Prior-guided Editing Field**<br>
*Chong Bao, Yinda Zhang, Bangbang Yang, Tianxing Fan, Zesong Yang, Hujun Bao, Guofeng Zhang, Zhaopeng Cui*<br>
CVPR 2023, 23 Mar 2023  <br>
[[arXiv](https://arxiv.org/abs/2303.13277)] [[Project](https://zju3dv.github.io/sine/)] [[Video](https://www.bilibili.com/video/BV1d84y1u7V2/)]

**PartNeRF: Generating Part-Aware Editable 3D Shapes without 3D Supervision**<br>
*Konstantinos Tertikas, Despoina Paschalidou, Boxiao Pan, Jeong Joon Park, Mikaela Angelina Uy, Ioannis Emiris, Yannis Avrithis, Leonidas Guibas*<br>
CVPR 2023, 16 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.09554)] [[Project](https://ktertikas.github.io/part_nerf)] [[Github](https://github.com/ktertikas/part_nerf)]

**InpaintNeRF360: Text-Guided 3D Inpainting on Unbounded Neural Radiance Fields**<br>
*Dongqing Wang, Tong Zhang, Alaa Abboud, Sabine Süsstrunk*<br>
arXiv preprint, 24 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.15094)]

**FusedRF: Fusing Multiple Radiance Fields**<br>
*Rahul Goel, Dhawal Sirikonda, Rajvi Shah, PJ Narayanan*<br>
CVPR Workshop,  7 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.04180)]

**RePaint-NeRF: NeRF Editting via Semantic Masks and Diffusion Models**<br>
*Xingchen Zhou, Ying He, F. Richard Yu, Jianqiang Li, You Li*<br>
IJCAI 2023, 9 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.05668)] [[Github](https://repaintnerf.github.io/)]

**Relighting Neural Radiance Fields With Shadow and Highlight Hints**<br>
*Chong Zeng, Guojun Chen, Yue Dong, Pieter Peers, Hongzhi Wu, Xin Tong*<br>
SIGGRAPH 2023
[[Paper](https://nrhints.github.io/pdfs/nrhints-sig23.pdf)] [[Project](https://nrhints.github.io/)] [[Github](https://github.com/iamNCJ/NRHints)]

**Dyn-E: Local Appearance Editing of Dynamic Neural Radiance Fields**<br>
*Shangzhan Zhang, Sida Peng, Yinji ShenTu, Qing Shuai, Tianrun Chen, Kaicheng Yu, Hujun Bao, Xiaowei Zhou*<br>
arXiv preprint, 24 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.12909)] [[Project](https://dyn-e.github.io/)]

**Seal-3D: Interactive Pixel-Level Editing for Neural Radiance Fields**<br>
*Xiangyu Wang, Jingsen Zhu, Qi Ye, Yuchi Huo, Yunlong Ran, Zhihua Zhong, Jiming Chen*<br>
ICCV 2023, 27 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.15131)] [[Project](https://windingwind.github.io/seal-3d/)] [[Github](https://github.com/windingwind/seal-3d/)]

**Mirror-NeRF: Learning Neural Radiance Fields for Mirrors with Whitted-Style Ray Tracing**<br>
*Junyi Zeng, Chong Bao, Rui Chen, Zilong Dong, Guofeng Zhang, Hujun Bao, Zhaopeng Cui*<br>
ACMMM 2023, 7 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.03280)] [[Project](https://zju3dv.github.io/Mirror-NeRF/)]

**Learning Unified Decompositional and Compositional NeRF for Editable Novel View Synthesis**<br>
*Yuxin Wang, Wayne Wu, Dan Xu*<br>
ICCV 2023, 5 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.02840)] [[Project](https://w-ted.github.io/publications/udc-nerf)]

**DeformToon3D: Deformable 3D Toonification from Neural Radiance Fields**<br>
*Junzhe Zhang, Yushi Lan, Shuai Yang, Fangzhou Hong, Quan Wang, Chai Kiat Yeo, Ziwei Liu, Chen Change Loy*<br>
ICCV 2023, 8 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.04410)] [[Project](https://www.mmlab-ntu.com/project/deformtoon3d/)] [[Github](https://github.com/junzhezhang/DeformToon3D)]

**Locally Stylized Neural Radiance Fields**<br>
*Hong-Wing Pang, Binh-Son Hua, Sai-Kit Yeung*<br>
ICCV 2023, 19 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.10684)]

**Language-driven Object Fusion into Neural Radiance Fields with Pose-Conditioned Dataset Updates**<br>
*Ka Chun Shum, Jaeyeon Kim, Binh-Son Hua, Duc Thanh Nguyen, Sai-Kit Yeung*<br>
arXiv preprint, 20 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.11281)]

**MM-NeRF: Multimodal-Guided 3D Multi-Style Transfer of Neural Radiance Field**<br>
*Zijiang Yang, Zhongwei Qiu, Chang Xu, Dongmei Fu*<br>
arXiv preprint, 24 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.13607)]

**ED-NeRF: Efficient Text-Guided Editing of 3D Scene using Latent Space NeRF**<br>
*Jangho Park, Gihyun Kwon, Jong Chul Ye*<br>
arXiv preprint, 4 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.02712)]

**Neural Impostor: Editing Neural Radiance Fields with Explicit Shape Manipulation**<br>
*Ruiyang Liu, Jinxu Xiang, Bowen Zhao, Ran Zhang, Jingyi Yu, Changxi Zheng*<br>
Pacific Graphics 2023, 9 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.05391)]

**A Real-time Method for Inserting Virtual Objects into Neural Radiance Fields**<br>
*Keyang Ye, Hongzhi Wu, Xin Tong, Kun Zhou*<br>
arXiv preprint, 9 Oct, 2023<br>
[[arXiv](https://arxiv.org/abs/2310.05837)]

**Customize your NeRF: Adaptive Source Driven 3D Scene Editing via Local-Global Iterative Training**<br>
*Runze He, Shaofei Huang, Xuecheng Nie, Tianrui Hui, Luoqi Liu, Jiao Dai, Jizhong Han, Guanbin Li, Si Liu*<br>
arXiv preprint, 4 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.01663)] [[Project](https://customnerf.github.io/)]

**NeRFiller: Completing Scenes via Generative 3D Inpainting**<br>
*Ethan Weber, Aleksander Hołyński, Varun Jampani, Saurabh Saxena, Noah Snavely, Abhishek Kar, Angjoo Kanazawa*<br>
CVPR 2024, 7 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.04560)] [[Project](https://ethanweber.me/nerfiller/)] [[Code](https://github.com/ethanweber/nerfiller)]

**Towards 4D Human Video Stylization**<br>
*Tiantian Wang, Xinxin Zuo, Fangzhou Mu, Jian Wang, Ming-Hsuan Yang*<br>
arXiv preprint, 7 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.04143)]

### NeRF + Open Surface Reconstruction and Cloth Simulation

**NeuralUDF: Learning Unsigned Distance Fields for Multi-view Reconstruction of Surfaces with Arbitrary Topologies**<br>
*Xiaoxiao Long, Cheng Lin, Lingjie Liu, Yuan Liu, Peng Wang, Christian Theobalt, Taku Komura, Wenping Wang*<br>
CVPR 2023, 25 Nov 2022 <br>
[[arXiv](https://arxiv.org/abs/2211.14173)] [[Project](https://www.xxlong.site/NeuralUDF/)] [[Github](https://github.com/xxlong0/NeuralUDF)] [[Video](https://www.bilibili.com/video/BV14g411x7nT/)]

**NeAT: Learning Neural Implicit Surfaces with Arbitrary Topologies from Multi-view Images**<br>
*Xiaoxu Meng, Weikai Chen, Bo Yang*<br>
CVPR 2023, 21 Mar 2023 <br>
[[arXiv](https://arxiv.org/abs/2303.12012)] [[Project](https://xmeng525.github.io/xiaoxumeng.github.io/projects/cvpr23_neat)] [[Github](https://github.com/xmeng525/NeAT)] [[Video](https://www.bilibili.com/video/BV1ix4y1w7NC/)]

**NeuralClothSim: Neural Deformation Fields Meet the Kirchhoff-Love Thin Shell Theory**<br>
*Navami Kairanda, Marc Habermann, Christian Theobalt, Vladislav Golyanik*<br>
arXiv preprint, 24 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.12970)] [[Project](https://4dqv.mpi-inf.mpg.de/NeuralClothSim/)] [[Video](https://www.bilibili.com/video/BV1mF411C7JT/)]


### NeRF + Segmentation

**SSDNeRF: Semantic Soft Decomposition of Neural Radiance Fields**<br>
*Siddhant Ranade, Christoph Lassner, Kai Li, Christian Haene, Shen-Chi Chen, Jean-Charles Bazin, Sofien Bouaziz*<br>
arXiv preprint, 7 Dec 2022 <br>
[[arXiv](https://arxiv.org/abs/2212.03406)] [[Project](https://www.siddhantranade.com/research/2022/12/06/SSDNeRF-Semantic-Soft-Decomposition-of-Neural-Radiance-Fields.html)] [[Video](https://www.bilibili.com/video/BV1XR4y1C7Yf/)]

:fire:**Panoptic Lifting for 3D Scene Understanding with Neural Fields**<br>
*Yawar Siddiqui, Lorenzo Porzi, Samuel Rota Buló, Norman Müller, Matthias Nießner, Angela Dai, Peter Kontschieder*<br>
CVPR 2023, 19 Dec 2022 <br>
[[arXiv](https://arxiv.org/abs/2212.09802)] [[Project](https://nihalsid.github.io/panoptic-lifting/)] [[Github](https://github.com/nihalsid/panoptic-lifting)] [[Video](https://www.youtube.com/watch?v=QtsiL-6rSuM)]

**Segment Anything in 3D with NeRFs**<br>
*Jiazhong Cen, Zanwei Zhou, Jiemin Fang, Wei Shen, Lingxi Xie, Dongsheng Jiang, Xiaopeng Zhang, Qi Tian*<br>
arXiv preprint, 24 Apr 2023 <br>
[[arXiv](https://arxiv.org/abs/2304.12308)] [[Project](https://jumpat.github.io/SA3D/)] [[Github](https://github.com/Jumpat/SegmentAnythingin3D)] [[Video](https://www.bilibili.com/video/BV1Xo4y1b7s6/)]

**Obj-NeRF: Extract Object NeRFs from Multi-view Images**<br>
*Zhiyi Li, Lihe Ding, Tianfan Xue*<br>
arXiv preprint, 26 Nov, 2023<br>
[[arXiv](https://arxiv.org/abs/2311.15291)]

**SANeRF-HQ: Segment Anything for NeRF in High Quality**<br>
*Yichen Liu, Benran Hu, Chi-Keung Tang, Yu-Wing Tai*<br>
arXiv preprint, 3 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.01531)] [[Project](https://lyclyc52.github.io/SANeRF-HQ/)]

### NeRF + Semantic

**uSF: Learning Neural Semantic Field with Uncertainty**<br>
*Vsevolod Skorokhodov, Darya Drozdova, Dmitry Yudin*<br>
arXiv preprint, 13 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.08012)] [[Code](https://github.com/sevashasla/usf/)]

### NeRF + Mesh Extraction

:fire:**Delicate Textured Mesh Recovery from NeRF via Adaptive Surface Refinement**<br>
*Jiaxiang Tang, Hang Zhou, Xiaokang Chen, Tianshu Hu, Errui Ding, Jingdong Wang, Gang Zeng*<br>
arXiv preprint, 3 Mar 2023 <br>
[[arXiv/](https://arxiv.org/abs/2303.02091)] [[Project](https://me.kiui.moe/nerf2mesh/)] [[Github](https://github.com/ashawkey/nerf2mesh)] [[Video](https://www.bilibili.com/video/BV18M41147JN/)]

**TeTriRF: Temporal Tri-Plane Radiance Fields for Efficient Free-Viewpoint Video**<br>
*Minye Wu, Zehao Wang, Georgios Kouros, Tinne Tuytelaars*<br>
arXiv preprint, 10 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.06713)]

### NeRF + Codec/Streaming

**Learning Neural Volumetric Field for Point Cloud Geometry Compression**<br>
*Yueyu Hu, Yao Wang*<br>
PCS 2022, 11 Dec 2022 <br>
[[arXiv](https://arxiv.org/abs/2212.05589)] [[Project](http://yenchenlin.me/inerf/)] [[Github](https://github.com/yenchenlin/iNeRF-public)]

**Towards Scalable Neural Representation for Diverse Videos**<br>
*Bo He, Xitong Yang, Hanyu Wang, Zuxuan Wu, Hao Chen, Shuaiyi Huang, Yixuan Ren, Ser-Nam Lim, Abhinav Shrivastava*<br>
CVPR 2023, 24 Mar 2023 <br>
[[arXiv](https://arxiv.org/abs/2303.14124)] [[Project](https://boheumd.github.io/D-NeRV/)] [[Github](https://github.com/boheumd/D-NeRV)]

:fire:**Neural Residual Radiance Fields for Streamably Free-Viewpoint Videos**<br>
*Liao Wang, Qiang Hu, Qihan He, Ziyu Wang, Jingyi Yu, Tinne Tuytelaars, Lan Xu, Minye Wu*<br>
CVPR 2023, 11 Dec 2022 <br>
[[arXiv](https://arxiv.org/abs/2304.04452)] [[Project](https://aoliao12138.github.io/ReRF/)]

**VideoRF: Rendering Dynamic Radiance Fields as 2D Feature Video Streams**<br>
*Liao Wang, Kaixin Yao, Chengcheng Guo, Zhirui Zhang, Qiang Hu, Jingyi Yu, Lan Xu, Minye Wu*<br>
arxiv preprint, 3 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.01407)] [[Project](https://aoliao12138.github.io/VideoRF)]

:fire:**SlimmeRF: Slimmable Radiance Fields**<br>
*Shiran Yuan, Hao Zhao*<br>
3DV 2024, 15 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.10034)] [[Project](https://shiran-yuan.github.io/SlimmeRF/)] [[Code](https://github.com/Shiran-Yuan/SlimmeRF)]

### NeRF + Model Conversion

**One is All: Bridging the Gap Between Neural Radiance Fields Architectures with Progressive Volume Distillation**<br>
*Shuangkang Fang, Weixin Xu, Heng Wang, Yi Yang, Yufeng Wang, Shuchang Zhou*<br>
AAAI 2023, 29 Nov 2022 <br>
[[arXiv](https://arxiv.org/abs/2211.15977)] [[Project](https://sk-fun.fun/PVD)] [[Github](https://github.com/megvii-research/AAAI2023-PVD)] [[PVD-AL Github](https://github.com/megvii-research/AAAI2023-PVD/tree/PVD-AL)]

### NeRF + Medical/Biology

**MedNeRF: Medical Neural Radiance Fields for Reconstructing 3D-aware CT-Projections from a Single X-ray**<br>
*Abril Corona-Figueroa, Jonathan Frawley, Sam Bond-Taylor, Sarath Bethapudi, Hubert P. H. Shum, Chris G. Willcocks*<br>
EMBC 2022, 2 Feb 2022 <br>
[[arXiv](https://arxiv.org/abs/2202.01020)] [[Github](https://github.com/abrilcf/mednerf)]

**NeAT: Neural Adaptive Tomography**<br>
*Darius Rückert, Yuanhao Wang, Rui Li, Ramzi Idoughi, Wolfgang Heidrich*<br>
arXiv preprint, 4 Feb, 2022<br>
[[arXiv](https://arxiv.org/abs/2202.02171)]

**NAF: Neural Attenuation Fields for Sparse-View CBCT Reconstruction**<br>
*Ruyi Zha, Yanhao Zhang, Hongdong Li*<br>
MICCAI 2022, 29 Sep 2022<br>
[[arXiv](https://arxiv.org/abs/2209.14540)]

**SNAF: Sparse-view CBCT Reconstruction with Neural Attenuation Fields**<br>
*Yu Fang, Lanzhuju Mei, Changjian Li, Yuan Liu, Wenping Wang, Zhiming Cui, Dinggang Shen*<br>
arXiv preprint, 30 Nov 2022<br>
[[arXiv](https://arxiv.org/abs/2211.17048)]

**Learning Deep Intensity Field for Extremely Sparse-View CBCT Reconstruction**<br>
*Yiqun Lin, Zhongjin Luo, Wei Zhao, Xiaomeng Li*<br>
arXiv preprint, 12 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.06681)]

**Geometry-Aware Attenuation Field Learning for Sparse-View CBCT Reconstruction**<br>
*Zhentao Liu, Yu Fang, Changjian Li, Han Wu, Yuan Liu, Zhiming Cui, Dinggang Shen*<br>
arXiv preprint, 26 Mar, 2023<br>
[[arXiv](https://arxiv.org/abs/2303.14739)]

**ColonNeRF: Neural Radiance Fields for High-Fidelity Long-Sequence Colonoscopy Reconstruction**<br>
*Yufei Shi, Beijia Lu, Jia-Wei Liu, Ming Li, Mike Zheng Shou*<br>
arXiv preprint, 4 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02015)] [[Project](https://showlab.github.io/ColonNeRF/)]

**Efficient Deformable Tissue Reconstruction via Orthogonal Neural Plane**<br>
*Chen Yang, Kailing Wang, Yuehao Wang, Qi Dou, Xiaokang Yang, Wei Shen*<br>
MICCI 2024, 23 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.15253)] [[Code](https://github.com/Loping151/ForPlane)]

### NeRF + Inverse Rendering

:fire:**Multi-view Inverse Rendering for Large-scale Real-world Indoor Scenes**<br>
*Zhen Li, Lingli Wang, Mofang Cheng, Cihui Pan, Jiaqi Yang*<br>
CVPR 2023, 18 Nov 2022 <br>
[[arXiv](https://arxiv.org/abs/2211.10206)] [[Project](http://yodlee.top/TexIR/)] [[Github](http://github.com/LZleejean/TexIR_code)] [[Video](https://www.bilibili.com/video/BV1gM411K7ik/)]

:fire:**TensoIR: Tensorial Inverse Rendering**<br>
*Haian Jin, Isabella Liu, Peijia Xu, Xiaoshuai Zhang, Songfang Han, Sai Bi, Xiaowei Zhou, Zexiang Xu, Hao Su*<br>
CVPR 2023, 24 Apr 2023 <br>
[[arXiv](https://arxiv.org/abs/2304.12461)] [[Project](https://haian-jin.github.io/TensoIR/)] [[Github](https://github.com/Haian-Jin/TensoIR)] [[Video](https://www.bilibili.com/video/BV1Fc411n7Gb/)]

:fire:**Inverse Global Illumination using a Neural Radiometric Prior**<br>
*Saeed Hadadan, Geng Lin, Jan Novák, Fabrice Rousselle, Matthias Zwicker*<br>
SIGGRAPH 2023, 3 May 2023 <br>
[[arXiv](https://arxiv.org/abs/2305.02192)] [[Notes](./paper_discussions/InverseGlobalIllumination.md)]

**SplitNeRF: Split Sum Approximation Neural Field for Joint Geometry, Illumination, and Material Estimation**<br>
*Jesus Zarzar, Bernard Ghanem*<br>
arXiv preprint, 28 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16671)] 

### NeRF + Texture Synthesis

**NeRF-Tex: Neural Reflectance Field Textures**<br>
*Hendrik Baatz, Jonathan Granskog, Marios Papas, Fabrice Rousselle, Jan Novák*<br>
EGSR 2021, 22 Jun, 2021<br>
[[Paper](https://d1qx31qr3h6wln.cloudfront.net/publications/NeRFTex.pdf)] [[Project](https://research.nvidia.com/publication/2021-06_nerf-tex-neural-reflectance-field-textures)]

**NeRF-Texture: Texture Synthesis With Neural Radiance Fields**<br>
*Yihua Huang, Yan-Pei Cao, Yu-Kun Lai, Ying Shan, Lin Gao*<br>
SIGGRAPH 2023<br>
[[Video](https://www.bilibili.com/video/BV1UW4y1f7oK/)]

### NeRF + Transparent Object

**Neural Radiance Fields for Transparent Object Using Visual Hull**<br>
*Heechan Yoon, Seungkyu Lee*<br>
arXiv preprint, 13 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.08118)]



### NeRF + Transparent Object

**Neural Radiance Fields for Transparent Object Using Visual Hull**<br>
*Heechan Yoon, Seungkyu Lee*<br>
arXiv preprint, 13 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.08118)]

## NeRF + Robotics

**MACS: Mass Conditioned 3D Hand and Object Motion Synthesis**<br>
*Soshi Shimada, Franziska Mueller, Jan Bednarik, Bardia Doosti, Bernd Bickel, Danhang Tang, Vladislav Golyanik, Jonathan Taylor, Christian Theobalt, Thabo Beeler*<br>
arXiv preprint, 22 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.14929)]

### NeRF + Transparent and Specular

**NeRRF: 3D Reconstruction and View Synthesis for Transparent and Specular Objects with Neural Refractive-Reflective Fields**<br>
*Xiaoxue Chen, Junchen Liu, Hao Zhao, Guyue Zhou, Ya-Qin Zhang*<br>
arXiv preprint, 22 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.13039)]

**TraM-NeRF: Tracing Mirror and Near-Perfect Specular Reflections through Neural Radiance Fields**<br>
*Leif Van Holland, Ruben Bliersbach, Jan U. Müller, Patrick Stotko, Reinhard Klein*<br>
arXiv preprint, 16 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.10650)]

**SpecNeRF: Gaussian Directional Encoding for Specular Reflections**<br>
*Li Ma, Vasu Agrawal, Haithem Turki, Changil Kim, Chen Gao, Pedro Sander, Michael Zollhöfer, Christian Richardt*<br>
CVPR 2024, 20 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.13102)] [[Project](https://limacv.github.io/SpecNeRF_web/)] [[Video](https://www.youtube.com/watch?v=3nUooe3pVA0)]

**UniSDF: Unifying Neural Representations for High-Fidelity 3D Reconstruction of Complex Scenes with Reflections**<br>
*Fangjinhua Wang, Marie-Julie Rakotosaona, Michael Niemeyer, Richard Szeliski, Marc Pollefeys, Federico Tombari*<br>
arXiv preprint, 20 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.13285)] [[Project](https://fangjinhuawang.github.io/UniSDF/)]



### Other 3D Generative Work

:fire:**Patch-based 3D Natural Scene Generation from a Single Example**<br>
*Weiyu Li, Xuelin Chen, Jue Wang, Baoquan Chen*<br>
CVPR 2023, 25 Apr 2023 <br>
[[arXiv](https://arxiv.org/abs/2304.12670)] [[Project](http://weiyuli.xyz/Sin3DGen/)] [[Github](https://github.com/wyysf-98/Sin3DGen)] [[Notes](./paper_discussions/Sin3DGen.md)]

### NeRF + Other applications

**ORCa: Glossy Objects as Radiance Field Cameras**<br>
*Kushagra Tiwary, Akshat Dave, Nikhil Behari, Tzofi Klinghoffer, Ashok Veeraraghavan, Ramesh Raskar*<br>
arXiv preprint, 8 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.04531)] [[Projects](https://ktiwary2.github.io/objectsascam/)] [[Video](https://www.bilibili.com/video/BV16L411v7iU/)]

**WaterNeRF: Neural Radiance Fields for Underwater Scenes**<br>
*Advaith Venkatramanan Sethuraman, Manikandasriram Srinivasan Ramanagopal, Katherine A. Skinner*<br>
arXiv preprint, 27 Sep 2022<br>
[[arXiv](https://arxiv.org/abs/2209.13091)]

**Virtual Pets: Animatable Animal Generation in 3D Scenes**<br>
*Yen-Chi Cheng, Chieh Hubert Lin, Chaoyang Wang, Yash Kant, Sergey Tulyakov, Alexander Schwing, Liangyan Gui, Hsin-Ying Lee*<br>
arXiv preprint, 21 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.14154)] [[Project](https://yccyenchicheng.github.io/VirtualPets/)]

### NeRF + Quality Metric

**Towards a Robust Framework for NeRF Evaluation**<br>
*Adrian Azzarelli, Nantheera Anantrasirichai, David R Bull*<br>
arXiv preprint, 29 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.18079)]

### NeRF + CAD

**Magic NeRF Lens: Interactive Fusion of Neural Radiance Fields for Virtual Facility Inspection**<br>
*Ke Li, Susanne Schmidt, Tim Rolff, Reinhard Bacher, Wim Leemans, Frank Steinicke*<br>
TCVG, 19 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.09860)]

### NeRF + GIS

**Improving NeRF with Height Data for Utilization of GIS Data**<br>
*Hinata Aoki, Takao Yamanaka*<br>
ICIP 2023, 15 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.07729)]

### NeRF + Satellite Images

**Sat-NeRF: Learning Multi-View Satellite Photogrammetry With Transient Objects and Shadow Modeling Using RPC Cameras**<br>
*Roger Marí, Gabriele Facciolo, Thibaud Ehret*<br>
CVPR 2022, 16 Mar 2022<br>
[[arXiv](https://arxiv.org/abs/2203.08896)] 

**SparseSat-NeRF: Dense Depth Supervised Neural Radiance Fields for Sparse Satellite Images**<br>
*Lulin Zhang, Ewelina Rupnik*<br>
ISPRS Annals 2023, 1 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.00277)] [[Github](https://github.com/LulinZhang/SpS-NeRF)]

**Enabling Neural Radiance Fields (NeRF) for Large-scale Aerial Images -- A Multi-tiling Approaching and the Geometry Assessment of NeRF**<br>
*Ningli Xu, Rongjun Qin, Debao Huang, Fabio Remondino*<br>
arXiv preprint, 1 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.00530)]

### NeRF + Copyright protection and Security

**CopyRNeRF: Protecting the CopyRight of Neural Radiance Fields**<br>
*Ziyuan Luo, Qing Guo, Ka Chun Cheung, Simon See, Renjie Wan*<br>
ICCV 2023, 21 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.11526)] [[Project](https://luo-ziyuan.github.io/copyrnerf/)]

**Steganography for Neural Radiance Fields by Backdooring**<br>
*Weina Dong, Jia Liu, Yan Ke, Lifeng Chen, Wenquan Sun, Xiaozhong Pan*<br>
arXiv preprint, 19 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.10503)]

**Targeted Adversarial Attacks on Generalizable Neural Radiance Fields**<br>
Andras Horvath, Csaba M. Jozsa<br>
*arXiv preprint, 5 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.03578)]

### NeRF + Motion Detection

**3D Motion Magnification: Visualizing Subtle Motions with Time Varying Radiance Fields**<br>
*Brandon Y. Feng, Hadi Alzayer, Michael Rubinstein, William T. Freeman, Jia-Bin Huang*<br>
ICCV 2023, 7 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.03757)] [[Project](https://3d-motion-magnification.github.io/)]

**C-NERF: Representing Scene Changes as Directional Consistency Difference-based NeRF**<br>
*Rui Huang, Binbin Jiang, Qingyi Zhao, William Wang, Yuxiang Zhang, Qing Guo*<br>
arXiv 2023, 5 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02751)]

### Datasets

**MVImgNet: A Large-scale Dataset of Multi-view Images**<br>
*Xianggang Yu, Mutian Xu, Yidan Zhang, Haolin Liu, Chongjie Ye, Yushuang Wu, Zizheng Yan, Chenming Zhu, Zhangyang Xiong, Tianyou Liang, Guanying Chen, Shuguang Cui, Xiaoguang Han*<br>
CVPR 2023, 10 Mar 2023 <br>
[[arXiv](https://arxiv.org/abs/2303.06042)] [[Project](https://gaplab.cuhk.edu.cn/projects/MVImgNet/#table_stat)] [[Github](https://github.com/GAP-LAB-CUHK-SZ/MVImgNet)] [[Notes](./paper_discussions/MVImgNet.md)]

**DiVA-360: The Dynamic Visuo-Audio Dataset for Immersive Neural Fields**<br>
*Cheng-You Lu, Peisen Zhou, Angela Xing, Chandradeep Pokhariya, Arnab Dey, Ishaan Shah, Rugved Mavidipalli, Dylan Hu, Andrew Comport, Kefan Chen, Srinath Sridhar*<br>
arXiv preprint, 31 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.16897)] [[Project](https://diva360.github.io/)]

**SingingHead: A Large-scale 4D Dataset for Singing Head Animation**<br>
*Sijing Wu, Yunhao Li, Weitian Zhang, Jun Jia, Yucheng Zhu, Yichao Yan, Guangtao Zhai*<br>
arXiv preprint, 7 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.04369)] [[Project](https://wsj-sjtu.github.io/SingingHead/)] [[Code](https://github.com/wsj-sjtu/SingingHead)]

### Neural Surface Reconstruction

**Neural Kernel Surface Reconstruction**<br>
*Jiahui Huang, Zan Gojcic, Matan Atzmon, Or Litany, Sanja Fidler, Francis Williams*<br>
CVPR 2023, 31 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.19590)]

**Neuralangelo: High-Fidelity Neural Surface Reconstruction**<br>
*Zhaoshuo Li, Thomas Müller, Alex Evans, Russell H. Taylor, Mathias Unberath, Ming-Yu Liu, Chen-Hsuan Lin*<br>
CVPR 2023, 5 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.03092)] [[Project](https://research.nvidia.com/labs/dir/neuralangelo)] [[Video](https://www.bilibili.com/video/BV1mh4y1d7rX/)]

## Other Important Related Work

### Depth Estimation

**Repurposing Diffusion-Based Image Generators for Monocular Depth Estimation**<br>
*Bingxin Ke, Anton Obukhov, Shengyu Huang, Nando Metzger, Rodrigo Caye Daudt, Konrad Schindler*<br>
CVPR 2024, 4 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02145)] [[Project](https://marigoldmonodepth.github.io/)] [[Code](https://github.com/prs-eth/marigold)]

## Contributors

Thanks to the community and hoping more and more people are joining us and submit commits and PRs!<br>

<a href = "https://github.com/yangjiheng/nerf_and_beyond_docs/graphs/contributors">
  <img src = "https://contrib.rocks/image?repo=yangjiheng/nerf_and_beyond_docs"/>
</a>

Made with [contributors-img](https://contrib.rocks).

## License

CC-0
