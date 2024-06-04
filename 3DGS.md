# <p align='center'>`NeRF and Beyond Docs`</p>

3DGS is raising quickly, it is expected to be another branch of 3D vision that's going to be active for quick a long time. So let's keep track of everything that's happening within the 3DGS domain.

<summary>Table of Content</summary>

- [`NeRF and Beyond Docs`](#nerf-and-beyond-docs)
  - [3DGS Original Paper](#3dgs-original-paper)
  - [3DGS Surveys](#3dgs-surveys)
  - [3DGS Quality Enhancement](#3dgs-quality-enhancement)
  - [3DGS Acceleration](#3dgs-acceleration)
  - [3DGS Surface Reconstruction](#3dgs-surface-reconstruction)
  - [3DGS Based Dynamic Scene](#3dgs-based-dynamic-scene)
  - [3DGS Few-shot Reconstruction](#3dgs-few-shot-reconstruction)
  - [3DGS Weak Camera Pose](#3dgs-weak-camera-pose)
  - [3DGS Indoor Scene Reconstruction](#3dgs-indoor-scene-reconstruction)
  - [3DGS Based Large Scene Reconstruction](#3dgs-based-large-scene-reconstruction)
  - [3DGS Autonomous Drivibng](#3dgs-autonomous-drivibng)
  - [3DGS Based AIGC](#3dgs-based-aigc)
  - [3DGS Model Compactness Optimization](#3dgs-model-compactness-optimization)
  - [3DGS Avatar Generation](#3dgs-avatar-generation)
  - [3DGS Scene Editing and Animation](#3dgs-scene-editing-and-animation)
  - [3DGS for Computer Graphics](#3dgs-for-computer-graphics)
  - [3DGS Based Scene Understanding](#3dgs-based-scene-understanding)
  - [3DGS Based SLAM](#3dgs-based-slam)
  - [3DGS Based Inverse Rendering](#3dgs-based-inverse-rendering)
  - [3DGS Imaging Tasks](#3dgs-imaging-tasks)
  - [3DGS Scene Understanding](#3dgs-scene-understanding)
  - [3DGS Applications](#3dgs-applications)
    - [3DGS Application in Animal Reconstruction](#3dgs-application-in-animal-reconstruction)
    - [3DGS Application in Medical Imaging](#3dgs-application-in-medical-imaging)
  
## 3DGS Original Paper

**3D Gaussian Splatting for Real-Time Radiance Field Rendering**<br>
*Bernhard Kerbl, Georgios Kopanas, Thomas Leimkühler, George Drettakis*<br>
ACM ToG 2023, 8 August, 2023<br>
[[arXiv](https://arxiv.org/abs/2308.04079)] [[Project](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)] [[Github](https://github.com/graphdeco-inria/gaussian-splatting)]

## 3DGS Surveys

**A Survey on 3D Gaussian Splatting**<br>
*Guikun Chen, Wenguan Wang*<br>
arXiv preprint, 8 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.03890)]

**3D Gaussian as a New Vision Era: A Survey**<br>
*Ben Fei, Jingyi Xu, Rui Zhang, Qingyuan Zhou, Weidong Yang, Ying He*<br>
arXiv preprint, 11 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.07181)]

## 3DGS Quality Enhancement

**Mip-Splatting: Alias-free 3D Gaussian Splatting**<br>
*Zehao Yu, Anpei Chen, Binbin Huang, Torsten Sattler, Andreas Geiger*<br>
arXiv preprint, 27 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16493)] [[Project](https://niujinshuchong.github.io/mip-splatting/)]

**Multi-Scale 3D Gaussian Splatting for Anti-Aliased Rendering**<br>
*Zhiwen Yan, Weng Fei Low, Yu Chen, Gim Hee Lee*<br>
arXiv preprint, 28 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.17089)]

**Scaffold-GS: Structured 3D Gaussians for View-Adaptive Rendering**<br>
*Tao Lu, Mulin Yu, Linning Xu, Yuanbo Xiangli, Limin Wang, Dahua Lin, Bo Dai*<br>
arXiv preprint, 30 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2312.00109)] [[Project](https://city-super.github.io/scaffold-gs/)]

**Gaussian Splitting Algorithm with Color and Opacity Depended on Viewing Direction**<br>
*Dawid Malarz, Weronika Smolak, Jacek Tabor, Sławomir Tadeja, Przemysław Spurek*<br>
arXiv preprint, 21 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.13729)]

**TRIPS: Trilinear Point Splatting for Real-Time Radiance Field Rendering**<br>
*Linus Franke, Darius Rückert, Laura Fink, Marc Stamminger*<br>
Eurographics 2024, 11 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.06003)] [[Project](https://lfranke.github.io/trips/)] [[Code](https://github.com/lfranke/trips)] [[Video](https://www.youtube.com/watch?v=Nw4A1tIcErQ&feature=youtu.be)]

**Optimal Projection for 3D Gaussian Splatting**<br>
*Letian Huang, Jiayang Bai, Jie Guo, Yanwen Guo*<br>
arXiv preprint, 1 Feb 2024<br>
[[arXiv](https://browse.arxiv.org/abs/2402.00752)]

**GaMeS: Mesh-Based Adapting and Modification of Gaussian Splatting**<br>
*Joanna Waczyńska, Piotr Borycki, Sławomir Tadeja, Jacek Tabor, Przemysław Spurek*<br>
arXiv preprint, 2 Feb 2024<br>
[[arXiv](https://browse.arxiv.org/abs/2402.01459)]

## 3DGS Acceleration

**EAGLES: Efficient Accelerated 3D Gaussians with Lightweight EncodingS**<br>
*Sharath Girish, Kamal Gupta, Abhinav Shrivastava*<br>
arXiv preprint, 7 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.04564)] [[Project](https://efficientgaussian.github.io/)] [[Code](https://github.com/Sharath-girish/efficientgaussian)]

**StopThePop: Sorted Gaussian Splatting for View-Consistent Real-time Rendering**<br>
*Lukas Radl, Michael Steiner, Mathias Parger, Alexander Weinrauch, Bernhard Kerbl, Markus Steinberger*<br>
SIGGRAPH 2024, 1 Feb 2024<br>
[[arXiv](https://browse.arxiv.org/abs/2402.00525)] [[Project](https://r4dl.github.io/StopThePop/)] [[Code](https://github.com/r4dl/StopThePop)] [[Video](https://www.youtube.com/watch?v=EmcXtHYhigk)]

**GES: Generalized Exponential Splatting for Efficient Radiance Field Rendering**<br>
*Abdullah Hamdi, Luke Melas-Kyriazi, Guocheng Qian, Jinjie Mai, Ruoshi Liu, Carl Vondrick, Bernard Ghanem, Andrea Vedaldi*<br>
CVPR 2024, 15 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.10128)] [[Project](https://abdullahamdi.com/ges/)] [[Code](https://github.com/ajhamdi/ges-splatting)] [[Video](https://www.youtube.com/watch?v=edSvNy3roV8&feature=youtu.be)]

## 3DGS Surface Reconstruction

**SuGaR: Surface-Aligned Gaussian Splatting for Efficient 3D Mesh Reconstruction and High-Quality Mesh Rendering**<br>
*Antoine Guédon, Vincent Lepetit*<br>
arXiv preprint, 21 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.12775)] [[Project](https://imagine.enpc.fr/~guedona/sugar/)]

**NeuSG: Neural Implicit Surface Reconstruction with 3D Gaussian Splatting Guidance**<br>
*Hanlin Chen, Chen Li, Gim Hee Lee*<br>
arXiv preprint, 1 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.00846)]

## 3DGS Based Dynamic Scene

**Dynamic 3D Gaussians: Tracking by Persistent Dynamic View Synthesis**<br>
*Jonathon Luiten, Georgios Kopanas, Bastian Leibe, Deva Ramanan*<br>
arXiv preprint, 18 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.09713)] [[Project](https://dynamic3dgaussians.github.io/)] [[Github](https://github.com/JonathonLuiten/Dynamic3DGaussians)]

**Deformable 3D Gaussians for High-Fidelity Monocular Dynamic Scene Reconstruction**<br>
*Ziyi Yang, Xinyu Gao, Wen Zhou, Shaohui Jiao, Yuqing Zhang, Xiaogang Jin*<br>
arXiv preprint, 22 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.13101)]

**4D Gaussian Splatting for Real-Time Dynamic Scene Rendering**<br>
*Guanjun Wu, Taoran Yi, Jiemin Fang, Lingxi Xie, Xiaopeng Zhang, Wei Wei, Wenyu Liu, Qi Tian, Xinggang Wang*<br>
arXiv preprint, 12 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.08528)] [[Project](https://guanjunwu.github.io/4dgs/)] [[Github](https://github.com/hustvl/4DGaussians)]

**Real-time Photorealistic Dynamic Scene Representation and Rendering with 4D Gaussian Splatting**<br>
*Zeyu Yang, Hongye Yang, Zijie Pan, Xiatian Zhu, Li Zhang*<br>
arXiv preprint, 16 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.10642)]

**Neural Parametric Gaussians for Monocular Non-Rigid Object Reconstruction**<br>
*Devikalyan Das, Christopher Wewer, Raza Yunus, Eddy Ilg, Jan Eric Lenssen*<br>
arXiv preprint, 2 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.01196)]

**Gaussian-Flow: 4D Reconstruction with Dynamic 3D Gaussian Particle**<br>
*Youtian Lin, Zuozhuo Dai, Siyu Zhu, Yao Yao*<br>
arXiv preprint, 6 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.03431)]

**CoGS: Controllable Gaussian Splatting**<br>
*Heng Yu, Joel Julin, Zoltán Á. Milacski, Koichiro Niinuma, László A. Jeni*<br>
CVPR 2024, 9 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.05664)]

**GauFRe: Gaussian Deformation Fields for Real-time Dynamic Novel View Synthesis**<br>
*Yiqing Liang, Numair Khan, Zhengqin Li, Thu Nguyen-Phuoc, Douglas Lanman, James Tompkin, Lei Xiao*<br>
arXiv preprint, 18 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.11458)] [[Project](https://lynl7130.github.io/gaufre/index.html)]

**SC-GS: Sparse-Controlled Gaussian Splatting for Editable Dynamic Scenes**<br>
*Yi-Hua Huang, Yang-Tian Sun, Ziyi Yang, Xiaoyang Lyu, Yan-Pei Cao, Xiaojuan Qi*<br>
CVPR 2024, 4 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.14937)] [[Project](https://yihua7.github.io/SC-GS-web/)] [[Code](https://github.com/yihua7/SC-GS)] [[Video](https://www.youtube.com/watch?v=CYQYX_0xi5E&feature=youtu.be)]

**Spacetime Gaussian Feature Splatting for Real-Time Dynamic View Synthesis**<br>
*Zhan Li, Zhang Chen, Zhong Li, Yi Xu*<br>
CVPR 2024, 28 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.16812)] [[Project](https://oppo-us-research.github.io/SpacetimeGaussians-website/)] [[Code](https://github.com/oppo-us-research/SpacetimeGaussians)] [[Video](https://www.youtube.com/watch?v=YsPPmf-E6Lg)]

**4D Gaussian Splatting: Towards Efficient Novel View Synthesis for Dynamic Scenes**<br>
*Yuanxing Duan, Fangyin Wei, Qiyu Dai, Yuhang He, Wenzheng Chen, Baoquan Chen*<br>
arXiv preprint, 5 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.03307)]

**Mesh-based Gaussian Splatting for Real-time Large-scale Deformation**<br>
*Lin Gao, Jie Yang, Bo-Tao Zhang, Jia-Mu Sun, Yu-Jie Yuan, Hongbo Fu, Yu-Kun Lai*<br>
arXiv preprint, 7 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.04796)]

## 3DGS Few-shot Reconstruction

**Depth-Regularized Optimization for 3D Gaussian Splatting in Few-Shot Images**<br>
*Jaeyoung Chung, Jeongtaek Oh, Kyoung Mu Lee*<br>
arXiv preprint, 22 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.13398)]

**FSGS: Real-Time Few-shot View Synthesis using Gaussian Splatting**<br>
*Zehao Zhu, Zhiwen Fan, Yifan Jiang, Zhangyang Wang*<br>
arXiv preprint, 1 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.00451)] [[Project](https://zehaozhu.github.io/FSGS/)]

**Triplane Meets Gaussian Splatting: Fast and Generalizable Single-View 3D Reconstruction with Transformers**<br>
*Zi-Xin Zou, Zhipeng Yu, Yuan-Chen Guo, Yangguang Li, Ding Liang, Yan-Pei Cao, Song-Hai Zhang*<br>
arXiv preprint, 14 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.09147)] [[Project](https://zouzx.github.io/TriplaneGaussian/)] [[Code](https://github.com/VAST-AI-Research/TriplaneGaussian)]

**pixelSplat: 3D Gaussian Splats from Image Pairs for Scalable Generalizable 3D Reconstruction**<br>
*David Charatan, Sizhe Li, Andrea Tagliasacchi, Vincent Sitzmann*<br>
arXiv preprint, 19 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.12337)] [[Project](https://davidcharatan.com/pixelsplat/)] [[Code](https://github.com/dcharatan/pixelsplat)]

**AGG: Amortized Generative 3D Gaussians for Single Image to 3D**<br>
*Dejia Xu, Ye Yuan, Morteza Mardani, Sifei Liu, Jiaming Song, Zhangyang Wang, Arash Vahdat*<br>
arXiv preprint, 8 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.04099)] [[Project](https://ir1d.github.io/AGG/)]

**GaussianObject: Just Taking Four Images to Get A High-Quality 3D Object with Gaussian Splatting**<br>
*Chen Yang, Sikuang Li, Jiemin Fang, Ruofan Liang, Lingxi Xie, Xiaopeng Zhang, Wei Shen, Qi Tian*<br>
arXiv preprint, 15 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.10259)] [[Project](https://gaussianobject.github.io/)]

## 3DGS Weak Camera Pose

**COLMAP-Free 3D Gaussian Splatting**<br>
*Yang Fu, Sifei Liu, Amey Kulkarni, Jan Kautz, Alexei A. Efros, Xiaolong Wang*<br>
CVPR 2024, 12 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.07504)] [[Project](https://oasisyang.github.io/colmap-free-3dgs/)] [[Video](https://www.youtube.com/watch?si=kqu3dbXopDdNg0wX&v=mGeVQS4ExK4&feature=youtu.be)]

**iComMa: Inverting 3D Gaussians Splatting for Camera Pose Estimation via Comparing and Matching**<br>
*Yuan Sun, Xuan Wang, Yunfan Zhang, Jie Zhang, Caigui Jiang, Yu Guo, Fei Wang*<br>
arXiv preprint, 14 Dec 2023<br>
[[arXiv]https://arxiv.org/abs/2312.09031]

## 3DGS Indoor Scene Reconstruction

**360-GS: Layout-guided Panoramic Gaussian Splatting For Indoor Roaming**<br>
*Jiayang Bai, Letian Huang, Jie Guo, Wen Gong, Yuanqi Li, Yanwen Guo*<br>
arXiv preprint, 1 Feb 2024<br>
[[arXiv]](https://browse.arxiv.org/abs/2402.00763)

## 3DGS Based Large Scene Reconstruction
**Periodic Vibration Gaussian: Dynamic Urban Scene Reconstruction and Real-time Rendering**<br>
*Yurui Chen, Chun Gu, Junzhe Jiang, Xiatian Zhu, Li Zhang*<br>
arXiv preprint, 30 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.18561)] [[Project](https://fudan-zvg.github.io/PVG/)]

**GauU-Scene: A Scene Reconstruction Benchmark on Large Scale 3D Reconstruction Dataset Using Gaussian Splatting**<br>
*Butian Xiong, Zhuo Li, Zhen Li*<br>
arXiv preprint, 25 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.14032)]

**GaussianPro: 3D Gaussian Splatting with Progressive Propagation**<br>
*Kai Cheng, Xiaoxiao Long, Kaizhi Yang, Yao Yao, Wei Yin, Yuexin Ma, Wenping Wang, Xuejin Chen*<br>
arXiv preprint, 22 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.14650)] [[Project](https://kcheng1021.github.io/gaussianpro.github.io/)] [[Code](https://github.com/kcheng1021/GaussianPro)]

## 3DGS Autonomous Drivibng
**DrivingGaussian: Composite Gaussian Splatting for Surrounding Dynamic Autonomous Driving Scenes**<br>
*Xiaoyu Zhou, Zhiwei Lin, Xiaojun Shan, Yongtao Wang, Deqing Sun, Ming-Hsuan Yang*<br>
CVPR 2024, 13 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.07920)] [[Code](https://github.com/VDIGPKU/DrivingGaussian)]

**Street Gaussians for Modeling Dynamic Urban Scenes**<br>
*Yunzhi Yan, Haotong Lin, Chenxu Zhou, Weijie Wang, Haiyang Sun, Kun Zhan, Xianpeng Lang, Xiaowei Zhou, Sida Peng*<br>
arXiv preprint, 2 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.01339)] [[Project](https://zju3dv.github.io/street_gaussians/)] [[Code](https://github.com/zju3dv/street_gaussians)]

## 3DGS Based AIGC

**GaussianDiffusion: 3D Gaussian Splatting for Denoising Diffusion Probabilistic Models with Structured Noise**<br>
*Xinhai Li, Huaibin Wang, Kuo-Kun Tseng*<br>
arXiv preprint, 19 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.11221)]

**LucidDreamer: Towards High-Fidelity Text-to-3D Generation via Interval Score Matching**<br>
*Yixun Liang, Xin Yang, Jiantao Lin, Haodong Li, Xiaogang Xu, Yingcong Chen*<br>
arXiv preprint, 19 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.11284)] [[Github](https://github.com/EnVision-Research/LucidDreamer)]

**LucidDreamer: Domain-free Generation of 3D Gaussian Splatting Scenes**<br>
*Jaeyoung Chung, Suyoung Lee, Hyeongjin Nam, Jaerin Lee, Kyoung Mu Lee*<br>
arXiv preprint, 22 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.13384)] [[Project](https://luciddreamer-cvlab.github.io/)]

**DreamGaussian: Generative Gaussian Splatting for Efficient 3D Content Creation**<br>
*Jiaxiang Tang, Jiawei Ren, Hang Zhou, Ziwei Liu, Gang Zeng*<br>
arXiv preprint, 28 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.16653)] [[Project](https://dreamgaussian.github.io/)] [[Github](https://github.com/dreamgaussian/dreamgaussian)]

**Text-to-3D using Gaussian Splatting**<br>
*Zilong Chen, Feng Wang, Huaping Liu*<br>
arXiv preprint, 29 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.16585)] [[Project](https://gsgen3d.github.io/)] [[Github](https://github.com/gsgen3d/gsgen)]

**GaussianDreamer: Fast Generation from Text to 3D Gaussian Splatting with Point Cloud Priors**<br>
*Taoran Yi, Jiemin Fang, Guanjun Wu, Lingxi Xie, Xiaopeng Zhang, Wenyu Liu, Qi Tian, Xinggang Wang*<br>
arXiv preprint, 12 Oct 2023<br>
[[arXiv](https://arxiv.org/abs/2310.08529)] [[Project](https://taoranyi.com/gaussiandreamer/)] [[Github](https://github.com/hustvl/GaussianDreamer)]

**CG3D: Compositional Generation for Text-to-3D via Gaussian Splatting**<br>
*Alexander Vilesov, Pradyumna Chari, Achuta Kadambi*<br>
arXiv preprint, 29 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.17907)]

**Text2Immersion: Generative Immersive Scene with 3D Gaussians**<br>
*Hao Ouyang, Kathryn Heal, Stephen Lombardi, Tiancheng Sun*<br>
arXiv preprint, 14 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.09242)] [[Project](https://ken-ouyang.github.io/text2immersion/index.html)]

**Align Your Gaussians: Text-to-4D with Dynamic 3D Gaussians and Composed Diffusion Models**<br>
*Huan Ling, Seung Wook Kim, Antonio Torralba, Sanja Fidler, Karsten Kreis*<br>
CVPR 2024, 21 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.13763)] [[Project](https://research.nvidia.com/labs/toronto-ai/AlignYourGaussians/)]

:fire:**LangSplat: 3D Language Gaussian Splatting**<br>
*Minghan Qin, Wanhua Li, Jiawei Zhou, Haoqian Wang, Hanspeter Pfister*<br>
CVPR 2024, 26 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.16084)] [[Project](https://langsplat.github.io/)] [[Code](https://github.com/minghanqin/LangSplat)] [[Video](https://www.youtube.com/watch?v=XMlyjsei-Es)]

**4DGen: Grounded 4D Content Generation with Spatial-temporal Consistency**<br>
*Yuyang Yin, Dejia Xu, Zhangyang Wang, Yao Zhao, Yunchao Wei*<br>
arXiv preprint, 28 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.17225)] [[Project](https://vita-group.github.io/4DGen/)] [[Code](https://github.com/VITA-Group/4DGen)]


**DreamGaussian4D: Generative 4D Gaussian Splatting**<br>
*Jiawei Ren, Liang Pan, Jiaxiang Tang, Chi Zhang, Ang Cao, Gang Zeng, Ziwei Liu*<br>
arXiv preprint, 28 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.17142)] [[Project](https://jiawei-ren.github.io/projects/dreamgaussian4d/)] [[Code](https://github.com/jiawei-ren/dreamgaussian4d)]

**IM-3D: Iterative Multiview Diffusion and Reconstruction for High-Quality 3D Generation**<br>
*Luke Melas-Kyriazi, Iro Laina, Christian Rupprecht, Natalia Neverova, Andrea Vedaldi, Oran Gafni, Filippos Kokkinos*<br>
arXiv preprint, 13 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.08682)]

**GALA3D: Towards Text-to-3D Complex Scene Generation via Layout-guided Generative Gaussian Splatting**<br>
*Xiaoyu Zhou, Xingjian Ran, Yajiao Xiong, Jinlin He, Zhiwei Lin, Yongtao Wang, Deqing Sun, Ming-Hsuan Yang*<br>
arXiv preprint, 11 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.07207)]

## 3DGS Model Compactness Optimization

**LightGaussian: Unbounded 3D Gaussian Compression with 15x Reduction and 200+ FPS**<br>
*Zhiwen Fan, Kevin Wang, Kairun Wen, Zehao Zhu, Dejia Xu, Zhangyang Wang*<br>
arXiv preprint, 28 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.17245)] [[Project](https://lightgaussian.github.io/)] [[Video](https://www.bilibili.com/video/BV1QN4y127o9/)]

**Identifying Unnecessary 3D Gaussians using Clustering for Fast Rendering of 3D Gaussian Splatting**<br>
*Joongho Jo, Hyeongwon Kim, Jongsun Park*<br>
arXiv preprint, 21 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.13827)]


## 3DGS Avatar Generation

**Animatable 3D Gaussian: Fast and High-Quality Reconstruction of Multiple Human Avatars**<br>
*Yang Liu, Xiang Huang, Minghan Qin, Qinwei Lin, Haoqian Wang*<br>
arXiv preprint, 27 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16482)] [[Project](https://jimmyyliu.github.io/Animatable-3D-Gaussian/)]

**HumanGaussian: Text-Driven 3D Human Generation with Gaussian Splatting**<br>
*Xian Liu, Xiaohang Zhan, Jiaxiang Tang, Ying Shan, Gang Zeng, Dahua Lin, Xihui Liu, Ziwei Liu*<br>
arXiv preprint, 28 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.17061)] [[Project](https://alvinliu0.github.io/projects/HumanGaussian)]

**HUGS: Human Gaussian Splats**<br>
*Muhammed Kocabas, Jen-Hao Rick Chang, James Gabriel, Oncel Tuzel, Anurag Ranjan*<br>
arXiv preprint, 29 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.17910)]

**Gaussian Shell Maps for Efficient 3D Human Generation**<br>
*Rameen Abdal, Wang Yifan, Zifan Shi, Yinghao Xu, Ryan Po, Zhengfei Kuang, Qifeng Chen, Dit-Yan Yeung, Gordon Wetzstein*<br>
arXiv preprint, 29 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.17857)]

**GPS-Gaussian: Generalizable Pixel-wise 3D Gaussian Splatting for Real-time Human Novel View Synthesis**<br>
*Shunyuan Zheng, Boyao Zhou, Ruizhi Shao, Boning Liu, Shengping Zhang, Liqiang Nie, Yebin Liu*<br>
arXiv preprint, 4 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02155)] [[Project](https://shunyuanzheng.github.io/)]

**GaussianAvatar: Towards Realistic Human Avatar Modeling from a Single Video via Animatable 3D Gaussians**<br>
*Liangxiao Hu, Hongwen Zhang, Yuxiang Zhang, Boyao Zhou, Boning Liu, Shengping Zhang, Liqiang Nie*<br>
arXiv preprint, 4 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02134)] [[Project](https://huliangxiao.github.io/GaussianAvatar)]

**GaussianAvatars: Photorealistic Head Avatars with Rigged 3D Gaussians**<br>
*Shenhan Qian, Tobias Kirschstein, Liam Schoneveld, Davide Davoli, Simon Giebenhain, Matthias Nießner*<br>
arXiv preprint, 4 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02069)] [[Project](https://shenhanqian.github.io/gaussian-avatars)]

**GaussianHead: Impressive 3D Gaussian-based Head Avatars with Dynamic Hybrid Neural Field**<br>
*Jie Wang, Xianyan Li, Jiucheng Xie, Feng Xu, Hao Gao*<br>
arXiv preprint, 4 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.01632)]

**GauHuman: Articulated Gaussian Splatting from Monocular Human Videos**<br>
*Shoukang Hu, Ziwei Liu*<br>
CVPR 2024, 5 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02973)] [[Project](https://skhu101.github.io/GauHuman/)] [[Code](https://github.com/skhu101/GauHuman)]

**HeadGaS: Real-Time Animatable Head Avatars via 3D Gaussian Splatting**<br>
*Helisa Dhamo, Yinyu Nie, Arthur Moreau, Jifei Song, Richard Shaw, Yiren Zhou, Eduardo Pérez-Pellitero*<br>
arXiv preprint, 5 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02902)]

**Relightable Gaussian Codec Avatars**<br>
*Shunsuke Saito, Gabriel Schwartz, Tomas Simon, Junxuan Li, Giljoo Nam*<br>
CVPR 2024, 5 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.03704)] [[Project](https://shunsukesaito.github.io/rgca/)]

**HiFi4G: High-Fidelity Human Performance Rendering via Compact Gaussian Splatting**<br>
*Yuheng Jiang, Zhehao Shen, Penghao Wang, Zhuo Su, Yu Hong, Yingliang Zhang, Jingyi Yu, Lan Xu*<br>
arXiv preprint, 6 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.03461)]

**MonoGaussianAvatar: Monocular Gaussian Point-based Head Avatar**<br>
*Yufan Chen, Lizhen Wang, Qijing Li, Hongjiang Xiao, Shengping Zhang, Hongxun Yao, Yebin Liu*<br>
SIGGRAPH 2024, 7 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.04558)] [[Project](https://yufan1012.github.io/MonoGaussianAvatar)] [[Code](https://github.com/yufan1012/MonoGaussianAvatar)] [[Video](https://www.youtube.com/embed/3UvBkyPc-oc)]

**ASH: Animatable Gaussian Splats for Efficient and Photoreal Human Rendering**<br>
*Haokai Pang, Heming Zhu, Adam Kortylewski, Christian Theobalt, Marc Habermann*<br>
arXiv preprint, 10 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.05941)] [[Project](https://vcai.mpi-inf.mpg.de/projects/ash/)] [[Code](https://github.com/kv2000/ASH)]

**3DGS-Avatar: Animatable Avatars via Deformable 3D Gaussian Splatting**<br>
*Zhiyin Qian, Shaofei Wang, Marko Mihajlovic, Andreas Geiger, Siyu Tang*<br>
CVPR 2024, 14 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.09228)] [[Project](https://neuralbodies.github.io/3DGS-Avatar/)] [[Code](https://github.com/mikeqzy/3dgs-avatar-release)]

**GAvatar: Animatable 3D Gaussian Avatars with Implicit Mesh Learning**<br>
*Ye Yuan, Xueting Li, Yangyi Huang, Shalini De Mello, Koki Nagano, Jan Kautz, Umar Iqbal*<br>
CVPR 2024, 18 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.11461)] [[Project](https://nvlabs.github.io/GAvatar/)] [[Video](https://www.youtube.com/watch?v=PbCF1HzrKrs&feature=youtu.be)]

**3D Points Splatting for Real-Time Dynamic Hand Reconstruction**<br>
*Zheheng Jiang, Hossein Rahmani, Sue Black, Bryan M. Williams*<br>
arXiv preprint, 21 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.13770)]

**Human101: Training 100+FPS Human Gaussians in 100s from 1 View**<br>
*Mingwei Li, Jiachen Tao, Zongxin Yang, Yi Yang*<br>
arXiv preprint, 23 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.15258)] [[Code](https://github.com/longxiang-ai/Human101)]

**Gaussian Shadow Casting for Neural Characters**<br>
*Luis Bolanos, Shih-Yang Su, Helge Rhodin*<br>
arXiv preprint, 11 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.06116)]

**GPAvatar: Generalizable and Precise Head Avatar from Image(s)**<br>
*Xuangeng Chu, Yu Li, Ailing Zeng, Tianyu Yang, Lijian Lin, Yunfei Liu, Tatsuya Harada*<br>
ICLR 2024, 18 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.10215)] [[Code](https://github.com/xg-chu/GPAvatar)]

**PSAvatar: A Point-based Morphable Shape Model for Real-Time Head Avatar Creation with 3D Gaussian Splatting**<br>
*Zhongyuan Zhao, Zhenyu Bao, Qing Li, Guoping Qiu, Kanglin Liu*<br>
arXiv preprint, 23 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.12900)]

**ImplicitDeepfake: Plausible Face-Swapping through Implicit Deepfake Generation using NeRF and Gaussian Splatting**<br>
*Georgii Stanishevskii, Jakub Steczkiewicz, Tomasz Szczepanik, Sławomir Tadeja, Jacek Tabor, Przemysław Spurek*<br>
arXiv preprint, 9 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.06390)]

**GaussianHair: Hair Modeling and Rendering with Light-aware Gaussians**<br>
*Haimin Luo, Min Ouyang, Zijun Zhao, Suyi Jiang, Longwen Zhang, Qixuan Zhang, Wei Yang, Lan Xu, Jingyi Yu*<br>
arXiv preprint, 16 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.10483)]

**HeadStudio: Text to Animatable Head Avatars with 3D Gaussian Splatting**<br>
*Zhenglin Zhou, Fan Ma, Hehe Fan, Yi Yang*<br>
arXiv preprint, 9 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.06149)]

**Rig3DGS: Creating Controllable Portraits from Casual Monocular Videos**<br>
*Alfredo Rivero, ShahRukh Athar, Zhixin Shu, Dimitris Samaras*<br>
arXiv preprint, 6 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.03723)] [[Project](https://shahrukhathar.github.io/2024/02/05/Rig3DGS.html)]

## 3DGS Scene Editing and Animation

**Animatable 3D Gaussians for High-fidelity Synthesis of Human Motions**<br>
*Keyang Ye, Tianjia Shao, Kun Zhou*<br>
arXiv preprint, 22 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.13404)]

**GaussianEditor: Swift and Controllable 3D Editing with Gaussian Splatting**<br>
*Yiwen Chen, Zilong Chen, Chi Zhang, Feng Wang, Xiaofeng Yang, Yikai Wang, Zhongang Cai, Lei Yang, Huaping Liu, Guosheng Lin*<br>
arXiv preprint, 24 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.14521)] [[Project](https://buaacyw.github.io/gaussian-editor/)]

**Relightable 3D Gaussian: Real-time Point Cloud Relighting with BRDF Decomposition and Ray Tracing**<br>
*Jian Gao, Chun Gu, Youtian Lin, Hao Zhu, Xun Cao, Li Zhang, Yao Yao*<br>
arXiv preprint, 27 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16043)] [[Project](https://nju-3dv.github.io/projects/Relightable3DGaussian/)]

**GART: Gaussian Articulated Template Models**<br>
*Jiahui Lei, Yufu Wang, Georgios Pavlakos, Lingjie Liu, Kostas Daniilidis*<br>
arXiv preprint, 27 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16099)] [[Project](https://www.cis.upenn.edu/~leijh/projects/gart/)]

**Animatable Gaussians: Learning Pose-dependent Gaussian Maps for High-fidelity Human Avatar Modeling**<br>
*Zhe Li, Zerong Zheng, Lizhen Wang, Yebin Liu*<br>
arXiv preprint, 27 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16096)] [[Project](https://animatable-gaussians.github.io/)]

**Point'n Move: Interactive Scene Object Manipulation on Gaussian Splatting Radiance Fields**<br>
*Jiajun Huang, Hongchuan Yu*<br>
arXiv preprint, 28 Nov, 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16737)]

**TIP-Editor: An Accurate 3D Editor Following Both Text-Prompts And Image-Prompts**<br>
*Jingyu Zhuang, Di Kang, Yan-Pei Cao, Guanbin Li, Liang Lin, Ying Shan*<br>
SIGGRAPH 2024, 26 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.14828)]

## 3DGS for Computer Graphics

**PhysGaussian: Physics-Integrated 3D Gaussians for Generative Dynamics**<br>
*Tianyi Xie, Zeshun Zong, Yuxing Qiu, Xuan Li, Yutao Feng, Yin Yang, Chenfanfu Jiang*<br>
arXiv preprint, 20 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.12198)] [[Project](https://xpandora.github.io/PhysGaussian/)]

**Gaussian Splashing: Dynamic Fluid Synthesis with Gaussian Splatting**<br>
*Yutao Feng, Xiang Feng, Yintong Shang, Ying Jiang, Chang Yu, Zeshun Zong, Tianjia Shao, Hongzhi Wu, Kun Zhou, Chenfanfu Jiang, Yin Yang*<br>
arXiv preprint, 27 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.15318)] [[Project](https://amysteriouscat.github.io/GaussianSplashing/)] [[Video](https://www.youtube.com/watch?v=KgaR1ni-Egg&t=4s)]

**VR-GS: A Physical Dynamics-Aware Interactive Gaussian Splatting System in Virtual Reality**<br>
*Ying Jiang, Chang Yu, Tianyi Xie, Xuan Li, Yutao Feng, Huamin Wang, Minchen Li, Henry Lau, Feng Gao, Yin Yang, Chenfanfu Jiang*<br>
arXiv preprint, 30 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.16663)] [[Project](https://yingjiang96.github.io/VR-GS/)]

## 3DGS Based Scene Understanding

**Language Embedded 3D Gaussians for Open-Vocabulary Scene Understanding**<br>
*Jin-Chuan Shi, Miao Wang, Hao-Bin Duan, Shao-Hua Guan*<br>
arXiv preprint, 30 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.18482)]

**Semantic Anything in 3D Gaussians**<br>
*Xu Hu, Yuxi Wang, Lue Fan, Junsong Fan, Junran Peng, Zhen Lei, Qing Li, Zhaoxiang Zhang*<br>
arXiv preprint, 31 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.17857)]

## 3DGS Based SLAM

**SplaTAM: Splat, Track & Map 3D Gaussians for Dense RGB-D SLAM**<br>
*Nikhil Keetha, Jay Karhade, Krishna Murthy Jatavallabhula, Gengshan Yang, Sebastian Scherer, Deva Ramanan, Jonathon Luiten*<br>
arXiv preprint, 4 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02126)]

**LIV-GaussMap: LiDAR-Inertial-Visual Fusion for Real-time 3D Radiance Field Map Rendering**<br>
*Sheng Hong, Junjie He, Xinhu Zheng, Hesheng Wang, Hao Fang, Kangcheng Liu, Chunran Zheng, Shaojie Shen*<br>
arXiv preprint, 26 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.14857)]

**SGS-SLAM: Semantic Gaussian Splatting For Neural Dense SLAM**<br>
*Mingrui Li, Shuhong Liu, Heng Zhou*<br>
arXiv preprint, 5 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.03246)]

**MoD-SLAM: Monocular Dense Mapping for Unbounded 3D Scene Reconstruction**<br>
*Heng Zhou, Zhetao Guo, Shuhong Liu, Lechen Zhang, Qihao Wang, Yuxiang Ren, Mingrui Li*<br>
arXiv preprint, 6 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.03762)]

## 3DGS Based Inverse Rendering

**GIR: 3D Gaussian Inverse Rendering for Relightable Scene Factorization**<br>
*Yahao Shi, Yanmin Wu, Chenming Wu, Xing Liu, Chen Zhao, Haocheng Feng, Jingtuo Liu, Liangjun Zhang, Jian Zhang, Bin Zhou, Errui Ding, Jingdong Wang*<br>
arXiv preprint, 8 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.05133)] [[Project](https://3dgir.github.io/)]

## 3DGS Imaging Tasks

**Deblurring 3D Gaussian Splatting**<br>
*Byeonghyeon Lee, Howoong Lee, Xiangyu Sun, Usman Ali, Eunbyung Park*<br>
arXiv preprint, 1 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.00834)] [[Project](https://benhenryl.github.io/Deblurring-3D-Gaussian-Splatting/)] [[Code](https://github.com/benhenryL/Deblurring-3D-Gaussian-Splatting)]

## 3DGS Scene Understanding

**2D-Guided 3D Gaussian Segmentation**<br>
*Kun Lan, Haoran Li, Haolin Shi, Wenjun Wu, Yong Liao, Lin Wang, Pengyuan Zhou*<br>
arXiv preprint, 26 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.16047)]

**CoSSegGaussians: Compact and Swift Scene Segmenting 3D Gaussians**<br>
*Bin Dou, Tianyu Zhang, Yongjia Ma, Zhaohui Wang, Zejian Yuan*<br>
arXiv preprint, 11 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.05925)] [[Project](https://david-dou.github.io/CoSSegGaussians/)]

## 3DGS Applications

### 3DGS Application in Animal Reconstruction

**Exploring the Feasibility of Generating Realistic 3D Models of Endangered Species Using DreamGaussian: An Analysis of Elevation Angle's Impact on Model Generation**<br>
*Selcuk Anil Karatopak, Deniz Sen*<br>
arXiv preprint, 15 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.09682)]

### 3DGS Application in Medical Imaging

**EndoGaussian: Gaussian Splatting for Deformable Surgical Scene Reconstruction**<br>
*Yifan Liu, Chenxin Li, Chen Yang, Yixuan Yuan*<br>
arXiv preprint, 23 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.12561/)] [[Project](https://yifliu3.github.io/EndoGaussian/)] [[Code](https://github.com/yifliu3/EndoGaussian)]

**Deformable Endoscopic Tissues Reconstruction with Gaussian Splatting**<br>
*Lingting Zhu, Zhao Wang, Zhenchao Jin, Guying Lin, Lequan Yu*<br>
arXiv preprint, 21 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.11535)] [[Code](https://github.com/HKU-MedAI/EndoGS)]

**Endo-4DGS: Distilling Depth Ranking for Endoscopic Monocular Scene Reconstruction with 4D Gaussian Splatting**<br>
*Yiming Huang, Beilei Cui, Long Bai, Ziqi Guo, Mengya Xu, Hongliang Ren*<br>
arXiv preprint, 29 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.16416)]
