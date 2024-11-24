# <p align='center'>NeRF and Beyond Docs</p>

This is a collection of documents and topics NeRF/3DGS & Beyond channel accumulated, as well as papers in literaure. Since there are lots of papers out there, so we split them into two seperate repositories: [NeRF and Beyond Docs](https://github.com/yangjiheng/nerf_and_beyond_docs) and [3DGS and Beyond Docs](https://github.com/yangjiheng/3DGS_and_Beyond_Docs). Please choose accordingly recarding to your preference.

Some papers we discussed in the group, will be added to the back of the paper with a **Notes** link. You can follow the link to check whether there is topic you are interested in. If not, welcome to join us and ask the question to the crowd. The mighty community might have your answers.

We are actively maintaining this page trying to stay up-to-date and gather important works in a daily basis. We would also like to put as many notes as possible to some works, trying to make it easier to catch up. 

Please feel free to join us on WeChat group or start a discussion topic here.


## NeRF/3DGS Book

I have recently published a book with PHEI(Publishing House of Electronics Industry) on NeRF/3DGS. This would not have been possible without the help of the whole 3D vision community. It is now available on jd.com ([Checkout here](https://item.jd.com/10110615626932.html)) and it should be suitable as a reference handbook for NeRF/3DGS beginners or engineers in related areas. I sincerely hope the book can be helpful in any perspective. 

For those of you who have already purchased the book, all references can be downloaded [HERE](./assets/book_references.pdf). If you experience any issue reading the book or have any suggestions to improve it, please contact me through my email address: `jiheng.yang@gmail.com`, or directly concact me on WeChat: `jiheng_yang`. I'm looking forward to talk to anyone reaching out to me, thanks in advance.

<div style="text-align: center;">
  <img src="./assets/book_cover.jpeg" width="400">
</div>


## How to join us

For now, you can join us in the following ways

* [Bilibili Channel](https://space.bilibili.com/455056488) where we post near daily updates (primarily) on NeRF.
* WeChat group, due to the limitation of WeChat group, you can add my personal account: `jiheng_yang`, and I will add you to the chat groups.
* If you want to view this from a timeline perspective, please refer to this [ProcessOn Diagram](https://www.processon.com/view/link/643f8907f1144c215788f3e2)
* If you think something is not correct or you think we could do better in some way, please write to us through all possible channels or drop an issue. All suggestions are appreciated!
* For other discussed techniques that's related to 3D reconstruction and NeRF, please refer to [link](./NeRF_Related_Tech.md), we are constantly trying to add more resource to this document.
* We are trying to gradually setup Discord channels, join the [Discord Channel](https://discord.gg/AF2uMWGc) if you want to, we will certainly look forward to talk with you guys!

## 3DGS Progresses

For 3DGS related progress, you can refer to [3DGS and Beyond Docs](https://github.com/yangjiheng/3DGS_and_Beyond_Docs)

## NeRF progresses

<summary>Table of Content</summary>

- [NeRF and Beyond Docs](#nerf-and-beyond-docs)
  - [NeRF/3DGS Book](#nerf3dgs-book)
  - [How to join us](#how-to-join-us)
  - [3DGS Progresses](#3dgs-progresses)
  - [NeRF progresses](#nerf-progresses)
  - [New to NeRF](#new-to-nerf)
    - [Begin of NeRF, Always Start Here](#begin-of-nerf-always-start-here)
    - [NeRF Related Surveys](#nerf-related-surveys)
    - [NeRF Tutorials](#nerf-tutorials)
    - [NeRF Profiling](#nerf-profiling)
    - [NeRF OpenSource Tools](#nerf-opensource-tools)
  - [NeRF Fundamental Enhancements](#nerf-fundamental-enhancements)
  - [Depth Supervised Reconstruction](#depth-supervised-reconstruction)
  - [Activation Function Optimization](#activation-function-optimization)
  - [Positional Encoding](#positional-encoding)
  - [Deformable \& Dynamic NeRF](#deformable--dynamic-nerf)
  - [NeRF Training and Rendering Speed Enhancements](#nerf-training-and-rendering-speed-enhancements)
  - [One-Shot/Few-Shot Sparse View Reconstruction](#one-shotfew-shot-sparse-view-reconstruction)
  - [NeRF-3DGS Transfer](#nerf-3dgs-transfer)
  - [NeRF Based SLAM](#nerf-based-slam)
    - [NeRF SLAM Survey](#nerf-slam-survey)
    - [NeRF SLAM Progress](#nerf-slam-progress)
  - [Camera Pose Estimation \& Weak Camera Pose Reconstruction](#camera-pose-estimation--weak-camera-pose-reconstruction)
  - [NeRF with MVS](#nerf-with-mvs)
  - [NeRF AIGC](#nerf-aigc)
    - [NeRF AIGC Survey](#nerf-aigc-survey)
    - [NeRF AIGC Progresses](#nerf-aigc-progresses)
  - [Generalization](#generalization)
  - [Model Compression](#model-compression)
  - [NeRF Based 2D High Quality Image Synthesis](#nerf-based-2d-high-quality-image-synthesis)
  - [SDF Based Reconstruction / Other Geometry Based Reconstruction](#sdf-based-reconstruction--other-geometry-based-reconstruction)
  - [NeRF + Hardware Optimization/Acceleration](#nerf--hardware-optimizationacceleration)
  - [NeRF + Light Field Rendering](#nerf--light-field-rendering)
  - [NeRF + Point Cloud / LiDAR](#nerf--point-cloud--lidar)
  - [NeRF + Auto Data Collection](#nerf--auto-data-collection)
  - [NeRF + Avatar/Talking Head](#nerf--avatartalking-head)
  - [NeRF + Imaging Tasks](#nerf--imaging-tasks)
  - [NeRF + Super-resolution](#nerf--super-resolution)
  - [NeRF + Indoor Scenes](#nerf--indoor-scenes)
  - [NeRF + Large Scale Scenes \& Urban Scenes](#nerf--large-scale-scenes--urban-scenes)
  - [NeRF + Autonomous Driving](#nerf--autonomous-driving)
    - [NeRF Autonomous Driving Survey](#nerf-autonomous-driving-survey)
    - [NeRF Autonomous Driving Progress](#nerf-autonomous-driving-progress)
  - [NeRF + Editing](#nerf--editing)
  - [NeRF + Relighting](#nerf--relighting)
  - [NeRF + Open Surface Reconstruction and Cloth Simulation](#nerf--open-surface-reconstruction-and-cloth-simulation)
  - [NeRF + Segmentation](#nerf--segmentation)
  - [NeRF + Multi-Modal](#nerf--multi-modal)
    - [NeRF Multi-Modal Survey](#nerf-multi-modal-survey)
    - [NeRF Multi-Modal Progresses](#nerf-multi-modal-progresses)
  - [NeRF + Semantic/Understanding](#nerf--semanticunderstanding)
  - [NeRF + Mesh Extraction](#nerf--mesh-extraction)
  - [NeRF + Codec/Streaming](#nerf--codecstreaming)
  - [NeRF + Model Conversion](#nerf--model-conversion)
  - [NeRF + Medical/Biology](#nerf--medicalbiology)
  - [NeRF + Inverse Rendering](#nerf--inverse-rendering)
  - [NeRF + Texture Synthesis](#nerf--texture-synthesis)
  - [NeRF + Robotics](#nerf--robotics)
    - [NeRF Robotics Survey](#nerf-robotics-survey)
    - [NeRF Robotics Progresses](#nerf-robotics-progresses)
  - [NeRF + Transparent and Specular](#nerf--transparent-and-specular)
  - [Other 3D Generative Work](#other-3d-generative-work)
  - [NeRF + Other applications](#nerf--other-applications)
  - [NeRF + Gaming](#nerf--gaming)
  - [NeRF + Quality Metric](#nerf--quality-metric)
  - [NeRF + CAD](#nerf--cad)
  - [NeRF + GIS](#nerf--gis)
  - [NeRF + Terrain](#nerf--terrain)
  - [NeRF + Satellite Images / Radar](#nerf--satellite-images--radar)
  - [NeRF + UAV/Drone](#nerf--uavdrone)
  - [NeRF + Copyright protection and Security](#nerf--copyright-protection-and-security)
  - [NeRF + Motion Detection](#nerf--motion-detection)
  - [NeRF Defect Detection](#nerf-defect-detection)
  - [Datasets](#datasets)
  - [Neural Surface Reconstruction](#neural-surface-reconstruction)
  - [Other Important Related Work](#other-important-related-work)
    - [Depth Estimation](#depth-estimation)
    - [Diffusion Surveys](#diffusion-surveys)
  - [New Ideas](#new-ideas)
  - [Contributors](#contributors)
  - [License](#license)

## New to NeRF

### Begin of NeRF, Always Start Here

:fire:**NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis**<br>
*Ben Mildenhall, Pratul P. Srinivasan, Matthew Tancik, Jonathan T. Barron, Ravi Ramamoorthi, Ren Ng*<br>
ECCV 2020, 19 Mar 2020 <br>
<details span>
<summary><b>Abstract</b></summary>
We present a method that achieves state-of-the-art results for synthesizing novel views of complex scenes by optimizing an underlying continuous volumetric scene function using a sparse set of input views. Our algorithm represents a scene using a fully-connected (non-convolutional) deep network, whose input is a single continuous 5D coordinate (spatial location (x,y,z) and viewing direction (θ,ϕ)) and whose output is the volume density and view-dependent emitted radiance at that spatial location. We synthesize views by querying 5D coordinates along camera rays and use classic volume rendering techniques to project the output colors and densities into an image. Because volume rendering is naturally differentiable, the only input required to optimize our representation is a set of images with known camera poses. We describe how to effectively optimize neural radiance fields to render photorealistic novel views of scenes with complicated geometry and appearance, and demonstrate results that outperform prior work on neural rendering and view synthesis. View synthesis results are best viewed as videos, so we urge readers to view our supplementary video for convincing comparisons.
</details>

[[arXiv](https://arxiv.org/abs/2003.08934)] [[Project](https://www.matthewtancik.com/nerf)] [[Code](https://github.com/bmild/nerf)] [[PyTorch Impl](https://github.com/yenchenlin/nerf-pytorch)] [[Notes](./paper_discussions/NeRF.md)]<br>

### NeRF Related Surveys

:fire:**State of the Art on Neural Rendering**<br>
*Ayush Tewari, Ohad Fried, Justus Thies, Vincent Sitzmann, Stephen Lombardi, Kalyan Sunkavalli, Ricardo Martin-Brualla, Tomas Simon, Jason Saragih, Matthias Nießner, Rohit Pandey, Sean Fanello, Gordon Wetzstein, Jun-Yan Zhu, Christian Theobalt, Maneesh Agrawala, Eli Shechtman, Dan B Goldman, Michael Zollhöfer*<br>
ECCV 2020,8 Apr 2020<br>
<details span>
<summary><b>Abstract</b></summary>
Efficient rendering of photo-realistic virtual worlds is a long standing effort of computer graphics. Modern graphics techniques have succeeded in synthesizing photo-realistic images from hand-crafted scene representations. However, the automatic generation of shape, materials, lighting, and other aspects of scenes remains a challenging problem that, if solved, would make photo-realistic computer graphics more widely accessible. Concurrently, progress in computer vision and machine learning have given rise to a new approach to image synthesis and editing, namely deep generative models. Neural rendering is a new and rapidly emerging field that combines generative machine learning techniques with physical knowledge from computer graphics, e.g., by the integration of differentiable rendering into network training. With a plethora of applications in computer graphics and vision, neural rendering is poised to become a new area in the graphics community, yet no survey of this emerging field exists. This state-of-the-art report summarizes the recent trends and applications of neural rendering. We focus on approaches that combine classic computer graphics techniques with deep generative models to obtain controllable and photo-realistic outputs. Starting with an overview of the underlying computer graphics and machine learning concepts, we discuss critical aspects of neural rendering approaches. This state-of-the-art report is focused on the many important use cases for the described algorithms such as novel view synthesis, semantic photo manipulation, facial and body reenactment, relighting, free-viewpoint video, and the creation of photo-realistic avatars for virtual and augmented reality telepresence. Finally, we conclude with a discussion of the social implications of such technology and investigate open research problems.
</details>

[[arXiv](https://arxiv.org/abs/2004.03805)]<br>

:fire:**Advances in Neural Rendering**<br>
*Ayush Tewari, Justus Thies, Ben Mildenhall, Pratul Srinivasan, Edgar Tretschk, Yifan Wang, Christoph Lassner, Vincent Sitzmann, Ricardo Martin-Brualla, Stephen Lombardi, Tomas Simon, Christian Theobalt, Matthias Niessner, Jonathan T. Barron, Gordon Wetzstein, Michael Zollhoefer, Vladislav Golyanik*<br>
ECCV 2022, 10 Nov 2021<br>
<details span>
<summary><b>Abstract</b></summary>
Synthesizing photo-realistic images and videos is at the heart of computer graphics and has been the focus of decades of research. Traditionally, synthetic images of a scene are generated using rendering algorithms such as rasterization or ray tracing, which take specifically defined representations of geometry and material properties as input. Collectively, these inputs define the actual scene and what is rendered, and are referred to as the scene representation (where a scene consists of one or more objects). Example scene representations are triangle meshes with accompanied textures (e.g., created by an artist), point clouds (e.g., from a depth sensor), volumetric grids (e.g., from a CT scan), or implicit surface functions (e.g., truncated signed distance fields). The reconstruction of such a scene representation from observations using differentiable rendering losses is known as inverse graphics or inverse rendering. Neural rendering is closely related, and combines ideas from classical computer graphics and machine learning to create algorithms for synthesizing images from real-world observations. Neural rendering is a leap forward towards the goal of synthesizing photo-realistic image and video content. In recent years, we have seen immense progress in this field through hundreds of publications that show different ways to inject learnable components into the rendering pipeline. This state-of-the-art report on advances in neural rendering focuses on methods that combine classical rendering principles with learned 3D scene representations, often now referred to as neural scene representations. A key advantage of these methods is that they are 3D-consistent by design, enabling applications such as novel viewpoint synthesis of a captured scene. In addition to methods that handle static scenes, we cover neural scene representations for modeling non-rigidly deforming objects...
</details>

[[arXiv](https://arxiv.org/abs/2111.05849)]<br>

:fire:**NeRF: Neural Radiance Field in 3D Vision, A Comprehensive Review**<br>
*Kyle Gao, Yina Gao, Hongjie He, Dening Lu, Linlin Xu, Jonathan Li*<br>
TPAMI 2022, 1 Oct 2022<br>
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Field (NeRF) has recently become a significant development in the field of Computer Vision, allowing for implicit, neural network-based scene representation and novel view synthesis. NeRF models have found diverse applications in robotics, urban mapping, autonomous navigation, virtual reality/augmented reality, and more. Due to the growing popularity of NeRF and its expanding research area, we present a comprehensive survey of NeRF papers from the past two years. Our survey is organized into architecture and application-based taxonomies and provides an introduction to the theory of NeRF and its training via differentiable volume rendering. We also present a benchmark comparison of the performance and speed of key NeRF models. By creating this survey, we hope to introduce new researchers to NeRF, provide a helpful reference for influential works in this field, as well as motivate future research directions with our discussion section.
</details>

[[arXiv](https://arxiv.org/abs/2210.00379)]<br>

**Neural Radiance Fields: Past, Present, and Future**<br>
*Ansh Mittal*<br>
In Progress,20 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.10050)]

**Survey on Fundamental Deep Learning 3D Reconstruction Techniques**<br>
*Yonge Bai, LikHang Wong, TszYin Twan*<br>
arXiv preprint, 11 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.08137)]

**3D Representation Methods: A Survey**<br>
*Zhengren Wang*<br>
arXiv preprint, 9 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.06475)]

### NeRF Tutorials

:fire:**Neural Rendering Course**<br>
SIGGRAPH 2021 [[BiliBili](https://www.bilibili.com/video/BV1B3411q7hy)]

:fire:**Neural Volumetric Rendering for Computer Vision**<br>
ECCV 2022 Tutorial [[Website](https://sites.google.com/berkeley.edu/nerf-tutorial/home)]

:fire:**Scaling NeRF Up and Down: Big Scenes and Real-Time View Synthesis**<br>
I3D 2023 Keynote [[Video](https://www.bilibili.com/video/BV1fh4y1t7rW/)]

### NeRF Profiling

**NerfBaselines: Consistent and Reproducible Evaluation of Novel View Synthesis Methods**<br>
*Jonas Kulhanek, Torsten Sattler*<br>
arXiv preprint, 25 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.17345)] [[Project](https://jkulhanek.com/nerfbaselines/)]

### NeRF OpenSource Tools

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

## NeRF Fundamental Enhancements

:fire:**NeRF in the Wild: Neural Radiance Fields for Unconstrained Photo Collections**<br>
*Ricardo Martin-Brualla, Noha Radwan, Mehdi S. M. Sajjadi, Jonathan T. Barron, Alexey Dosovitskiy, Daniel Duckworth*<br>
CVPR 2021, 5 Aug 2020 <br>
<details span>
<summary><b>Abstract</b></summary>
We present a learning-based method for synthesizing novel views of complex scenes using only unstructured collections of in-the-wild photographs. We build on Neural Radiance Fields (NeRF), which uses the weights of a multilayer perceptron to model the density and color of a scene as a function of 3D coordinates. While NeRF works well on images of static subjects captured under controlled settings, it is incapable of modeling many ubiquitous, real-world phenomena in uncontrolled images, such as variable illumination or transient occluders. We introduce a series of extensions to NeRF to address these issues, thereby enabling accurate reconstructions from unstructured image collections taken from the internet. We apply our system, dubbed NeRF-W, to internet photo collections of famous landmarks, and demonstrate temporally consistent novel view renderings that are significantly closer to photorealism than the prior state of the art.
</details>

[[arXiv](https://arxiv.org/abs/2008.02268)] [[Project](https://nerf-w.github.io/)]<br>

:fire:**Mip-NeRF: A Multiscale Representation for Anti-Aliasing Neural Radiance Fields**<br>
*Jonathan T. Barron, Ben Mildenhall, Matthew Tancik, Peter Hedman, Ricardo Martin-Brualla, Pratul P. Srinivasan*<br>
ICCV 2021, 24 Mar 2021<br>
<details span>
<summary><b>Abstract</b></summary>
The rendering procedure used by neural radiance fields (NeRF) samples a scene with a single ray per pixel and may therefore produce renderings that are excessively blurred or aliased when training or testing images observe scene content at different resolutions. The straightforward solution of supersampling by rendering with multiple rays per pixel is impractical for NeRF, because rendering each ray requires querying a multilayer perceptron hundreds of times. Our solution, which we call "mip-NeRF" (a la "mipmap"), extends NeRF to represent the scene at a continuously-valued scale. By efficiently rendering anti-aliased conical frustums instead of rays, mip-NeRF reduces objectionable aliasing artifacts and significantly improves NeRF's ability to represent fine details, while also being 7% faster than NeRF and half the size. Compared to NeRF, mip-NeRF reduces average error rates by 17% on the dataset presented with NeRF and by 60% on a challenging multiscale variant of that dataset that we present. Mip-NeRF is also able to match the accuracy of a brute-force supersampled NeRF on our multiscale dataset while being 22x faster.
</details>

[[arXiv](https://arxiv.org/abs/2103.13415)] [[Project](http://jonbarron.info/mipnerf)] [[Github](https://github.com/google/mipnerf)] [[Notes](./paper_discussions/mipnerf.md)]<br>

:fire:**Mip-NeRF 360: Unbounded Anti-Aliased Neural Radiance Fields**<br>
*Jonathan T. Barron, Ben Mildenhall, Dor Verbin, Pratul P. Srinivasan, Peter Hedman*<br>
CVPR 2022, 23 Nov 2021<br>
<details span>
<summary><b>Abstract</b></summary>
Though neural radiance fields (NeRF) have demonstrated impressive view synthesis results on objects and small bounded regions of space, they struggle on "unbounded" scenes, where the camera may point in any direction and content may exist at any distance. In this setting, existing NeRF-like models often produce blurry or low-resolution renderings (due to the unbalanced detail and scale of nearby and distant objects), are slow to train, and may exhibit artifacts due to the inherent ambiguity of the task of reconstructing a large scene from a small set of images. We present an extension of mip-NeRF (a NeRF variant that addresses sampling and aliasing) that uses a non-linear scene parameterization, online distillation, and a novel distortion-based regularizer to overcome the challenges presented by unbounded scenes. Our model, which we dub "mip-NeRF 360" as we target scenes in which the camera rotates 360 degrees around a point, reduces mean-squared error by 57% compared to mip-NeRF, and is able to produce realistic synthesized views and detailed depth maps for highly intricate, unbounded real-world scenes.
</details>

[[arXiv](https://arxiv.org/abs/2111.12077)] [[Project](https://jonbarron.info/mipnerf360/)] [[Github](https://github.com/google-research/multinerf)] [[Notes](./paper_discussions/mipnerf360.md)]<br>

:fire:**Ref-NeRF: Structured View-Dependent Appearance for Neural Radiance Fields**<br>
*Dor Verbin, Peter Hedman, Ben Mildenhall, Todd Zickler, Jonathan T. Barron, Pratul P. Srinivasan*<br>
CVPR 2022, 7 Dec 2021<br>
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Fields (NeRF) is a popular view synthesis technique that represents a scene as a continuous volumetric function, parameterized by multilayer perceptrons that provide the volume density and view-dependent emitted radiance at each location. While NeRF-based techniques excel at representing fine geometric structures with smoothly varying view-dependent appearance, they often fail to accurately capture and reproduce the appearance of glossy surfaces. We address this limitation by introducing Ref-NeRF, which replaces NeRF's parameterization of view-dependent outgoing radiance with a representation of reflected radiance and structures this function using a collection of spatially-varying scene properties. We show that together with a regularizer on normal vectors, our model significantly improves the realism and accuracy of specular reflections. Furthermore, we show that our model's internal representation of outgoing radiance is interpretable and useful for scene editing.
</details>

[[arXiv](https://arxiv.org/abs/2112.03907)] [[Project](https://dorverbin.github.io/refnerf/)] [[Github](https://github.com/google-research/multinerf)]<br>

:fire:**PS-NeRF: Neural Inverse Rendering for Multi-view Photometric Stereo**<br>
*Wenqi Yang, Guanying Chen, Chaofeng Chen, Zhenfang Chen, Kwan-Yee K. Wong*<br>
ECCV 2022, 23 Jul 2022<br>
<details span>
<summary><b>Abstract</b></summary>
Traditional multi-view photometric stereo (MVPS) methods are often composed of multiple disjoint stages, resulting in noticeable accumulated errors. In this paper, we present a neural inverse rendering method for MVPS based on implicit representation. Given multi-view images of a non-Lambertian object illuminated by multiple unknown directional lights, our method jointly estimates the geometry, materials, and lights. Our method first employs multi-light images to estimate per-view surface normal maps, which are used to regularize the normals derived from the neural radiance field. It then jointly optimizes the surface normals, spatially-varying BRDFs, and lights based on a shadow-aware differentiable rendering layer. After optimization, the reconstructed object can be used for novel-view rendering, relighting, and material editing. Experiments on both synthetic and real datasets demonstrate that our method achieves far more accurate shape reconstruction than existing MVPS and neural rendering methods. Our code and model can be found at this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2207.11406)] [[Project](https://ywq.github.io/psnerf/)] [[Github](https://github.com/ywq/psnerf)]<br>

**4K-NeRF: High Fidelity Neural Radiance Fields at Ultra High Resolutions**<br>
*Zhongshu Wang, Lingzhi Li, Zhen Shen, Li Shen, Liefeng Bo*<br>
arXiv preprint, 9 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.04701)] [[Project](https://frozoul.github.io/4knerf/)] [[Github](https://github.com/frozoul/4K-NeRF)]

:fire:**Zip-NeRF: Anti-Aliased Grid-Based Neural Radiance Fields**<br>
*Jonathan T. Barron, Ben Mildenhall, Dor Verbin, Pratul P. Srinivasan, Peter Hedman*<br>
arXiv preprint, 13 Apr 2023<br>
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Field training can be accelerated through the use of grid-based representations in NeRF's learned mapping from spatial coordinates to colors and volumetric density. However, these grid-based approaches lack an explicit understanding of scale and therefore often introduce aliasing, usually in the form of jaggies or missing scene content. Anti-aliasing has previously been addressed by mip-NeRF 360, which reasons about sub-volumes along a cone rather than points along a ray, but this approach is not natively compatible with current grid-based techniques. We show how ideas from rendering and signal processing can be used to construct a technique that combines mip-NeRF 360 and grid-based models such as Instant NGP to yield error rates that are 8% - 77% lower than either prior technique, and that trains 24x faster than mip-NeRF 360.
</details>

[[arXiv](https://arxiv.org/abs/2304.06706)] [[Project](https://jonbarron.info/zipnerf/)] [[Unofficial Impl](https://github.com/SuLvXiangXin/zipnerf-pytorch)] [[Notes](./paper_discussions/Zip-NeRF.md)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
Despite the tremendous progress in neural radiance fields (NeRF), we still face a dilemma of the trade-off between quality and efficiency, e.g., MipNeRF presents fine-detailed and anti-aliased renderings but takes days for training, while Instant-ngp can accomplish the reconstruction in a few minutes but suffers from blurring or aliasing when rendering at various distances or resolutions due to ignoring the sampling area. To this end, we propose a novel Tri-Mip encoding that enables both instant reconstruction and anti-aliased high-fidelity rendering for neural radiance fields. The key is to factorize the pre-filtered 3D feature spaces in three orthogonal mipmaps. In this way, we can efficiently perform 3D area sampling by taking advantage of 2D pre-filtered feature maps, which significantly elevates the rendering quality without sacrificing efficiency. To cope with the novel Tri-Mip representation, we propose a cone-casting rendering technique to efficiently sample anti-aliased 3D features with the Tri-Mip encoding considering both pixel imaging and observing distance. Extensive experiments on both synthetic and real-world datasets demonstrate our method achieves state-of-the-art rendering quality and reconstruction speed while maintaining a compact representation that reduces 25% model size compared against Instant-ngp.
</details>

[[arXiv](https://arxiv.org/abs/2307.11335)] [[Project](https://wbhu.github.io/projects/Tri-MipRF/)] [[Video](https://www.bilibili.com/video/BV1Lu41157Yj/)]<br>

**Bayes' Rays: Uncertainty Quantification for Neural Radiance Fields**<br>
*Lily Goli, Cody Reading, Silvia Selllán, Alec Jacobson, Andrea Tagliasacchi*<br>
arXiv preprint, 6 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.03185)] [[Project](https://bayesrays.github.io/)]

**ResFields: Residual Neural Fields for Spatiotemporal Signals**<br>
*Marko Mihajlovic, Sergey Prokudin, Marc Pollefeys, Siyu Tang*<br>
arXiv preprint, 1 Oct 2023
[[arXiv](https://arxiv.org/abs/2309.03160#)] [[Project](https://markomih.github.io/ResFields/)] [[Github](https://github.com/markomih/ResFields)]

:fire:**NeuRBF: A Neural Fields Representation with Adaptive Radial Basis Functions**<br>
*Zhang Chen, Zhong Li, Liangchen Song, Lele Chen, Jingyi Yu, Junsong Yuan, Yi Xu*<br>
ICCV 2023, 27 Sep 2023<br>
<details span>
<summary><b>Abstract</b></summary>
We present a novel type of neural fields that uses general radial bases for signal representation. State-of-the-art neural fields typically rely on grid-based representations for storing local neural features and N-dimensional linear kernels for interpolating features at continuous query points. The spatial positions of their neural features are fixed on grid nodes and cannot well adapt to target signals. Our method instead builds upon general radial bases with flexible kernel position and shape, which have higher spatial adaptivity and can more closely fit target signals. To further improve the channel-wise capacity of radial basis functions, we propose to compose them with multi-frequency sinusoid functions. This technique extends a radial basis to multiple Fourier radial bases of different frequency bands without requiring extra parameters, facilitating the representation of details. Moreover, by marrying adaptive radial bases with grid-based ones, our hybrid combination inherits both adaptivity and interpolation smoothness. We carefully designed weighting schemes to let radial bases adapt to different types of signals effectively. Our experiments on 2D image and 3D signed distance field representation demonstrate the higher accuracy and compactness of our method than prior arts. When applied to neural radiance field reconstruction, our method achieves state-of-the-art rendering quality, with small model size and comparable training speed.
</details>

[[arXiv](https://arxiv.org/abs/2309.15426)] [[Project](https://oppo-us-research.github.io/NeuRBF-website/)] [[Github](https://github.com/oppo-us-research/NeuRBF)]<br>

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

**Methods and strategies for improving the novel view synthesis quality of neural radiation field**<br>
*Shun Fang, Ming Cui, Xing Feng, Yanna Lv*<br>
arXiv preprint, 23 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.12451)]

**Divide and Conquer: Rethinking the Training Paradigm of Neural Radiance Fields**<br>
*Rongkai Ma, Leo Lebrat, Rodrigo Santa Cruz, Gil Avraham, Yan Zuo, Clinton Fookes, Olivier Salvado*<br>
arXiv preprint, 29 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.16144)]

**TaylorGrid: Towards Fast and High-Quality Implicit Field Learning via Direct Taylor-based Grid Optimization**<br>
*Renyi Mao, Qingshan Xu, Peng Zheng, Ye Wang, Tieru Wu, Rui Ma*<br>
arXiv preprint, 22 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.14415)]

**Mip-Grid: Anti-aliased Grid Representations for Neural Radiance Fields**<br>
*Seungtae Nam, Daniel Rho, Jong Hwan Ko, Eunbyung Park*<br>
NeurIPS 2023, 22 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.14196)] [[Project](https://stnamjef.github.io/mipgrid.github.io/)] [[Code](https://github.com/stnamjef/MipGrid)]

**NeRF-VPT: Learning Novel View Representations with Neural Radiance Fields via View Prompt Tuning**<br>
*Linsheng Chen, Guangrun Wang, Liuchun Yuan, Keze Wang, Ken Deng, Philip H.S. Torr*<br>
AAAI 2024, 2 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.01325)] [[Code](https://github.com/Freedomcls/NeRF-VPT)]

**RoGUENeRF: A Robust Geometry-Consistent Universal Enhancer for NeRF**<br>
*Sibi Catley-Chandar, Richard Shaw, Gregory Slabaugh, Eduardo Perez-Pellitero*<br>
arXiv preprint, 18 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.11909)]

**Mesh2NeRF: Direct Mesh Supervision for Neural Radiance Field Representation and Generation**<br>
*Yujin Chen, Yinyu Nie, Benjamin Ummenhofer, Reiner Birkl, Michael Paulitsch, Matthias Müller, Matthias Nießner*<br>
arXiv preprint, 28 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.19319)] [[Project](https://terencecyj.github.io/projects/Mesh2NeRF/)] [[Video](https://youtu.be/oufv1N3f7iY)]

**Sine Activated Low-Rank Matrices for Parameter Efficient Learning**<br>
*Yiping Ji, Hemanth Saratchandran, Cameron Gordon, Zeyu Zhang, Simon Lucey*<br>
arXiv preprint, 28 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.19243)]

**Neural Radiance Fields with Torch Units**<br>
*Bingnan Ni, Huanyu Wang, Dongfeng Bai, Minghe Weng, Dexin Qi, Weichao Qiu, Bingbing Liu*<br>
arXiv preprint, 3 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.02617)]

**Alpha Invariance: On Inverse Scaling Between Distance and Volume Density in Neural Radiance Fields**<br>
*Joshua Ahn, Haochen Wang, Raymond A. Yeh, Greg Shakhnarovich*<br>
CVPR 2024, 2 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.02155)] [[Project](https://pals.ttic.edu/p/alpha-invariance)]

**RaFE: Generative Radiance Fields Restoration**<br>
*Zhongkai Wu, Ziyu Wan, Jing Zhang, Jing Liao, Dong Xu*<br>
arXiv preprint, 4 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.03654)] [[Project](https://zkaiwu.github.io/RaFE-Project/)] [[Code](https://zkaiwu.github.io/RaFE-Project/)] [[Video](https://www.youtube.com/embed/LHAFASRjc1A)]

**Bayesian NeRF: Quantifying Uncertainty with Volume Density in Neural Radiance Fields**<br>
*Sibeak Lee, Kyeongsu Kang, Hyeonwoo Yu*<br>
arXiv preprint, 10 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.06727)]

:fire:**Rip-NeRF: Anti-aliasing Radiance Fields with Ripmap-Encoded Platonic Solids**<br>
*Junchen Liu, Wenbo Hu, Zhuo Yang, Jianteng Chen, Guoliang Wang, Xiaoxue Chen, Yantong Cai, Huan-ang Gao, Hao Zhao*<br>
SIGGRAPH 2024, 3 May 2024<br>
<details span>
<summary><b>Abstract</b></summary>
Despite significant advancements in Neural Radiance Fields (NeRFs), the renderings may still suffer from aliasing and blurring artifacts, since it remains a fundamental challenge to effectively and efficiently characterize anisotropic areas induced by the cone-casting procedure. This paper introduces a Ripmap-Encoded Platonic Solid representation to precisely and efficiently featurize 3D anisotropic areas, achieving high-fidelity anti-aliasing renderings. Central to our approach are two key components: Platonic Solid Projection and Ripmap encoding. The Platonic Solid Projection factorizes the 3D space onto the unparalleled faces of a certain Platonic solid, such that the anisotropic 3D areas can be projected onto planes with distinguishable characterization. Meanwhile, each face of the Platonic solid is encoded by the Ripmap encoding, which is constructed by anisotropically pre-filtering a learnable feature grid, to enable featurzing the projected anisotropic areas both precisely and efficiently by the anisotropic area-sampling. Extensive experiments on both well-established synthetic datasets and a newly captured real-world dataset demonstrate that our Rip-NeRF attains state-of-the-art rendering quality, particularly excelling in the fine details of repetitive structures and textures, while maintaining relatively swift training times.
</details>

[[arXiv](https://arxiv.org/abs/2405.02386)] [[Project](https://junchenliu77.github.io/Rip-NeRF)] [[Code](https://github.com/JunchenLiu77/Rip-NeRF)] [[Video](https://www.youtube.com/watch?v=VeZTbQwMFRs)]<br>

**DistGrid: Scalable Scene Reconstruction with Distributed Multi-resolution Hash Grid**<br>
*Sidun Liu, Peng Qiao, Zongxin Ye, Wenyu Li, Yong Dou*<br>
Siggraph Asia 2023, 7 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.04416)]

**NPLMV-PS: Neural Point-Light Multi-View Photometric Stereo**<br>
*Fotios Logothetis, Ignas Budvytis, Roberto Cipolla*<br>
arXiv preprint, 20 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.12057)]

**PruNeRF: Segment-Centric Dataset Pruning via 3D Spatial Consistency**<br>
*Yeonsung Jung, Heecheol Yun, Joonhyung Park, Jin-Hwa Kim, Eunho Yang*<br>
arXiv preprint, 2 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.00798)]

**NeRF Director: Revisiting View Selection in Neural Volume Rendering**<br>
*Wenhui Xiao, Rodrigo Santa Cruz, David Ahmedt-Aristizabal, Olivier Salvado, Clinton Fookes, Leo Lebrat*<br>
CVPR 2024, 13 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.08839)]

**InterNeRF: Scaling Radiance Fields via Parameter Interpolation**<br>
*Clinton Wang, Peter Hedman, Polina Golland, Jonathan T. Barron, Daniel Duckworth*<br>
CVPR 2024 Neural Rendering Intelligence Workshop, 17 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.11737)]

**Uncertainty modeling for fine-tuned implicit functions**<br>
*Anna Susmelj, Mael Macuglia, Nataša Tagasovska, Reto Sutter, Sebastiano Caprara, Jean-Philippe Thiran, Ender Konukoglu*<br>
arXiv preprint, 17 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.12082)]

**Matching Query Image Against Selected NeRF Feature for Efficient and Scalable Localization**<br>
*Huaiji Zhou, Bing Wang, Changhao Chen*<br>
arXiv preprint, 17 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.11766)]

**Federated Neural Radiance Field for Distributed Intelligence**<br>
*Yintian Zhang, Ziyu Shao*<br>
arXiv preprint, 15 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.10474)]

**Drantal-NeRF: Diffusion-Based Restoration for Anti-aliasing Neural Radiance Field**<br>
*Ganlin Yang, Kaidong Zhang, Jingjing Fu, Dong Liu*<br>
arXiv preprint, 10 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.07461)]

**RS-NeRF: Neural Radiance Fields from Rolling Shutter Images**<br>
*Muyao Niu, Tong Chen, Yifan Zhan, Zhuoxiao Li, Xiang Ji, Yinqiang Zheng*<br>
ECCV 2024, 14 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.10267)] [[Code](https://github.com/MyNiuuu/RS-NeRF)]

**Efficient NeRF Optimization -- Not All Samples Remain Equally Hard**<br>
*Juuso Korhonen, Goutham Rangu, Hamed R. Tavakoli, Juho Kannala*<br>
arXiv preprint, 6 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.03193)]

**Magnituder Layers for Implicit Neural Representations in 3D**<br>
*Sang Min Kim, Byeongchan Kim, Arijit Sehanobish Krzysztof Choromanski, Dongseok Shim, Avinava Dubey, Min-hwan Oh*<br>
arXiv preprint, 13 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.09771)]

**Bringing NeRFs to the Latent Space: Inverse Graphics Autoencoder**<br>
*Antoine Schnepf, Karim Kassab, Jean-Yves Franceschi, Laurent Caraffa, Flavian Vasile, Jeremie Mary, Andrew Comport, Valerie Gouet-Brunet*<br>
arXiv preprint, 30 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.22936)] [[Project](https://ig-ae.github.io/)]
 

## Depth Supervised Reconstruction

:fire:**Depth-supervised NeRF: Fewer Views and Faster Training for Free**<br>
*Kangle Deng, Andrew Liu, Jun-Yan Zhu, Deva Ramanan*<br>
CVPR 2022, 6 Jul 2021<br>
<details span>
<summary><b>Abstract</b></summary>
A commonly observed failure mode of Neural Radiance Field (NeRF) is fitting incorrect geometries when given an insufficient number of input views. One potential reason is that standard volumetric rendering does not enforce the constraint that most of a scene's geometry consist of empty space and opaque surfaces. We formalize the above assumption through DS-NeRF (Depth-supervised Neural Radiance Fields), a loss for learning radiance fields that takes advantage of readily-available depth supervision. We leverage the fact that current NeRF pipelines require images with known camera poses that are typically estimated by running structure-from-motion (SFM). Crucially, SFM also produces sparse 3D points that can be used as "free" depth supervision during training: we add a loss to encourage the distribution of a ray's terminating depth matches a given 3D keypoint, incorporating depth uncertainty. DS-NeRF can render better images given fewer training views while training 2-3x faster. Further, we show that our loss is compatible with other recently proposed NeRF methods, demonstrating that depth is a cheap and easily digestible supervisory signal. And finally, we find that DS-NeRF can support other types of depth supervision such as scanned depth sensors and RGB-D reconstruction outputs.
</details>

[[arXiv](https://arxiv.org/abs/2107.02791)] [[Project](http://www.cs.cmu.edu/~dsnerf/)] [[Github](https://github.com/dunbar12138/DSNeRF)]<br>

:fire:**NerfingMVS: Guided Optimization of Neural Radiance Fields for Indoor Multi-view Stereo**<br>
*Yi Wei, Shaohui Liu, Yongming Rao, Wang Zhao, Jiwen Lu, Jie Zhou*<br>
ICCV 2021, 2 Sep 2021<br>
<details span>
<summary><b>Abstract</b></summary>
In this work, we present a new multi-view depth estimation method that utilizes both conventional reconstruction and learning-based priors over the recently proposed neural radiance fields (NeRF). Unlike existing neural network based optimization method that relies on estimated correspondences, our method directly optimizes over implicit volumes, eliminating the challenging step of matching pixels in indoor scenes. The key to our approach is to utilize the learning-based priors to guide the optimization process of NeRF. Our system firstly adapts a monocular depth network over the target scene by finetuning on its sparse SfM+MVS reconstruction from COLMAP. Then, we show that the shape-radiance ambiguity of NeRF still exists in indoor environments and propose to address the issue by employing the adapted depth priors to monitor the sampling process of volume rendering. Finally, a per-pixel confidence map acquired by error computation on the rendered image can be used to further improve the depth quality. Experiments show that our proposed framework significantly outperforms state-of-the-art methods on indoor scenes, with surprising findings presented on the effectiveness of correspondence-based optimization and NeRF-based optimization over the adapted depth priors. In addition, we show that the guided optimization scheme does not sacrifice the original synthesis capability of neural radiance fields, improving the rendering quality on both seen and novel views. Code is available at this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2109.01129)] [[Project](https://weiyithu.github.io/NerfingMVS)] [[Github](https://github.com/weiyithu/NerfingMVS)]<br>

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
AAAI 2024, 19 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.10001)]

**Depth Supervised Neural Surface Reconstruction from Airborne Imagery**<br>
*Vincent Hackstein, Paul Fauth-Mayer, Matthias Rothermel, Norbert Haala*<br>
arXiv preprint, 25 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.16429)]

## Activation Function Optimization

:fire:**Implicit Neural Representations with Periodic Activation Functions**<br>
*Vincent Sitzmann, Julien N. P. Martel, Alexander W. Bergman, David B. Lindell, Gordon Wetzstein*<br>
NeurIPS 2020, 17 Jun 2020<br>
<details span>
<summary><b>Abstract</b></summary>
Implicitly defined, continuous, differentiable signal representations parameterized by neural networks have emerged as a powerful paradigm, offering many possible benefits over conventional representations. However, current network architectures for such implicit neural representations are incapable of modeling signals with fine detail, and fail to represent a signal's spatial and temporal derivatives, despite the fact that these are essential to many physical signals defined implicitly as the solution to partial differential equations. We propose to leverage periodic activation functions for implicit neural representations and demonstrate that these networks, dubbed sinusoidal representation networks or Sirens, are ideally suited for representing complex natural signals and their derivatives. We analyze Siren activation statistics to propose a principled initialization scheme and demonstrate the representation of images, wavefields, video, sound, and their derivatives. Further, we show how Sirens can be leveraged to solve challenging boundary value problems, such as particular Eikonal equations (yielding signed distance functions), the Poisson equation, and the Helmholtz and wave equations. Lastly, we combine Sirens with hypernetworks to learn priors over the space of Siren functions.
</details>

[[arXiv](https://arxiv.org/abs/2006.09661)]<br>

**Multiplicative Filter Networks**<br>
*Rizal Fathony, Anit Kumar Sahu, Devin Willmott, J Zico Kolter*<br>
ICLR 2021, 13 Jan 2021<br>
[[OpenReview](https://openreview.net/forum?id=OmtmcPkkhT)]

**PREF: Phasorial Embedding Fields for Compact Neural Representations**<br>
*Binbin Huang, Xinhao Yan, Anpei Chen, Shenghua Gao, Jingyi Yu*<br>
arXiv preprint, 26 May 2022<br>
[[avXiv](https://arxiv.org/abs/2205.13524)]

## Positional Encoding

**Fourier Features Let Networks Learn High Frequency Functions in Low Dimensional Domains**<br>
*Matthew Tancik, Pratul P. Srinivasan, Ben Mildenhall, Sara Fridovich-Keil, Nithin Raghavan, Utkarsh Singhal, Ravi Ramamoorthi, Jonathan T. Barron, Ren Ng*<br>
arXiv preprint, 18 Jun 2020<br>
[[arXiv](https://arxiv.org/abs/2006.10739)]

**BACON: Band-limited Coordinate Networks for Multiscale Scene Representation**<br>
*David B. Lindell, Dave Van Veen, Jeong Joon Park, Gordon Wetzstein*<br>
CVPR 2022, 9 Dec 2021<br>
[[arXiv](https://arxiv.org/abs/2112.04645)] [[Project](https://www.computationalimaging.org/publications/bacon/)] 

**Improved Implicity Neural Representation with Fourier Bases Reparameterized Training**<br>
*Kexuan Shi, Xingyu Zhou, Shuhang Gu*<br>
arXiv preprint, 15 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.07402)]

## Deformable & Dynamic NeRF

:fire:**Nerfies: Deformable Neural Radiance Fields**<br>
*Keunhong Park, Utkarsh Sinha, Jonathan T. Barron, Sofien Bouaziz, Dan B Goldman, Steven M. Seitz, Ricardo Martin-Brualla*<br>
ICCV 2021, 25 Nov 2020<br>
<details span>
<summary><b>Abstract</b></summary>
We present the first method capable of photorealistically reconstructing deformable scenes using photos/videos captured casually from mobile phones. Our approach augments neural radiance fields (NeRF) by optimizing an additional continuous volumetric deformation field that warps each observed point into a canonical 5D NeRF. We observe that these NeRF-like deformation fields are prone to local minima, and propose a coarse-to-fine optimization method for coordinate-based models that allows for more robust optimization. By adapting principles from geometry processing and physical simulation to NeRF-like models, we propose an elastic regularization of the deformation field that further improves robustness. We show that our method can turn casually captured selfie photos/videos into deformable NeRF models that allow for photorealistic renderings of the subject from arbitrary viewpoints, which we dub "nerfies." We evaluate our method by collecting time-synchronized data using a rig with two mobile phones, yielding train/validation images of the same pose at different viewpoints. We show that our method faithfully reconstructs non-rigidly deforming scenes and reproduces unseen views with high fidelity.
</details>

[[arXiv](https://arxiv.org/abs/2011.12948)] [[Project](https://nerfies.github.io/)] [[Github](https://github.com/google/nerfies)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
Recent advances in radiance fields enable photorealistic rendering of static or dynamic 3D scenes, but still do not support explicit deformation that is used for scene manipulation or animation. In this paper, we propose a method that enables a new type of deformation of the radiance field: free-form radiance field deformation. We use a triangular mesh that encloses the foreground object called cage as an interface, and by manipulating the cage vertices, our approach enables the free-form deformation of the radiance field. The core of our approach is cage-based deformation which is commonly used in mesh deformation. We propose a novel formulation to extend it to the radiance field, which maps the position and the view direction of the sampling points from the deformed space to the canonical space, thus enabling the rendering of the deformed scene. The deformation results of the synthetic datasets and the real-world datasets demonstrate the effectiveness of our approach.
</details>

[[arXiv](https://arxiv.org/abs/2207.12298)] [[Project](https://xth430.github.io/deforming-nerf/)] [[Github](https://github.com/xth430/deforming-nerf)]<br>

:fire:**NeRFPlayer: A Streamable Dynamic Scene Representation with Decomposed Neural Radiance Fields**<br>
*Liangchen Song, Anpei Chen, Zhong Li, Zhang Chen, Lele Chen, Junsong Yuan, Yi Xu, Andreas Geiger*<br>
IEEE TVCG, 28 Oct 2022<br>
<details span>
<summary><b>Abstract</b></summary>
Visually exploring in a real-world 4D spatiotemporal space freely in VR has been a long-term quest. The task is especially appealing when only a few or even single RGB cameras are used for capturing the dynamic scene. To this end, we present an efficient framework capable of fast reconstruction, compact modeling, and streamable rendering. First, we propose to decompose the 4D spatiotemporal space according to temporal characteristics. Points in the 4D space are associated with probabilities of belonging to three categories: static, deforming, and new areas. Each area is represented and regularized by a separate neural field. Second, we propose a hybrid representations based feature streaming scheme for efficiently modeling the neural fields. Our approach, coined NeRFPlayer, is evaluated on dynamic scenes captured by single hand-held cameras and multi-camera arrays, achieving comparable or superior rendering performance in terms of quality and speed comparable to recent state-of-the-art methods, achieving reconstruction in 10 seconds per frame and interactive rendering.
</details>

[[arXiv](https://arxiv.org/abs/2210.15947)] [[Project](https://lsongx.github.io/projects/nerfplayer.html)] [[Github(in nerfstudio)](https://github.com/nerfstudio-project/nerfstudio)]<br>

**Robust Dynamic Radiance Fields**<br>
*Yu-Lun Liu, Chen Gao, Andreas Meuleman, Hung-Yu Tseng, Ayush Saraf, Changil Kim, Yung-Yu Chuang, Johannes Kopf, Jia-Bin Huang*<br>
CVPR 2023, 5 Jan 2023<br>
[[arXiv](https://arxiv.org/abs/2301.02239)] [[Project](https://robust-dynrf.github.io/)]

:fire:**HyperReel: High-Fidelity 6-DoF Video with Ray-Conditioned Sampling**<br>
*Benjamin Attal, Jia-Bin Huang, Christian Richardt, Michael Zollhoefer, Johannes Kopf, Matthew O'Toole, Changil Kim*<br>
arXiv preprint, 5 Jan 2023<br>
<details span>
<summary><b>Abstract</b></summary>
Volumetric scene representations enable photorealistic view synthesis for static scenes and form the basis of several existing 6-DoF video techniques. However, the volume rendering procedures that drive these representations necessitate careful trade-offs in terms of quality, rendering speed, and memory efficiency. In particular, existing methods fail to simultaneously achieve real-time performance, small memory footprint, and high-quality rendering for challenging real-world scenes. To address these issues, we present HyperReel -- a novel 6-DoF video representation. The two core components of HyperReel are: (1) a ray-conditioned sample prediction network that enables high-fidelity, high frame rate rendering at high resolutions and (2) a compact and memory-efficient dynamic volume representation. Our 6-DoF video pipeline achieves the best performance compared to prior and contemporary approaches in terms of visual quality with small memory requirements, while also rendering at up to 18 frames-per-second at megapixel resolution without any custom CUDA code.
</details>

[[arXiv](https://arxiv.org/abs/2301.02238)] [[Project](https://hyperreel.github.io/)] [[Github](https://github.com/facebookresearch/hyperreel)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
Modeling and re-rendering dynamic 3D scenes is a challenging task in 3D vision. Prior approaches build on NeRF and rely on implicit representations. This is slow since it requires many MLP evaluations, constraining real-world applications. We show that dynamic 3D scenes can be explicitly represented by six planes of learned features, leading to an elegant solution we call HexPlane. A HexPlane computes features for points in spacetime by fusing vectors extracted from each plane, which is highly efficient. Pairing a HexPlane with a tiny MLP to regress output colors and training via volume rendering gives impressive results for novel view synthesis on dynamic scenes, matching the image quality of prior work but reducing training time by more than 100×. Extensive ablations confirm our HexPlane design and show that it is robust to different feature fusion mechanisms, coordinate systems, and decoding mechanisms. HexPlane is a simple and effective solution for representing 4D volumes, and we hope they can broadly contribute to modeling spacetime for dynamic 3D scenes.
</details>

[[arXiv](https://arxiv.org/abs/2301.09632)] [[Project](https://caoang327.github.io/HexPlane)] [[Github](https://github.com/Caoang327/HexPlane)]<br>

:fire:**K-Planes: Explicit Radiance Fields in Space, Time, and Appearance**<br>
*Sara Fridovich-Keil, Giacomo Meanti, Frederik Warburg, Benjamin Recht, Angjoo Kanazawa*<br>
CVPR 2023, 24 Jan 2023<br>
<details span>
<summary><b>Abstract</b></summary>
We introduce k-planes, a white-box model for radiance fields in arbitrary dimensions. Our model uses d choose 2 planes to represent a d-dimensional scene, providing a seamless way to go from static (d=3) to dynamic (d=4) scenes. This planar factorization makes adding dimension-specific priors easy, e.g. temporal smoothness and multi-resolution spatial structure, and induces a natural decomposition of static and dynamic components of a scene. We use a linear feature decoder with a learned color basis that yields similar performance as a nonlinear black-box MLP decoder. Across a range of synthetic and real, static and dynamic, fixed and varying appearance scenes, k-planes yields competitive and often state-of-the-art reconstruction fidelity with low memory usage, achieving 1000x compression over a full 4D grid, and fast optimization with a pure PyTorch implementation. For video results and code, please see this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2301.10241)] [[Project](https://sarafridov.github.io/K-Planes/)] [[Github](https://github.com/sarafridov/K-Planes)] [[Notes](./paper_discussions/KPlane.md)]<br>

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

**Fast High Dynamic Range Radiance Fields for Dynamic Scenes**<br>
*Guanjun Wu, Taoran Yi, Jiemin Fang, Wenyu Liu, Xinggang Wang*<br>
3DV 2024, 11 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.06052)] [[Project](https://guanjunwu.github.io/HDR-HexPlane/)] [[Code](https://github.com/hustvl/HDR-HexPlane)]

**DaReNeRF: Direction-aware Representation for Dynamic Scenes**<br>
*Ange Lou, Benjamin Planche, Zhongpai Gao, Yamin Li, Tianyu Luan, Hao Ding, Terrence Chen, Jack Noble, Ziyan Wu*<br>
CVPR 2024, 4 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.02265)]

**S-DyRF: Reference-Based Stylized Radiance Fields for Dynamic Scenes**<br>
*Xingyi Li, Zhiguo Cao, Yizheng Wu, Kewei Wang, Ke Xian, Zhe Wang, Guosheng Lin*<br>
CVPR 2024, 10 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.06205)] [[Project](https://xingyi-li.github.io/s-dyrf/)] [[Code](https://github.com/xingyi-li/s-dyrf)]

**NeRF-HuGS: Improved Neural Radiance Fields in Non-static Scenes Using Heuristics-Guided Segmentation**<br>
*Jiahao Chen, Yipeng Qin, Lingjie Liu, Jiangbo Lu, Guanbin Li*<br>
CVPR 2024, 26 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.17537)] [[Project](https://cnhaox.com/NeRF-HuGS/)] [[Code](https://github.com/cnhaox/NeRF-HuGS)]

**LiDAR4D: Dynamic Neural Fields for Novel Space-time View LiDAR Synthesis**<br>
*Zehan Zheng, Fan Lu, Weiyi Xue, Guang Chen, Changjun Jiang*<br>
CVPR 2024, 3 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.02742)] [[Project](https://dyfcalid.github.io/LiDAR4D)] [[Code](https://github.com/ispc-lab/LiDAR4D)]

**TK-Planes: Tiered K-Planes with High Dimensional Feature Vectors for Dynamic UAV-based Scenes**<br>
*Christopher Maxey, Jaehoon Choi, Yonghan Lee, Hyungtae Lee, Dinesh Manocha, Heesung Kwon*<br>
IROS2024, 4 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.02762)]

**JointRF: End-to-End Joint Optimization for Dynamic Neural Radiance Field Representation and Compression**<br>
*Zihan Zheng, Houqiang Zhong, Qiang Hu, Xiaoyun Zhang, Li Song, Ya Zhang, Yanfeng Wang*<br>
arXiv preprint, 23 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.14452)]

**Improving Physics-Augmented Continuum Neural Radiance Field-Based Geometry-Agnostic System Identification with Lagrangian Particle Optimization**<br>
*Takuhiro Kaneko*<br>
CVPR 2024, 6 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.04155)] [[Project](https://www.kecl.ntt.co.jp/people/kaneko.takuhiro/projects/lpo/)] [[Video](https://www.youtube.com/watch?v=jSVgpjbMPvU)]

**TutteNet: Injective 3D Deformations by Composition of 2D Mesh Deformations**<br>
*Bo Sun, Thibault Groueix, Chen Song, Qixing Huang, Noam Aigerman*<br>
arXiv preprint, 17 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.12121)]

**Dynamic Neural Radiance Field From Defocused Monocular Video**<br>
*Xianrui Luo, Huiqiang Sun, Juewen Peng, Zhiguo Cao*<br>
ECCV 2024, 8 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.05586)]

**KFD-NeRF: Rethinking Dynamic NeRF with Kalman Filter**<br>
*Yifan Zhan, Zhuoxiao Li, Muyao Niu, Zhihang Zhong, Shohei Nobuhara, Ko Nishino, Yinqiang Zheng*<br>
ECCV 2024, 18 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.13185)]

**TFS-NeRF: Template-Free NeRF for Semantic 3D Reconstruction of Dynamic Scene**<br>
*Sandika Biswas, Qianyi Wu, Biplab Banerjee, Hamid Rezatofighi*<br>
NeurIPS 2024, 26 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.17459)]

**Deformable NeRF using Recursively Subdivided Tetrahedra**<br>
*Zherui Qiu, Chenqu Ren, Kaiwen Song, Xiaoyi Zeng, Leyuan Yang, Juyong Zhang*<br>
ACM MM 2024, 6 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.04402)] [[Project](https://ustc3dv.github.io/DeformRF/)]


## NeRF Training and Rendering Speed Enhancements

:fire:**Neural Sparse Voxel Fields**<br>
*Lingjie Liu, Jiatao Gu, Kyaw Zaw Lin, Tat-Seng Chua, Christian Theobalt*<br>
NeurIPS 2020, 22 Jul 2020<br>
<details span>
<summary><b>Abstract</b></summary>
Photo-realistic free-viewpoint rendering of real-world scenes using classical computer graphics techniques is challenging, because it requires the difficult step of capturing detailed appearance and geometry models. Recent studies have demonstrated promising results by learning scene representations that implicitly encode both geometry and appearance without 3D supervision. However, existing approaches in practice often show blurry renderings caused by the limited network capacity or the difficulty in finding accurate intersections of camera rays with the scene geometry. Synthesizing high-resolution imagery from these representations often requires time-consuming optical ray marching. In this work, we introduce Neural Sparse Voxel Fields (NSVF), a new neural scene representation for fast and high-quality free-viewpoint rendering. NSVF defines a set of voxel-bounded implicit fields organized in a sparse voxel octree to model local properties in each cell. We progressively learn the underlying voxel structures with a differentiable ray-marching operation from only a set of posed RGB images. With the sparse voxel octree structure, rendering novel views can be accelerated by skipping the voxels containing no relevant scene content. Our method is typically over 10 times faster than the state-of-the-art (namely, NeRF(Mildenhall et al., 2020)) at inference time while achieving higher quality results. Furthermore, by utilizing an explicit sparse voxel representation, our method can easily be applied to scene editing and scene composition. We also demonstrate several challenging tasks, including multi-scene learning, free-viewpoint rendering of a moving human, and large-scale scene rendering. Code and data are available at our website: this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2007.11571)]<br>

:fire:**NeRF++: Analyzing and Improving Neural Radiance Fields**<br>
*Kai Zhang, Gernot Riegler, Noah Snavely, Vladlen Koltun*<br>
arXiv Preprint 2020, 15 Oct 2020<br>
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Fields (NeRF) achieve impressive view synthesis results for a variety of capture settings, including 360 capture of bounded scenes and forward-facing capture of bounded and unbounded scenes. NeRF fits multi-layer perceptrons (MLPs) representing view-invariant opacity and view-dependent color volumes to a set of training images, and samples novel views based on volume rendering techniques. In this technical report, we first remark on radiance fields and their potential ambiguities, namely the shape-radiance ambiguity, and analyze NeRF's success in avoiding such ambiguities. Second, we address a parametrization issue involved in applying NeRF to 360 captures of objects within large-scale, unbounded 3D scenes. Our method improves view synthesis fidelity in this challenging scenario. Code is available at this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2010.07492)] [[Github](https://github.com/Kai-46/nerfplusplus)]<br>

**DeRF: Decomposed Radiance Fields**<br>
*Daniel Rebain, Wei Jiang, Soroosh Yazdani, Ke Li, Kwang Moo Yi, Andrea Tagliasacchi*<br>
CVPR 2021, 25 Nov 2020<br>
[[arXiv](https://arxiv.org/abs/2011.12490)] [[Project](https://ubc-vision.github.io/derf/)] [[Github](https://github.com/ubc-vision/derf/)]

:fire:**AutoInt: Automatic Integration for Fast Neural Volume Rendering**<br>
*David B. Lindell, Julien N. P. Martel, Gordon Wetzstein*<br>
CVPR 2021, 15 Oct 2020<br>
<details span>
<summary><b>Abstract</b></summary>
Numerical integration is a foundational technique in scientific computing and is at the core of many computer vision applications. Among these applications, neural volume rendering has recently been proposed as a new paradigm for view synthesis, achieving photorealistic image quality. However, a fundamental obstacle to making these methods practical is the extreme computational and memory requirements caused by the required volume integrations along the rendered rays during training and inference. Millions of rays, each requiring hundreds of forward passes through a neural network are needed to approximate those integrations with Monte Carlo sampling. Here, we propose automatic integration, a new framework for learning efficient, closed-form solutions to integrals using coordinate-based neural networks. For training, we instantiate the computational graph corresponding to the derivative of the network. The graph is fitted to the signal to integrate. After optimization, we reassemble the graph to obtain a network that represents the antiderivative. By the fundamental theorem of calculus, this enables the calculation of any definite integral in two evaluations of the network. Applying this approach to neural rendering, we improve a tradeoff between rendering speed and image quality: improving render times by greater than 10 times with a tradeoff of slightly reduced image quality.
</details>

[[arXiv](https://arxiv.org/abs/2012.01714)] [[Github](https://github.com/computational-imaging/automatic-integration)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
We introduce a method to render Neural Radiance Fields (NeRFs) in real time using PlenOctrees, an octree-based 3D representation which supports view-dependent effects. Our method can render 800x800 images at more than 150 FPS, which is over 3000 times faster than conventional NeRFs. We do so without sacrificing quality while preserving the ability of NeRFs to perform free-viewpoint rendering of scenes with arbitrary geometry and view-dependent effects. Real-time performance is achieved by pre-tabulating the NeRF into a PlenOctree. In order to preserve view-dependent effects such as specularities, we factorize the appearance via closed-form spherical basis functions. Specifically, we show that it is possible to train NeRFs to predict a spherical harmonic representation of radiance, removing the viewing direction as an input to the neural network. Furthermore, we show that PlenOctrees can be directly optimized to further minimize the reconstruction loss, which leads to equal or better quality compared to competing methods. Moreover, this octree optimization step can be used to reduce the training time, as we no longer need to wait for the NeRF training to converge fully. Our real-time neural rendering approach may potentially enable new applications such as 6-DOF industrial and product visualizations, as well as next generation AR/VR systems. PlenOctrees are amenable to in-browser rendering as well; please visit the project page for the interactive online demo, as well as video and code: this https URL
</details>

[[arXiv](https://arxiv.org/abs/2103.14024)] [[Project](https://alexyu.net/plenoctrees/)] [[Github](https://github.com/sxyu/plenoctree)] [[Viewer Github](https://github.com/sxyu/volrend)]<br>

:fire:**Baking Neural Radiance Fields for Real-Time View Synthesis**<br>
*Peter Hedman, Pratul P. Srinivasan, Ben Mildenhall, Jonathan T. Barron, Paul Debevec*<br>
ICCV 2021, 26 Mar 2021<br>
<details span>
<summary><b>Abstract</b></summary>
Neural volumetric representations such as Neural Radiance Fields (NeRF) have emerged as a compelling technique for learning to represent 3D scenes from images with the goal of rendering photorealistic images of the scene from unobserved viewpoints. However, NeRF's computational requirements are prohibitive for real-time applications: rendering views from a trained NeRF requires querying a multilayer perceptron (MLP) hundreds of times per ray. We present a method to train a NeRF, then precompute and store (i.e. "bake") it as a novel representation called a Sparse Neural Radiance Grid (SNeRG) that enables real-time rendering on commodity hardware. To achieve this, we introduce 1) a reformulation of NeRF's architecture, and 2) a sparse voxel grid representation with learned feature vectors. The resulting scene representation retains NeRF's ability to render fine geometric details and view-dependent appearance, is compact (averaging less than 90 MB per scene), and can be rendered in real-time (higher than 30 frames per second on a laptop GPU). Actual screen captures are shown in our video.
</details>

[[arXiv](https://arxiv.org/abs/2103.14645)] [[Project](https://phog.github.io/snerg/)] [[Github](https://github.com/google-research/google-research/tree/master/snerg)]<br>


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
<details span>
<summary><b>Abstract</b></summary>
We introduce Plenoxels (plenoptic voxels), a system for photorealistic view synthesis. Plenoxels represent a scene as a sparse 3D grid with spherical harmonics. This representation can be optimized from calibrated images via gradient methods and regularization without any neural components. On standard, benchmark tasks, Plenoxels are optimized two orders of magnitude faster than Neural Radiance Fields with no loss in visual quality.
</details>

[[arXiv](https://arxiv.org/abs/2112.05131)] [[Project](https://alexyu.net/plenoxels/)] [[Github](https://github.com/sxyu/svox2)]<br>

:fire:**Instant Neural Graphics Primitives with a Multiresolution Hash Encoding**<br>
*Thomas Müller, Alex Evans, Christoph Schied, Alexander Keller*<br>
SIGGRAPH 2022, 16 Jan 2022<br>
<details span>
<summary><b>Abstract</b></summary>
Neural graphics primitives, parameterized by fully connected neural networks, can be costly to train and evaluate. We reduce this cost with a versatile new input encoding that permits the use of a smaller network without sacrificing quality, thus significantly reducing the number of floating point and memory access operations: a small neural network is augmented by a multiresolution hash table of trainable feature vectors whose values are optimized through stochastic gradient descent. The multiresolution structure allows the network to disambiguate hash collisions, making for a simple architecture that is trivial to parallelize on modern GPUs. We leverage this parallelism by implementing the whole system using fully-fused CUDA kernels with a focus on minimizing wasted bandwidth and compute operations. We achieve a combined speedup of several orders of magnitude, enabling training of high-quality neural graphics primitives in a matter of seconds, and rendering in tens of milliseconds at a resolution of 1920×1080.
</details>

[[arXiv](https://arxiv.org/abs/2201.05989)] [[Project](https://nvlabs.github.io/instant-ngp/)] [[Github](https://github.com/NVlabs/instant-ngp)]<br>

:fire:**TensoRF: Tensorial Radiance Fields**<br>
*Anpei Chen, Zexiang Xu, Andreas Geiger, Jingyi Yu, Hao Su*<br>
ECCV 2022, 17 Mar 2022<br>
<details span>
<summary><b>Abstract</b></summary>
We present TensoRF, a novel approach to model and reconstruct radiance fields. Unlike NeRF that purely uses MLPs, we model the radiance field of a scene as a 4D tensor, which represents a 3D voxel grid with per-voxel multi-channel features. Our central idea is to factorize the 4D scene tensor into multiple compact low-rank tensor components. We demonstrate that applying traditional CP decomposition -- that factorizes tensors into rank-one components with compact vectors -- in our framework leads to improvements over vanilla NeRF. To further boost performance, we introduce a novel vector-matrix (VM) decomposition that relaxes the low-rank constraints for two modes of a tensor and factorizes tensors into compact vector and matrix factors. Beyond superior rendering quality, our models with CP and VM decompositions lead to a significantly lower memory footprint in comparison to previous and concurrent works that directly optimize per-voxel features. Experimentally, we demonstrate that TensoRF with CP decomposition achieves fast reconstruction (<30 min) with better rendering quality and even a smaller model size (<4 MB) compared to NeRF. Moreover, TensoRF with VM decomposition further boosts rendering quality and outperforms previous state-of-the-art methods, while reducing the reconstruction time (<10 min) and retaining a compact model size (<75 MB).
</details>

[[arXiv](https://arxiv.org/abs/2203.09517)] [[Project](https://apchenstu.github.io/TensoRF/)] [[Github](https://github.com/apchenstu/TensoRF)] [[Notes](./paper_discussions/TensoRF.md)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Fields (NeRFs) have demonstrated amazing ability to synthesize images of 3D scenes from novel views. However, they rely upon specialized volumetric rendering algorithms based on ray marching that are mismatched to the capabilities of widely deployed graphics hardware. This paper introduces a new NeRF representation based on textured polygons that can synthesize novel images efficiently with standard rendering pipelines. The NeRF is represented as a set of polygons with textures representing binary opacities and feature vectors. Traditional rendering of the polygons with a z-buffer yields an image with features at every pixel, which are interpreted by a small, view-dependent MLP running in a fragment shader to produce a final pixel color. This approach enables NeRFs to be rendered with the traditional polygon rasterization pipeline, which provides massive pixel-level parallelism, achieving interactive frame rates on a wide range of compute platforms, including mobile phones.
</details>

[[arXiv](https://arxiv.org/abs/2208.00277)] [[Project](https://mobile-nerf.github.io/)] [[Github](https://github.com/google-research/jax3d/tree/main/jax3d/projects/mobilenerf)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
Neural radiance fields enable state-of-the-art photorealistic view synthesis. However, existing radiance field representations are either too compute-intensive for real-time rendering or require too much memory to scale to large scenes. We present a Memory-Efficient Radiance Field (MERF) representation that achieves real-time rendering of large-scale scenes in a browser. MERF reduces the memory consumption of prior sparse volumetric radiance fields using a combination of a sparse feature grid and high-resolution 2D feature planes. To support large-scale unbounded scenes, we introduce a novel contraction function that maps scene coordinates into a bounded volume while still allowing for efficient ray-box intersection. We design a lossless procedure for baking the parameterization used during training into a model that achieves real-time rendering while still preserving the photorealistic view synthesis quality of a volumetric radiance field.
</details>

[[arXiv](https://arxiv.org/abs/2302.12249)] [[Project](https://merf42.github.io/)]<br>

:fire:**BakedSDF: Meshing Neural SDFs for Real-Time View Synthesis**<br>
*Lior Yariv, Peter Hedman, Christian Reiser, Dor Verbin, Pratul P. Srinivasan, Richard Szeliski, Jonathan T. Barron, Ben Mildenhall*<br>
arXiv preprint, 28 Feb 2023<br>
<details span>
<summary><b>Abstract</b></summary>
We present a method for reconstructing high-quality meshes of large unbounded real-world scenes suitable for photorealistic novel view synthesis. We first optimize a hybrid neural volume-surface scene representation designed to have well-behaved level sets that correspond to surfaces in the scene. We then bake this representation into a high-quality triangle mesh, which we equip with a simple and fast view-dependent appearance model based on spherical Gaussians. Finally, we optimize this baked representation to best reproduce the captured viewpoints, resulting in a model that can leverage accelerated polygon rasterization pipelines for real-time view synthesis on commodity hardware. Our approach outperforms previous scene representations for real-time rendering in terms of accuracy, speed, and power consumption, and produces high quality meshes that enable applications such as appearance editing and physical simulation.
</details>

[[arXiv](https://arxiv.org/abs/2302.14859)] [[Project](https://bakedsdf.github.io/)]<br>

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


**HyperPlanes: Hypernetwork Approach to Rapid NeRF Adaptation**<br>
*Paweł Batorski, Dawid Malarz, Marcin Przewięźlikowski, Marcin Mazur, Sławomir Tadeja, Przemysław Spurek*<br>
arXiv preprint, 2 Feb 2024<br>
[[arXiv](https://browse.arxiv.org/abs/2402.01524)]

**Preconditioners for the Stochastic Training of Implicit Neural Representations**<br>
*Shin-Fang Chng, Hemanth Saratchandran, Simon Lucey*<br>
arXiv preprint, 13 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.08784)]

**Improved Generalization of Weight Space Networks via Augmentations**<br>
*Aviv Shamsian, Aviv Navon, David W. Zhang, Yan Zhang, Ethan Fetaya, Gal Chechik, Haggai Maron*<br>
arXiv preprint, 6 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.04081)]

**Vosh: Voxel-Mesh Hybrid Representation for Real-Time View Synthesis**<br>
*Chenhao Zhang, Yongyang Zhou, Lei Zhang*<br>
arXiv preprint, 11 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.06505)]

**Plug-and-Play Acceleration of Occupancy Grid-based NeRF Rendering using VDB Grid and Hierarchical Ray Traversal**<br>
*Yoshio Kato, Shuhei Tarashima*<br>
CVPR Neural Rendering Intelligence Workshop 2024, 16 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.10272)] [[Code](https://github.com/Yosshi999/faster-occgrid)]

**Cicero: Addressing Algorithmic and Architectural Bottlenecks in Neural Rendering by Radiance Warping and Memory Optimizations**<br>
*Yu Feng, Zihan Liu, Jingwen Leng, Minyi Guo, Yuhao Zhu*<br>
arXiv preprint, 18 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.11852)]

:fire:**NeRF-XL: Scaling NeRFs with Multiple GPUs**<br>
*Ruilong Li, Sanja Fidler, Angjoo Kanazawa, Francis Williams*<br>
arXiv preprint, 24 Apr 2024<br>
<details span>
<summary><b>Abstract</b></summary>
We present NeRF-XL, a principled method for distributing Neural Radiance Fields (NeRFs) across multiple GPUs, thus enabling the training and rendering of NeRFs with an arbitrarily large capacity. We begin by revisiting existing multi-GPU approaches, which decompose large scenes into multiple independently trained NeRFs, and identify several fundamental issues with these methods that hinder improvements in reconstruction quality as additional computational resources (GPUs) are used in training. NeRF-XL remedies these issues and enables the training and rendering of NeRFs with an arbitrary number of parameters by simply using more hardware. At the core of our method lies a novel distributed training and rendering formulation, which is mathematically equivalent to the classic single-GPU case and minimizes communication between GPUs. By unlocking NeRFs with arbitrarily large parameter counts, our approach is the first to reveal multi-GPU scaling laws for NeRFs, showing improvements in reconstruction quality with larger parameter counts and speed improvements with more GPUs. We demonstrate the effectiveness of NeRF-XL on a wide variety of datasets, including the largest open-source dataset to date, MatrixCity, containing 258K images covering a 25km^2 city area.
</details>

[[arXiv](https://arxiv.org/abs/2404.16221)] [[Project](https://research.nvidia.com/labs/toronto-ai/nerfxl/)]<br>

**Towards Real-Time Neural Volumetric Rendering on Mobile Devices: A Measurement Study**<br>
*Zhe Wang, Yifei Zhu*<br>
ACM SIGCOMM Workshop on Emerging Multimedia Systems 2024, 23 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.16068)]

**NGP-RT: Fusing Multi-Level Hash Features with Lightweight Attention for Real-Time Novel View Synthesis**<br>
*Yubin Hu, Xiaoyang Guo, Yang Xiao, Jingwei Huang, Yong-Jin Liu*<br>
ECCV 2024, 15 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.10482)]

**Boost Your NeRF: A Model-Agnostic Mixture of Experts Framework for High Quality and Efficient Rendering**<br>
*Francesco Di Sario, Riccardo Renzulli, Enzo Tartaglione, Marco Grangetto*<br>
arXiv preprint, 15 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.10389)]

**Potamoi: Accelerating Neural Rendering via a Unified Streaming Architecture**<br>
*Yu Feng, Weikai Lin, Zihan Liu, Jingwen Leng, Minyi Guo, Han Zhao, Xiaofeng Hou, Jieru Zhao, Yuhao Zhu*<br>
arXiv preprint, 13 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.06608)]

**Expansive Supervision for Neural Radiance Field**<br>
*Weixiang Zhang, Shuzhao Xie, Shijia Ge, Wei Yao, Chen Tang, Zhi Wang*<br>
arXiv preprint, 12 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.08056)]

## One-Shot/Few-Shot Sparse View Reconstruction

:fire:**pixelNeRF: Neural Radiance Fields from One or Few Images**<br>
*Alex Yu, Vickie Ye, Matthew Tancik, Angjoo Kanazawa*<br>
CVPR 2021, 3 Dec 2020<br>
<details span>
<summary><b>Abstract</b></summary>
We propose pixelNeRF, a learning framework that predicts a continuous neural scene representation conditioned on one or few input images. The existing approach for constructing neural radiance fields involves optimizing the representation to every scene independently, requiring many calibrated views and significant compute time. We take a step towards resolving these shortcomings by introducing an architecture that conditions a NeRF on image inputs in a fully convolutional manner. This allows the network to be trained across multiple scenes to learn a scene prior, enabling it to perform novel view synthesis in a feed-forward manner from a sparse set of views (as few as one). Leveraging the volume rendering approach of NeRF, our model can be trained directly from images with no explicit 3D supervision. We conduct extensive experiments on ShapeNet benchmarks for single image novel view synthesis tasks with held-out objects as well as entire unseen categories. We further demonstrate the flexibility of pixelNeRF by demonstrating it on multi-object ShapeNet scenes and real scenes from the DTU dataset. In all cases, pixelNeRF outperforms current state-of-the-art baselines for novel view synthesis and single image 3D reconstruction. For the video and code, please visit the project website: this https URL
</details>

[[arXiv](https://arxiv.org/abs/2012.02190)] [[Project](https://alexyu.net/pixelnerf/)] [[Github](https://github.com/sxyu/pixel-nerf)]<br>

**IBRNet: Learning Multi-View Image-Based Rendering**<br>
*Qianqian Wang, Zhicheng Wang, Kyle Genova, Pratul Srinivasan, Howard Zhou, Jonathan T. Barron, Ricardo Martin-Brualla, Noah Snavely, Thomas Funkhouser*<br>
CVPR 2021, 25 Feb 2021<br>
[[arXiv](https://arxiv.org/abs/2102.13090)] [[Project](https://ibrnet.github.io/)] [[Github](https://github.com/googleinterns/IBRNet)]

:fire:**Putting NeRF on a Diet: Semantically Consistent Few-Shot View Synthesis**<br>
*Ajay Jain, Matthew Tancik, Pieter Abbeel*<br>
arXiv preprint, 1 Apr 2021<br>
<details span>
<summary><b>Abstract</b></summary>
We present DietNeRF, a 3D neural scene representation estimated from a few images. Neural Radiance Fields (NeRF) learn a continuous volumetric representation of a scene through multi-view consistency, and can be rendered from novel viewpoints by ray casting. While NeRF has an impressive ability to reconstruct geometry and fine details given many images, up to 100 for challenging 360° scenes, it often finds a degenerate solution to its image reconstruction objective when only a few input views are available. To improve few-shot quality, we propose DietNeRF. We introduce an auxiliary semantic consistency loss that encourages realistic renderings at novel poses. DietNeRF is trained on individual scenes to (1) correctly render given input views from the same pose, and (2) match high-level semantic attributes across different, random poses. Our semantic loss allows us to supervise DietNeRF from arbitrary poses. We extract these semantics using a pre-trained visual encoder such as CLIP, a Vision Transformer trained on hundreds of millions of diverse single-view, 2D photographs mined from the web with natural language supervision. In experiments, DietNeRF improves the perceptual quality of few-shot view synthesis when learned from scratch, can render novel views with as few as one observed image when pre-trained on a multi-view dataset, and produces plausible completions of completely unobserved regions.
</details>

[[arXiv](https://arxiv.org/abs/2104.00677)] [[Project](https://www.ajayj.com/dietnerf)] [[Github](https://github.com/ajayjain/DietNeRF)]<br>

**MINE: Towards Continuous Depth MPI with NeRF for Novel View Synthesis**<br>
*Jiaxin Li, Zijian Feng, Qi She, Henghui Ding, Changhu Wang, Gim Hee Lee*<br>
ICCV 2021, 27 Mar 2021<br>
[[arXiv](https://arxiv.org/abs/2103.14910)] [[Project](https://vincentfung13.github.io/projects/nemi/)] [[Github](https://github.com/vincentfung13/MINE)]

:fire:**MVSNeRF: Fast Generalizable Radiance Field Reconstruction from Multi-View Stereo**<br>
*Anpei Chen, Zexiang Xu, Fuqiang Zhao, Xiaoshuai Zhang, Fanbo Xiang, Jingyi Yu, Hao Su*<br>
ICCV 2021, 29 Mar 2021<br>
<details span>
<summary><b>Abstract</b></summary>
We present MVSNeRF, a novel neural rendering approach that can efficiently reconstruct neural radiance fields for view synthesis. Unlike prior works on neural radiance fields that consider per-scene optimization on densely captured images, we propose a generic deep neural network that can reconstruct radiance fields from only three nearby input views via fast network inference. Our approach leverages plane-swept cost volumes (widely used in multi-view stereo) for geometry-aware scene reasoning, and combines this with physically based volume rendering for neural radiance field reconstruction. We train our network on real objects in the DTU dataset, and test it on three different datasets to evaluate its effectiveness and generalizability. Our approach can generalize across scenes (even indoor scenes, completely different from our training scenes of objects) and generate realistic view synthesis results using only three input images, significantly outperforming concurrent works on generalizable radiance field reconstruction. Moreover, if dense images are captured, our estimated radiance field representation can be easily fine-tuned; this leads to fast per-scene reconstruction with higher rendering quality and substantially less optimization time than NeRF.
</details>

[[arXiv](https://arxiv.org/abs/2103.15595)] [[Project](https://apchenstu.github.io/mvsnerf/)] [[Github](https://github.com/apchenstu/mvsnerf)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
Novel view synthesis is a long-standing problem. In this work, we consider a variant of the problem where we are given only a few context views sparsely covering a scene or an object. The goal is to predict novel viewpoints in the scene, which requires learning priors. The current state of the art is based on Neural Radiance Field (NeRF), and while achieving impressive results, the methods suffer from long training times as they require evaluating millions of 3D point samples via a neural network for each image. We propose a 2D-only method that maps multiple context views and a query pose to a new image in a single pass of a neural network. Our model uses a two-stage architecture consisting of a codebook and a transformer model. The codebook is used to embed individual images into a smaller latent space, and the transformer solves the view synthesis task in this more compact space. To train our model efficiently, we introduce a novel branching attention mechanism that allows us to use the same model not only for neural rendering but also for camera pose estimation. Experimental results on real-world scenes show that our approach is competitive compared to NeRF-based methods while not reasoning explicitly in 3D, and it is faster to train.
</details>

[[arXiv](https://arxiv.org/abs/2203.10157)] [[Project](https://jkulhanek.github.io/viewformer)] [[Github](https://github.com/jkulhanek/viewformer)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
Novel view synthesis with sparse inputs is a challenging problem for neural radiance fields (NeRF). Recent efforts alleviate this challenge by introducing external supervision, such as pre-trained models and extra depth signals, and by non-trivial patch-based rendering. In this paper, we present Frequency regularized NeRF (FreeNeRF), a surprisingly simple baseline that outperforms previous methods with minimal modifications to the plain NeRF. We analyze the key challenges in few-shot neural rendering and find that frequency plays an important role in NeRF's training. Based on the analysis, we propose two regularization terms. One is to regularize the frequency range of NeRF's inputs, while the other is to penalize the near-camera density fields. Both techniques are ``free lunches'' at no additional computational cost. We demonstrate that even with one line of code change, the original NeRF can achieve similar performance as other complicated methods in the few-shot setting. FreeNeRF achieves state-of-the-art performance across diverse datasets, including Blender, DTU, and LLFF. We hope this simple baseline will motivate a rethinking of the fundamental role of frequency in NeRF's training under the low-data regime and beyond.
</details>

[[arXiv](https://arxiv.org/abs/2303.07418)] [[Project](https://jiawei-yang.github.io/FreeNeRF/)] [[Github](https://github.com/Jiawei-Yang/FreeNeRF)] [[Notes](./paper_discussions/FreeNeRF.md)]<br>

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

**ProvNeRF: Modeling per Point Provenance in NeRFs as a Stochastic Process**<br>
*Kiyohiro Nakayama, Mikaela Angelina Uy, Yang You, Ke Li, Leonidas Guibas*<br>
arXiv preprint, 16 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.08140)] [[Project](https://provnerf.github.io/)]

**HG3-NeRF: Hierarchical Geometric, Semantic, and Photometric Guided Neural Radiance Fields for Sparse View Inputs**<br>
*Zelin Gao, Weichen Dai, Yu Zhang*<br>
arXiv preprint, 22 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.11711)]

**FrameNeRF: A Simple and Efficient Framework for Few-shot Novel View Synthesis**<br>
*Yan Xing, Pan Wang, Ligang Liu, Daolun Li, Li Zhang*<br>
arXiv preprint, 22 Feb, 2024<br>
[[arXiv](https://arxiv.org/abs/2402.14586)]

**CMC: Few-shot Novel View Synthesis via Cross-view Multiplane Consistency**<br>
*Hanxin Zhu, Tianyu He, Zhibo Chen*<br>
IEEE VR 2024, 26 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.16407)]

**DreamUp3D: Object-Centric Generative Models for Single-View 3D Scene Understanding and Real-to-Sim Transfer**<br>
*Yizhe Wu, Haitz Sáez de Ocáriz Borde, Jack Collins, Oiwi Parker Jones, Ingmar Posner*<br>
arXiv preprint, 26 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.16308)]

**Depth-Guided Robust and Fast Point Cloud Fusion NeRF for Sparse Input Views**<br>
*Shuai Guo, Qiuwen Wang, Yijie Gao, Rong Xie, Li Song*<br>
arXiv preprint, 4 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.02063)]

**Is Vanilla MLP in Neural Radiance Field Enough for Few-shot View Synthesis?**<br>
*Hanxin Zhu, Tianyu He, Xin Li, Bingchen Li, Zhibo Chen*<br>
CVPR 2024, 10 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.06092)]

**FSViewFusion: Few-Shots View Generation of Novel Objects**<br>
*Rukhshanda Hussain, Hui Xian Grace Lim, Borchun Chen, Mubarak Shah, Ser Nam Lim*<br>
arXiv preprint, 11 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.06394)]

**CVT-xRF: Contrastive In-Voxel Transformer for 3D Consistent Radiance Fields from Sparse Inputs**<br>
*Yingji Zhong, Lanqing Hong, Zhenguo Li, Dan Xu*<br>
CVPR 2024, 25 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.16885)] [[Project](https://zhongyingji.github.io/CVT-xRF/)]

**UPNeRF: A Unified Framework for Monocular 3D Object Reconstruction and Pose Estimation**<br>
*Yuliang Guo, Abhinav Kumar, Cheng Zhao, Ruoyu Wang, Xinyu Huang, Liu Ren*<br>
arXiv preprint, 23 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.15705)]

**Stable Surface Regularization for Fast Few-Shot NeRF**<br>
*Byeongin Joung, Byeong-Uk Lee, Jaesung Choe, Ukcheol Shin, Minjun Kang, Taeyeop Lee, In So Kweon, Kuk-Jin Yoon*<br>
3DV 2024, 29 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.19985)]

**SGCNeRF: Few-Shot Neural Rendering via Sparse Geometric Consistency Guidance**<br>
*Yuru Xiao, Xianming Liu, Deming Zhai, Kui Jiang, Junjun Jiang, Xiangyang Ji*<br>
arXiv preprint, 1 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.00992)]

**Know Your Neighbors: Improving Single-View Reconstruction via Spatial Vision-Language Reasoning**<br>
*Rui Li, Tobias Fischer, Mattia Segu, Marc Pollefeys, Luc Van Gool, Federico Tombari*<br>
CVPR 2024, 4 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.03658)] [[Project](https://ruili3.github.io/kyn/)] [[Code](https://github.com/ruili3/Know-Your-Neighbors)]

**Boosting Self-Supervision for Single-View Scene Completion via Knowledge Distillation**<br>
*Keonhee Han, Dominik Muhle, Felix Wimbauer, Daniel Cremers*<br>
arXiv preprint, 11 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.07933)]

**NeRFG-NeRF: Geometry-enhanced Novel View Synthesis from Single-View Images**<br>
*Zixiong Huang, Qi Chen, Libo Sun, Yifan Yang, Naizhou Wang, Mingkui Tan, Qi Wu*<br>
CVPR 2024, 11 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.07474)]

**Simple-RF: Regularizing Sparse Input Radiance Fields with Simpler Solutions**<br>
*Nagabhushan Somraj, Adithyan Karanayil, Sai Harsha Mupparaju, Rajiv Soundararajan*<br>
arXiv preprint, 29 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.19015)] [[Project](https://nagabhushansn95.github.io/publications/2024/Simple-RF.html)] 

**GDGS: Gradient Domain Gaussian Splatting for Sparse Representation of Radiance Fields**<br>
*Yuanhao Gong*<br>
arXiv preprint, 8 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.05446)]

**Synergistic Integration of Coordinate Network and Tensorial Feature for Improving Neural Radiance Fields from Sparse Inputs**<br>
*Mingyu Kim, Jun-Seong Kim, Se-Young Yun, Jin-Hwa Kim*<br>
ICML 2024,  13 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.07857)] [[Project](https://mingyukim87.github.io/SynergyNeRF)] [[Code](https://github.com/MingyuKim87/SynergyNeRF)]

**Spatial Annealing Smoothing for Efficient Few-shot Neural Rendering**<br>
*Yuru Xiao, Xianming Liu, Deming Zhai, Kui Jiang, Junjun Jiang, Xiangyang Ji*<br>
arXiv preprint, 12 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.07828)]


**M-LRM: Multi-view Large Reconstruction Model**<br>
*Mengfei Li, Xiaoxiao Long, Yixun Liang, Weiyu Li, Yuan Liu, Peng Li, Xiaowei Chi, Xingqun Qi, Wei Xue, Wenhan Luo, Qifeng Liu, Yike Guo*<br>
arXiv preprint, 11 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.07648)] [[Project](https://murphylmf.github.io/M-LRM/)]

**GTR: Improving Large 3D Reconstruction Models through Geometry and Texture Refinement**<br>
*Peiye Zhuang, Songfang Han, Chaoyang Wang, Aliaksandr Siarohin, Jiaxu Zou, Michael Vasilkovsky, Vladislav Shakhrai, Sergey Korolev, Sergey Tulyakov, Hsin-Ying Lee*<br>
arXiv preprint, 9 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.05649)] [[Project](https://payeah.net/projects/GTR/)]

**Enhancing Neural Radiance Fields with Depth and Normal Completion Priors from Sparse Views**<br>
*Jiawei Guo, HungChyun Chou, Ning Ding*<br>
arXiv preprint, 8 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.05666)]

**MomentsNeRF: Leveraging Orthogonal Moments for Few-Shot Neural Rendering**<br>
*Ahmad AlMughrabi, Ricardo Marques, Petia Radeva*<br>
arXiv preprint, 2 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.02668)] [[Code](https://amughrabi.github.io/momentsnerf/)]

**InfoNorm: Mutual Information Shaping of Normals for Sparse-View Reconstruction**<br>
*Xulong Wang, Siyan Dong, Youyi Zheng, Yanchao Yang*<br>
ECCV 2024, 17 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.12661)] [[Code](https://github.com/Muliphein/InfoNorm)]

**FewShotNeRF: Meta-Learning-based Novel View Synthesis for Rapid Scene-Specific Adaptation**<br>
*Piraveen Sivakumar, Paul Janson, Jathushan Rajasegaran, Thanuja Ambegoda*<br>
arXiv preprint, 9 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.04803)]

**SSNeRF: Sparse View Semi-supervised Neural Radiance Fields with Augmentation**<br>
*Xiao Cao, Beibei Lin, Bo Wang, Zhiyong Huang, Robby T. Tan*<br>
arXiv preprint, 17 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.09144)]

**GeoTransfer : Generalizable Few-Shot Multi-View Reconstruction via Transfer Learning**<br>
*Shubhendu Jena, Franck Multon, Adnane Boukhayma*<br>
arXiv preprint, 27 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.14724)]

**Generic Objects as Pose Probes for Few-Shot View Synthesis**<br>
*Zhirui Gao, Renjiao Yi, Chenyang Zhu, Ke Zhuang, Wei Chen, Kai Xu*<br>
arXiv preprint, 29 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.16690)] [[Project](https://zhirui-gao.github.io/PoseProbe.github.io/)]

**Toward General Object-level Mapping from Sparse Views with 3D Diffusion Priors**<br>
*Ziwei Liao, Binbin Xu, Steven L. Waslander*<br>
CoRL 2024, 7 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.05514)] [[Code](https://github.com/TRAILab/GeneralObjectMapping)]

**Few-shot NeRF by Adaptive Rendering Loss Regularization**<br>
*Qingshan Xu, Xuanyu Yi, Jianyao Xu, Wenbing Tao, Yew-Soon Ong, Hanwang Zhang*<br>
ECCV 2024, 23 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.17839)]

**FrugalNeRF: Fast Convergence for Few-shot Novel View Synthesis without Learned Priors**<br>
*Chin-Yang Lin, Chung-Ho Wu, Chang-Han Yeh, Shih-Han Yen, Cheng Sun, Yu-Lun Liu*<br>
arXiv preprint, 21 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.16271)] [[Project](https://linjohnss.github.io/frugalnerf/)]



## NeRF-3DGS Transfer

**NeRFs to Gaussian Splats, and Back**<br>
*Siming He, Zach Osman, Pratik Chaudhari*<br>
arXiv preprint, 15 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.09717)]

## NeRF Based SLAM

### NeRF SLAM Survey

**How NeRFs and 3D Gaussian Splatting are Reshaping SLAM: a Survey**<br>
*Fabio Tosi, Youmin Zhang, Ziren Gong, Erik Sandström, Stefano Mattoccia, Martin R. Oswald, Matteo Poggi*<br>
arXiv preprint, 20 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.13255)]

### NeRF SLAM Progress

:fire:**NICE-SLAM: Neural Implicit Scalable Encoding for SLAM**<br>
*Zihan Zhu, Songyou Peng, Viktor Larsson, Weiwei Xu, Hujun Bao, Zhaopeng Cui, Martin R. Oswald, Marc Pollefeys*<br>
CVPR 2022, 22 Dec 2021<br>
<details span>
<summary><b>Abstract</b></summary>
Neural implicit representations have recently shown encouraging results in various domains, including promising progress in simultaneous localization and mapping (SLAM). Nevertheless, existing methods produce over-smoothed scene reconstructions and have difficulty scaling up to large scenes. These limitations are mainly due to their simple fully-connected network architecture that does not incorporate local information in the observations. In this paper, we present NICE-SLAM, a dense SLAM system that incorporates multi-level local information by introducing a hierarchical scene representation. Optimizing this representation with pre-trained geometric priors enables detailed reconstruction on large indoor scenes. Compared to recent neural implicit SLAM systems, our approach is more scalable, efficient, and robust. Experiments on five challenging datasets demonstrate competitive results of NICE-SLAM in both mapping and tracking quality. Project page: this https URL
</details>

[[arXiv](https://arxiv.org/abs/2112.12130)] [[Project](https://pengsongyou.github.io/nice-slam)] [[Github](https://github.com/cvg/nice-slam)] [[Notes](./paper_discussions/NICE-SLAM.md)]<br>

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

**Hi-Map: Hierarchical Factorized Radiance Field for High-Fidelity Monocular Dense Mapping**<br>
*Tongyan Hua, Haotian Bai, Zidong Cao, Ming Liu, Dacheng Tao, Lin Wang*<br>
arXiv preprint, 6 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.03203)]

**N^3-Mapping: Normal Guided Neural Non-Projective Signed Distance Fields for Large-scale 3D Mapping**<br>
*Shuangfu Song, Junqiao Zhao, Kai Huang, Jiaye Lin, Chen Ye, Tiantian Feng*<br>
arXiv preprint, 7 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.03412)]

**Q-SLAM: Quadric Representations for Monocular SLAM**<br>
*Chensheng Peng, Chenfeng Xu, Yue Wang, Mingyu Ding, Heng Yang, Masayoshi Tomizuka, Kurt Keutzer, Marco Pavone, Wei Zhan*<br>
arXiv preprint, 12 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.08125)]

**Learning Neural Volumetric Pose Features for Camera Localization**<br>
*Jingyu Lin, Jiaqi Gu, Bojian Wu, Lubin Fan, Renjie Chen, Ligang Liu, Jieping Ye*<br>
arXiv preprint, 19 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.12800)]

**DVN-SLAM: Dynamic Visual Neural SLAM Based on Local-Global Encoding**<br>
*Wenhua Wu, Guangming Wang, Ting Deng, Sebastian Aegidius, Stuart Shanks, Valerio Modugno, Dimitrios Kanoulas, Hesheng Wang*<br>
arXiv preprint, 18 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.11776)]

**WSCLoc: Weakly-Supervised Sparse-View Camera Relocalization**<br>
*Jialu Wang, Kaichen Zhou, Andrew Markham, Niki Trigoni*<br>
arXiv preprint, 22 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.15272)]

**NeSLAM: Neural Implicit Mapping and Self-Supervised Feature Tracking With Depth Completion and Denoising**<br>
*Tianchen Deng, Yanbo Wang, Hongle Xie, Hesheng Wang, Jingchuan Wang, Danwei Wang, Weidong Chen*<br>
arXiv preprint, 29 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.20034)]

**VRS-NeRF: Visual Relocalization with Sparse Neural Radiance Field**<br>
*Fei Xue, Ignas Budvytis, Daniel Olmeda Reino, Roberto Cipolla*<br>
arXiv preprint, 14 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.09271)] [[Code](https://github.com/feixue94/vrs-nerf)]

**SLAIM: Robust Dense Neural SLAM for Online Tracking and Mapping**<br>
*Vincent Cartillier, Grant Schindler, Irfan Essa*<br>
arXiv preprint, 17 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.11419)]

**EC-SLAM: Real-time Dense Neural RGB-D SLAM System with Effectively Constrained Global Bundle Adjustment**<br>
*Guanghao Li, Qi Chen, YuXiang Yan, Jian Pu*<br>
arXiv preprint, 20 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.13346)] [[Code](https://github.com/Lightingooo/EC-SLAM)]

**S3-SLAM: Sparse Tri-plane Encoding for Neural Implicit SLAM**<br>
*Zhiyao Zhang, Yunzhou Zhang, Yanmin Wu, Bin Zhao, Xingshuo Wang, Rui Tian*<br>
arXiv preprint, 28 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.18284)]

**Fast Global Localization on Neural Radiance Field**<br>
*Mangyu Kong, Seongwon Lee, Jaewon Lee, Euntai Kim*<br>
arXiv preprint, 18 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.12202)]

**I^2-SLAM: Inverting Imaging Process for Robust Photorealistic Dense SLAM**<br>
*Gwangtak Bae, Changwoon Choi, Hyeongjun Heo, Sang Min Kim, Young Min Kim*<br>
ECCV 2024, 16 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.11347)]

**Evaluating geometric accuracy of NeRF reconstructions compared to SLAM method**<br>
*Adam Korycki, Colleen Josephson, Steve McGuire*<br>
arXiv preprint, 15 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.11238)]

**Visual Localization in 3D Maps: Comparing Point Cloud, Mesh, and NeRF Representations**<br>
*Lintong Zhang, Yifu Tao, Jiarong Lin, Fu Zhang, Maurice Fallon*<br>
arXiv preprint, 21 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.11966)]

**Neural Implicit Representation for Highly Dynamic LiDAR Mapping and Odometry**<br>
*Qi Zhang, He Wang, Ru Li, Wenbin Li*<br>
arXiv preprint, 26 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.17729)]

## Camera Pose Estimation & Weak Camera Pose Reconstruction

**INeRF: Inverting Neural Radiance Fields for Pose Estimation**<br>
*Lin Yen-Chen, Pete Florence, Jonathan T. Barron, Alberto Rodriguez, Phillip Isola, Tsung-Yi Lin*<br>
IROS 2021, 10 Dec 2020 <br>
[[arXiv](https://arxiv.org/abs/2012.05877)] [[Github](https://github.com/huzi96/NVFPCC/)]

:fire:**NeRF--: Neural Radiance Fields Without Known Camera Parameters**<br>
*Zirui Wang, Shangzhe Wu, Weidi Xie, Min Chen, Victor Adrian Prisacariu*<br>
arXiv preprint, 14 Feb 2021<br>
<details span>
<summary><b>Abstract</b></summary>
Considering the problem of novel view synthesis (NVS) from only a set of 2D images, we simplify the training process of Neural Radiance Field (NeRF) on forward-facing scenes by removing the requirement of known or pre-computed camera parameters, including both intrinsics and 6DoF poses. To this end, we propose NeRF−−, with three contributions: First, we show that the camera parameters can be jointly optimised as learnable parameters with NeRF training, through a photometric reconstruction; Second, to benchmark the camera parameter estimation and the quality of novel view renderings, we introduce a new dataset of path-traced synthetic scenes, termed as Blender Forward-Facing Dataset (BLEFF); Third, we conduct extensive analyses to understand the training behaviours under various camera motions, and show that in most scenarios, the joint optimisation pipeline can recover accurate camera parameters and achieve comparable novel view synthesis quality as those trained with COLMAP pre-computed camera parameters. Our code and data are available at this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2102.07064)] [[Project](https://nerfmm.active.vision)] [[Github](https://github.com/ActiveVisionLab/nerfmm)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Fields (NeRF) have recently gained a surge of interest within the computer vision community for its power to synthesize photorealistic novel views of real-world scenes. One limitation of NeRF, however, is its requirement of accurate camera poses to learn the scene representations. In this paper, we propose Bundle-Adjusting Neural Radiance Fields (BARF) for training NeRF from imperfect (or even unknown) camera poses -- the joint problem of learning neural 3D representations and registering camera frames. We establish a theoretical connection to classical image alignment and show that coarse-to-fine registration is also applicable to NeRF. Furthermore, we show that naïvely applying positional encoding in NeRF has a negative impact on registration with a synthesis-based objective. Experiments on synthetic and real-world data show that BARF can effectively optimize the neural scene representations and resolve large camera pose misalignment at the same time. This enables view synthesis and localization of video sequences from unknown camera poses, opening up new avenues for visual localization systems (e.g. SLAM) and potential applications for dense 3D mapping and reconstruction.
</details>

[[arXiv](https://arxiv.org/abs/2104.06405)] [[Project](https://chenhsuanlin.bitbucket.io/bundle-adjusting-NeRF)] [[Github](https://github.com/chenhsuanlin/bundle-adjusting-NeRF)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
Training a Neural Radiance Field (NeRF) without pre-computed camera poses is challenging. Recent advances in this direction demonstrate the possibility of jointly optimising a NeRF and camera poses in forward-facing scenes. However, these methods still face difficulties during dramatic camera movement. We tackle this challenging problem by incorporating undistorted monocular depth priors. These priors are generated by correcting scale and shift parameters during training, with which we are then able to constrain the relative poses between consecutive frames. This constraint is achieved using our proposed novel loss functions. Experiments on real-world indoor and outdoor scenes show that our method can handle challenging camera trajectories and outperforms existing methods in terms of novel view rendering quality and pose estimation accuracy. Our project page is this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2212.07388)] [[Project](https://nope-nerf.active.vision/)] [[Github](https://github.com/ActiveVisionLab/nope-nerf/)]<br>

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

**Improving Robustness for Joint Optimization of Camera Poses and Decomposed Low-Rank Tensorial Radiance Fields**<br>
*Bo-Yu Cheng, Wei-Chen Chiu, Yu-Lun Liu*<br>
AAAI 2024, 20 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.13252)] [[Project](https://alex04072000.github.io/Joint-TensoRF/)] [[Code](https://github.com/Nemo1999/Joint-TensoRF)] [[Video](https://alex04072000.github.io/Joint-TensoRF/img/AAAI_Presentation.mp4)]

**IFFNeRF: Initialisation Free and Fast 6DoF pose estimation from a single image and a NeRF model**<br>
*Matteo Bortolon, Theodore Tsesmelis, Stuart James, Fabio Poiesi, Alessio Del Bue*<br>
ICRA 2024, 19 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.12682)] [[Project](https://mbortolon97.github.io/iffnerf/)] [[Code](https://github.com/mbortolon97/IFFNeRF)] [[Video](https://www.youtube.com/watch?v=0qUEpaws5oI)]

**VF-NeRF: Viewshed Fields for Rigid NeRF Registration**<br>
*Leo Segre, Shai Avidan*<br>
arXiv preprint, 4 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.03349)]

**CT-NeRF: Incremental Optimizing Neural Radiance Field and Poses with Complex Trajectory**<br>
*Yunlong Ran, Yanxu Li, Qi Ye, Yuchi Huo, Zechun Bai, Jiahao Sun, Jiming Chen*<br>
arXiv preprint, 22 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.13896)]

**TD-NeRF: Novel Truncated Depth Prior for Joint Camera Pose and Neural Radiance Field Optimization**<br>
*Zhen Tan, Zongtan Zhou, Yangbing Ge, Zi Wang, Xieyuanli Chen, Dewen Hu*<br>
arXiv preprint, 11 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.07027)]  [[Code](https://github.com/nubot-nudt/TD-NeRF)]

**Leveraging Neural Radiance Fields for Pose Estimation of an Unknown Space Object during Proximity Operations**<br>
*Antoine Legrand, Renaud Detry, Christophe De Vleeschouwer*<br>
arXiv preprint, 21 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.12728)]

**Camera Relocalization in Shadow-free Neural Radiance Fields**<br>
*Shiyao Xu, Caiyun Liu, Yuantao Chen, Zhenxin Zhu, Zike Yan, Yongliang Shi, Hao Zhao, Guyue Zhou*<br>
ICRA 2024, 23 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.14824)] [[Code](https://github.com/hnrna/ShadowfreeNeRF-CameraReloc)]

**SG-NeRF: Neural Surface Reconstruction with Scene Graph Optimization**<br>
*Yiyang Chen, Siyan Dong, Xulong Wang, Lulu Cai, Youyi Zheng, Yanchao Yang*<br>
ECCV 2024, 17 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.12667)] [[Code](https://github.com/Iris-cyy/SG-NeRF)]

**Invertible Neural Warp forNeRF**<br>
*Shin-Fang Chng, Ravi Garg, Hemanth Saratchandran, Simon Lucey*<br>
ECCV 2024, 17 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.12354)] [[Project](https://sfchng.github.io/ineurowarping-github.io/)] [[Code](https://github.com/sfchng/neural_invertible_warp)]

:fire:**TrackNeRF: Bundle Adjusting NeRF from Sparse and Noisy Views via Feature Tracks**<br>
*Jinjie Mai, Wenxuan Zhu, Sara Rojas, Jesus Zarzar, Abdullah Hamdi, Guocheng Qian, Bing Li, Silvio Giancola, Bernard Ghanem*<br>
ECCV 2024, 20 Aug 2024<br>
<details span>
<summary><b>Abstract</b></summary>
Neural radiance fields (NeRFs) generally require many images with accurate poses for accurate novel view synthesis, which does not reflect realistic setups where views can be sparse and poses can be noisy. Previous solutions for learning NeRFs with sparse views and noisy poses only consider local geometry consistency with pairs of views. Closely following \textit{bundle adjustment} in Structure-from-Motion (SfM), we introduce TrackNeRF for more globally consistent geometry reconstruction and more accurate pose optimization. TrackNeRF introduces \textit{feature tracks}, \ie connected pixel trajectories across \textit{all} visible views that correspond to the \textit{same} 3D points. By enforcing reprojection consistency among feature tracks, TrackNeRF encourages holistic 3D consistency explicitly. Through extensive experiments, TrackNeRF sets a new benchmark in noisy and sparse view reconstruction. In particular, TrackNeRF shows significant improvements over the state-of-the-art BARF and SPARF by ∼8 and ∼1 in terms of PSNR on DTU under various sparse and noisy view setups. The code is available at \href{this https URL}.
</details>

[[arXiv](https://arxiv.org/abs/2408.10739)] [[Project](https://tracknerf.github.io/)] [[Code](https://github.com/Wayne-Mai/traf_public)]<br>

**KRONC: Keypoint-based Robust Camera Optimization for 3D Car Reconstruction**<br>
*Davide Di Nucci, Alessandro Simoni, Matteo Tomei, Luca Ciuffreda, Roberto Vezzani, Rita Cucchiara*<br>
ECCVW 2024, 9 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.05407)]

**Robust SG-NeRF: Robust Scene Graph Aided Neural Surface Reconstruction**<br>
*Yi Gu, Dongjun Ye, Zhaorui Wang, Jiaxu Wang, Jiahang Cao, Renjing Xu*<br>
arXiv preprint, 20 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.13620)] [[Project](https://rsg-nerf.github.io/RSG-NeRF/)]
 
## NeRF with MVS

**BoostMVSNeRFs: Boosting MVS-based NeRFs to Generalizable View Synthesis in Large-scale Scenes**<br>
*Chih-Hai Su, Chih-Yao Hu, Shr-Ruei Tsai, Jie-Ying Lee, Chin-Yang Lin, Yu-Lun Liu*<br>
SIGGRAPH 2024, 22 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.15848)] [[Project](https://su-terry.github.io/BoostMVSNeRFs/)] [[Code](https://github.com/Su-Terry/BoostMVSNeRFs)]

## NeRF AIGC

### NeRF AIGC Survey

**Generative AI meets 3D: A Survey on Text-to-3D in AIGC Era**<br>
*Chenghao Li, Chaoning Zhang, Atish Waghwase, Lik-Hang Lee, Francois Rameau, Yang Yang, Sung-Ho Bae, Choong Seon Hong*<br>
arXiv preprint, 10 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.06131)]

**Advances in 3D Generation: A Survey**<br>
*Xiaoyu Li, Qi Zhang, Di Kang, Weihao Cheng, Yiming Gao, Jingbo Zhang, Zhihao Liang, Jing Liao, Yan-Pei Cao, Ying Shan*<br>
arXiv preprint, 31 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.17807)]

**A Survey On Text-to-3D Contents Generation In The Wild**<br>
*Chenhan Jiang*<br>
arXiv preprint, 15 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.09431)]

### NeRF AIGC Progresses

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
<details span>
<summary><b>Abstract</b></summary>
DreamFusion has recently demonstrated the utility of a pre-trained text-to-image diffusion model to optimize Neural Radiance Fields (NeRF), achieving remarkable text-to-3D synthesis results. However, the method has two inherent limitations: (a) extremely slow optimization of NeRF and (b) low-resolution image space supervision on NeRF, leading to low-quality 3D models with a long processing time. In this paper, we address these limitations by utilizing a two-stage optimization framework. First, we obtain a coarse model using a low-resolution diffusion prior and accelerate with a sparse 3D hash grid structure. Using the coarse representation as the initialization, we further optimize a textured 3D mesh model with an efficient differentiable renderer interacting with a high-resolution latent diffusion model. Our method, dubbed Magic3D, can create high quality 3D mesh models in 40 minutes, which is 2x faster than DreamFusion (reportedly taking 1.5 hours on average), while also achieving higher resolution. User studies show 61.7% raters to prefer our approach over DreamFusion. Together with the image-conditioned generation capabilities, we provide users with new ways to control 3D synthesis, opening up new avenues to various creative applications.
</details>

[[arXiv](https://arxiv.org/abs/2211.10440)] [[Project](https://research.nvidia.com/labs/dir/magic3d/)] [[threeStudio](https://github.com/threestudio-project/threestudio)] [[Notes](./paper_discussions/Magic3D.md)]<br>

**Score Jacobian Chaining: Lifting Pretrained 2D Diffusion Models for 3D Generation**<br>
*Haochen Wang, Xiaodan Du, Jiahao Li, Raymond A. Yeh, Greg Shakhnarovich*<br>
CVPR 2023, 1 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.00774)] [[Project](https://pals.ttic.edu/p/score-jacobian-chaining)] [[Github](https://github.com/pals-ttic/sjc/)] [[threeStudio](https://github.com/threestudio-project/threestudio)]

**SparseFusion: Distilling View-conditioned Diffusion for 3D Reconstruction**<br>
*Zhizhuo Zhou, Shubham Tulsiani*<br>
CVPR 2023, 1 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.00792)] [[Project](https://sparsefusion.github.io/)] [[Github](https://github.com/zhizdev/sparsefusion)]

**DiffRF: Rendering-Guided 3D Radiance Field Diffusion**<br>
*Ashkan Mirzaei, Yash Kant, Jonathan Kelly, Igor Gilitschenski*<br>
CVPR 2023, 2 Dec 2022<br>
[[arXiv](https://arxiv.org/abs/2212.01206)] [[Project](https://sirwyver.github.io/DiffRF/)]

:fire:**Dream3D: Zero-Shot Text-to-3D Synthesis Using 3D Shape Prior and Text-to-Image Diffusion Models**<br>
*Jiale Xu, Xintao Wang, Weihao Cheng, Yan-Pei Cao, Ying Shan, Xiaohu Qie, Shenghua Gao*<br>
CVPR 2023, 28 Dec 2022<br>
<details span>
<summary><b>Abstract</b></summary>
Recent CLIP-guided 3D optimization methods, such as DreamFields and PureCLIPNeRF, have achieved impressive results in zero-shot text-to-3D synthesis. However, due to scratch training and random initialization without prior knowledge, these methods often fail to generate accurate and faithful 3D structures that conform to the input text. In this paper, we make the first attempt to introduce explicit 3D shape priors into the CLIP-guided 3D optimization process. Specifically, we first generate a high-quality 3D shape from the input text in the text-to-shape stage as a 3D shape prior. We then use it as the initialization of a neural radiance field and optimize it with the full prompt. To address the challenging text-to-shape generation task, we present a simple yet effective approach that directly bridges the text and image modalities with a powerful text-to-image diffusion model. To narrow the style domain gap between the images synthesized by the text-to-image diffusion model and shape renderings used to train the image-to-shape generator, we further propose to jointly optimize a learnable text prompt and fine-tune the text-to-image diffusion model for rendering-style image generation. Our method, Dream3D, is capable of generating imaginative 3D content with superior visual quality and shape accuracy compared to state-of-the-art methods.
</details>

[[arXiv](https://arxiv.org/abs/2212.14704)] [[Project](https://bluestyle97.github.io/dream3d/)]<br>

**Text-To-4D Dynamic Scene Generation**<br>
*Jiale Xu, Xintao Wang, Weihao Cheng, Yan-Pei Cao, Ying Shan, Xiaohu Qie, Shenghua Gao*<br>
arXiv preprint, 26 Jan 2023<br>
[[arXiv](https://arxiv.org/abs/2301.11280)] [[Project](https://make-a-video3d.github.io/)]

:fire:**LERF: Language Embedded Radiance Fields**<br>
*Justin Kerr, Chung Min Kim, Ken Goldberg, Angjoo Kanazawa, Matthew Tancik*<br>
arXiv preprint, 16 Mar 2023<br>
<details span>
<summary><b>Abstract</b></summary>
Humans describe the physical world using natural language to refer to specific 3D locations based on a vast range of properties: visual appearance, semantics, abstract associations, or actionable affordances. In this work we propose Language Embedded Radiance Fields (LERFs), a method for grounding language embeddings from off-the-shelf models like CLIP into NeRF, which enable these types of open-ended language queries in 3D. LERF learns a dense, multi-scale language field inside NeRF by volume rendering CLIP embeddings along training rays, supervising these embeddings across training views to provide multi-view consistency and smooth the underlying language field. After optimization, LERF can extract 3D relevancy maps for a broad range of language prompts interactively in real-time, which has potential use cases in robotics, understanding vision-language models, and interacting with 3D scenes. LERF enables pixel-aligned, zero-shot queries on the distilled 3D CLIP embeddings without relying on region proposals or masks, supporting long-tail open-vocabulary queries hierarchically across the volume. The project website can be found at this https URL .
</details>

[[arXiv](https://arxiv.org/abs/2303.09553)] [[Project](https://www.lerf.io/)] [[Github](https://github.com/kerrj/lerf)]<br>

:fire:**Shap-E: Generating Conditional 3D Implicit Functions**<br>
*Heewoo Jun, Alex Nichol*<br>
arXiv preprint, 3 May 2023<br>
<details span>
<summary><b>Abstract</b></summary>
We present Shap-E, a conditional generative model for 3D assets. Unlike recent work on 3D generative models which produce a single output representation, Shap-E directly generates the parameters of implicit functions that can be rendered as both textured meshes and neural radiance fields. We train Shap-E in two stages: first, we train an encoder that deterministically maps 3D assets into the parameters of an implicit function; second, we train a conditional diffusion model on outputs of the encoder. When trained on a large dataset of paired 3D and text data, our resulting models are capable of generating complex and diverse 3D assets in a matter of seconds. When compared to Point-E, an explicit generative model over point clouds, Shap-E converges faster and reaches comparable or better sample quality despite modeling a higher-dimensional, multi-representation output space. We release model weights, inference code, and samples at this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2305.02463)] [[Github](https://github.com/openai/shap-e)]<br>

:fire:**3DGen: Triplane Latent Diffusion for Textured Mesh Generation**<br>
*Anchit Gupta, Wenhan Xiong, Yixin Nie, Ian Jones, Barlas Oğuz*<br>
arXiv preprint, 9 Mar 2023<br>
<details span>
<summary><b>Abstract</b></summary>
Latent diffusion models for image generation have crossed a quality threshold which enabled them to achieve mass adoption. Recently, a series of works have made advancements towards replicating this success in the 3D domain, introducing techniques such as point cloud VAE, triplane representation, neural implicit surfaces and differentiable rendering based training. We take another step along this direction, combining these developments in a two-step pipeline consisting of 1) a triplane VAE which can learn latent representations of textured meshes and 2) a conditional diffusion model which generates the triplane features. For the first time this architecture allows conditional and unconditional generation of high quality textured or untextured 3D meshes across multiple diverse categories in a few seconds on a single GPU. It outperforms previous work substantially on image-conditioned and unconditional generation on mesh quality as well as texture generation. Furthermore, we demonstrate the scalability of our model to large datasets for increased quality and diversity. We will release our code and trained models.
</details>

[[arXiv](https://arxiv.org/abs/2303.05371)]<br>

:fire:**MeshDiffusion: Score-based Generative 3D Mesh Modeling**<br>
*Zhen Liu, Yao Feng, Michael J. Black, Derek Nowrouzezahrai, Liam Paull, Weiyang Liu*<br>
ICLR 2023, 14 Mar 2023<br>
<details span>
<summary><b>Abstract</b></summary>
We consider the task of generating realistic 3D shapes, which is useful for a variety of applications such as automatic scene generation and physical simulation. Compared to other 3D representations like voxels and point clouds, meshes are more desirable in practice, because (1) they enable easy and arbitrary manipulation of shapes for relighting and simulation, and (2) they can fully leverage the power of modern graphics pipelines which are mostly optimized for meshes. Previous scalable methods for generating meshes typically rely on sub-optimal post-processing, and they tend to produce overly-smooth or noisy surfaces without fine-grained geometric details. To overcome these shortcomings, we take advantage of the graph structure of meshes and use a simple yet very effective generative modeling method to generate 3D meshes. Specifically, we represent meshes with deformable tetrahedral grids, and then train a diffusion model on this direct parametrization. We demonstrate the effectiveness of our model on multiple generative tasks.
</details>

[[arXiv](https://arxiv.org/abs/2303.08133)] [[Project](https://meshdiffusion.github.io/)] [[Github](https://github.com/lzzcd001/MeshDiffusion/)]<br>

:fire:**DreamBooth3D: Subject-Driven Text-to-3D Generation**<br>
*Amit Raj, Srinivas Kaza, Ben Poole, Michael Niemeyer, Nataniel Ruiz, Ben Mildenhall, Shiran Zada, Kfir Aberman, Michael Rubinstein, Jonathan Barron, Yuanzhen Li, Varun Jampani*<br>
arXiv preprint, 23 Mar 2023<br>
<details span>
<summary><b>Abstract</b></summary>
We present DreamBooth3D, an approach to personalize text-to-3D generative models from as few as 3-6 casually captured images of a subject. Our approach combines recent advances in personalizing text-to-image models (DreamBooth) with text-to-3D generation (DreamFusion). We find that naively combining these methods fails to yield satisfactory subject-specific 3D assets due to personalized text-to-image models overfitting to the input viewpoints of the subject. We overcome this through a 3-stage optimization strategy where we jointly leverage the 3D consistency of neural radiance fields together with the personalization capability of text-to-image models. Our method can produce high-quality, subject-specific 3D assets with text-driven modifications such as novel poses, colors and attributes that are not seen in any of the input images of the subject.
</details>

[[arXiv](https://arxiv.org/abs/2303.13508)] [[Project](https://dreambooth3d.github.io/)]<br>

:fire:**Make-It-3D: High-Fidelity 3D Creation from A Single Image with Diffusion Prior**<br>
*Junshu Tang, Tengfei Wang, Bo Zhang, Ting Zhang, Ran Yi, Lizhuang Ma, Dong Chen*<br>
arXiv preprint, 23 Mar 2023<br>
<details span>
<summary><b>Abstract</b></summary>
In this work, we investigate the problem of creating high-fidelity 3D content from only a single image. This is inherently challenging: it essentially involves estimating the underlying 3D geometry while simultaneously hallucinating unseen textures. To address this challenge, we leverage prior knowledge from a well-trained 2D diffusion model to act as 3D-aware supervision for 3D creation. Our approach, Make-It-3D, employs a two-stage optimization pipeline: the first stage optimizes a neural radiance field by incorporating constraints from the reference image at the frontal view and diffusion prior at novel views; the second stage transforms the coarse model into textured point clouds and further elevates the realism with diffusion prior while leveraging the high-quality textures from the reference image. Extensive experiments demonstrate that our method outperforms prior works by a large margin, resulting in faithful reconstructions and impressive visual quality. Our method presents the first attempt to achieve high-quality 3D creation from a single image for general objects and enables various applications such as text-to-3D creation and texture editing.
</details>

[[arXiv](https://arxiv.org/abs/2303.14184)] [[Project](https://make-it-3d.github.io/)] [[Github](https://github.com/junshutang/Make-It-3D)] [[Notes](./paper_discussions/Make-It-3D.md)]<br>


**Fantasia3D: Disentangling Geometry and Appearance for High-quality Text-to-3D Content Creation**<br>
*Rui Chen, Yongwei Chen, Ningxin Jiao, Kui Jia*<br>
arXiv preprint, 24 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2303.13873)] [[Project](https://fantasia3d.github.io/)] [[Github](https://github.com/Gorilla-Lab-SCUT/Fantasia3D)] [[threeStudio](https://github.com/threestudio-project/threestudio)]

**DITTO-NeRF: Diffusion-based Iterative Text To Omni-directional 3D Model**<br>
*Hoigi Seo, Hayeon Kim, Gwanghyun Kim, Se Young Chun*<br>
CVPR 2023, 6 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.02827)] [[Project](https://janeyeon.github.io/ditto-nerf/)] [[Github](https://github.com/janeyeon/ditto-nerf-code)]


**Single-Stage Diffusion NeRF: A Unified Approach to 3D Generation and Reconstruction**<br>
*Hansheng Chen, Jiatao Gu, Anpei Chen, Wei Tian, Zhuowen Tu, Lingjie Liu, Hao Su*<br>
arXiv preprint, 13 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.06714)] [[Project](https://lakonik.github.io/ssdnerf/)] [[Github](https://github.com/Lakonik/SSDNeRF)]


**Deceptive-NeRF: Enhancing NeRF Reconstruction using Pseudo-Observations from Diffusion Models**<br>
*Xinhang Liu, Shiu-hong Kao, Jiaben Chen, Yu-Wing Tai, Chi-Keung Tang*<br>
arXiv preprint, 24 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.15171)]


:fire:**ProlificDreamer: High-Fidelity and Diverse Text-to-3D Generation with Variational Score Distillation**<br>
*Zhengyi Wang, Cheng Lu, Yikai Wang, Fan Bao, Chongxuan Li, Hang Su, Jun Zhu*<br>
arXiv preprint, 25 May 2023<br>
<details span>
<summary><b>Abstract</b></summary>
Score distillation sampling (SDS) has shown great promise in text-to-3D generation by distilling pretrained large-scale text-to-image diffusion models, but suffers from over-saturation, over-smoothing, and low-diversity problems. In this work, we propose to model the 3D parameter as a random variable instead of a constant as in SDS and present variational score distillation (VSD), a principled particle-based variational framework to explain and address the aforementioned issues in text-to-3D generation. We show that SDS is a special case of VSD and leads to poor samples with both small and large CFG weights. In comparison, VSD works well with various CFG weights as ancestral sampling from diffusion models and simultaneously improves the diversity and sample quality with a common CFG weight (i.e., 7.5). We further present various improvements in the design space for text-to-3D such as distillation time schedule and density initialization, which are orthogonal to the distillation algorithm yet not well explored. Our overall approach, dubbed ProlificDreamer, can generate high rendering resolution (i.e., 512×512) and high-fidelity NeRF with rich structure and complex effects (e.g., smoke and drops). Further, initialized from NeRF, meshes fine-tuned by VSD are meticulously detailed and photo-realistic. Project page and codes: this https URL
</details>

[[arXiv](https://arxiv.org/abs/2305.16213)] [[Project](https://ml.cs.tsinghua.edu.cn/prolificdreamer/)] [[Unofficial Implementation](https://github.com/threestudio-project/threestudio/tree/prolific-dreamer)]<br>

**ATT3D: Amortized Text-to-3D Object Synthesis**<br>
*Jonathan Lorraine, Kevin Xie, Xiaohui Zeng, Chen-Hsuan Lin, Towaki Takikawa,Nicholas Sharp, Tsung-Yi Lin, Ming-Yu Liu, Sanja Fidler, James Lucas*<br>
arXiv preprint, 6 Jun 2023<br>
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

**ReconFusion: 3D Reconstruction with Diffusion Priors**<br>
*Rundi Wu, Ben Mildenhall, Philipp Henzler, Keunhong Park, Ruiqi Gao, Daniel Watson, Pratul P. Srinivasan, Dor Verbin, Jonathan T. Barron, Ben Poole, Aleksander Holynski*<br>
CVPR 2024, 5 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02981)] [[Project](https://reconfusion.github.io/)]

**DreamControl: Control-Based Text-to-3D Generation with 3D Self-Prior**<br>
*Tianyu Huang, Yihan Zeng, Zhilu Zhang, Wan Xu, Hang Xu, Songcen Xu, Rynson W. H. Lau, Wangmeng Zuo*<br>
CVPR 2024, 11 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.06439)] [[Code](https://github.com/tyhuang0428/DreamControl)]

**Text-Image Conditioned Diffusion for Consistent Text-to-3D Generation**<br>
*Yuze He, Yushi Bai, Matthieu Lin, Jenny Sheng, Yubin Hu, Qi Wang, Yu-Hui Wen, Yong-Jin Liu*<br>
arXiv preprint, 19 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.11774)]

**Carve3D: Improving Multi-view Reconstruction Consistency for Diffusion Models with RL Finetuning**<br>
*Desai Xie, Jiahao Li, Hao Tan, Xin Sun, Zhixin Shu, Yi Zhou, Sai Bi, Sören Pirk, Arie E. Kaufman*<br>
CVPR 2024, 21 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.13980)] [[Project](https://desaixie.github.io/carve-3d/)] [[Code](https://github.com/desaixie/carve3d)]

**Inpaint4DNeRF: Promptable Spatio-Temporal NeRF Inpainting with Generative Diffusion Models**<br>
*Han Jiang, Haosen Sun, Ruoxuan Li, Chi-Keung Tang, Yu-Wing Tai*<br>
arXiv preprint, 30 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2401.00208)]

**SIGNeRF: Scene Integrated Generation for Neural Radiance Fields**<br>
*Jan-Niklas Dihlmann, Andreas Engelhardt, Hendrik Lensch*<br>
arXiv preprint, 3 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.01647)] [[Project](https://signerf.jdihlmann.com/)] [[Code](https://github.com/cgtuebingen/SIGNeRF)] [[Video](https://www.youtube.com/playlist?list=PL5y23CB9WmildtW3QyMEi3arXg06zB4ex)]

**GO-NeRF: Generating Virtual Objects in Neural Radiance Fields**<br>
*Peng Dai, Feitong Tan, Xin Yu, Yinda Zhang, Xiaojuan Qi*<br>
arXiv preprint, 11 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.05750)] [[Project](https://daipengwa.github.io/GO-NeRF/)]

**Sketch2NeRF: Multi-view Sketch-guided Text-to-3D Generation**<br>
*Minglin Chen, Longguang Wang, Weihao Yuan, Yukun Wang, Zhe Sheng, Yisheng He, Zilong Dong, Liefeng Bo, Yulan Guo*<br>
arXiv preprint, 25 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.14257)]

**ReplaceAnything3D:Text-Guided 3D Scene Editing with Compositional Neural Radiance Fields**<br>
*Edward Bartrum, Thu Nguyen-Phuoc, Chris Xie, Zhengqin Li, Numair Khan, Armen Avetisyan, Douglas Lanman, Lei Xiao*<br>
arXiv preprint, 31 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.17895)] [[Project](https://replaceanything3d.github.io/)]

**ViewFusion: Learning Composable Diffusion Models for Novel View Synthesis**<br>
*Bernard Spiegl, Andrea Perin, Stéphane Deny, Alexander Ilin*<br>
arXiv preprint, 5 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.02906)]

**VP3D: Unleashing 2D Visual Prompt for Text-to-3D Generation**<br>
*Yang Chen, Yingwei Pan, Haibo Yang, Ting Yao, Tao Mei*<br>
CVPR 2024, 25 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.17001)] [[Project](https://vp3d-cvpr24.github.io/)]

**FlexiDreamer: Single Image-to-3D Generation with FlexiCubes**<br>
*Ruowen Zhao, Zhengyi Wang, Yikai Wang, Zihan Zhou, Jun Zhu*<br>
arXiv preprint, 1 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.00987)] [[Project](https://flexidreamer.github.io/)] [[Code](https://github.com/zhaorw02/FlexiDreamer)]

**SC4D: Sparse-Controlled Video-to-4D Generation and Motion Transfer**<br>
*Zijie Wu, Chaohui Yu, Yanqin Jiang, Chenjie Cao, Fan Wang, Xiang Bai*<br>
arXiv preprint, 4 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.03736)] [[Project](https://sc4d.github.io/)] [[Code](https://github.com/JarrentWu1031/SC4D)] [[Video](https://www.youtube.com/watch?v=SkpTEuX4B5c)]

**Magic-Boost: Boost 3D Generation with Mutli-View Conditioned Diffusion**<br>
*Fan Yang, Jianfeng Zhang, Yichun Shi, Bowen Chen, Chenxu Zhang, Huichao Zhang, Xiaofeng Yang, Jiashi Feng, Guosheng Lin*<br>
arXiv preprint, 9 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.06429)]

**Enhancing 3D Fidelity of Text-to-3D using Cross-View Correspondences**<br>
*Seungwook Kim, Kejie Li, Xueqing Deng, Yichun Shi, Minsu Cho, Peng Wang*<br>
CVPR 2024, 16 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.10603)]

**MeshLRM: Large Reconstruction Model for High-Quality Mesh**<br>
*Xinyue Wei, Kai Zhang, Sai Bi, Hao Tan, Fujun Luan, Valentin Deschaintre, Kalyan Sunkavalli, Hao Su, Zexiang Xu*<br>
arXiv preprint, 18 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.12385)] [[Project](https://sarahweiii.github.io/meshlrm/)]

**SketchDream: Sketch-based Text-to-3D Generation and Editing**<br>
*Feng-Lin Liu, Hongbo Fu, Yu-Kun Lai, Lin Gao*<br>
arXiv preprint, 10 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.06461)]

**4Diffusion: Multi-view Video Diffusion Model for 4D Generation**<br>
*Haiyu Zhang, Xinyuan Chen, Yaohui Wang, Xihui Liu, Yunhong Wang, Yu Qiao*<br>
arXiv preprint, 31 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.20674)] [[Project](https://aejion.github.io/4diffusion/)] [[Code](https://github.com/aejion/4Diffusion)]

**Rethinking Score Distillation as a Bridge Between Image Distributions**<br>
*David McAllister, Songwei Ge, Jia-Bin Huang, David W. Jacobs, Alexei A. Efros, Aleksander Holynski, Angjoo Kanazawa*<br>
arXiv preprint, 13 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.09417)] [[Project](https://sds-bridge.github.io/)]

**Preserving Identity with Variational Score for General-purpose 3D Editing**<br>
*Duong H. Le, Tuan Pham, Aniruddha Kembhavi, Stephan Mandt, Wei-Chiu Ma, Jiasen Lu*<br>
arXiv preprint, 13 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.08953)]

**Generative Lifting of Multiview to 3D from Unknown Pose: Wrapping NeRF inside Diffusion**<br>
*Xin Yuan, Rana Hanocka, Michael Maire*<br>
arXiv preprint, 11 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.06972)]

**C3DAG: Controlled 3D Animal Generation using 3D pose guidance**<br>
*Sandeep Mishra, Oindrila Saha, Alan C. Bovik*<br>
arXiv preprint, 11 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.07742)]

**OrientDream: Streamlining Text-to-3D Generation**<br>
*Yuzhong Huang, Zhong Li, Zhang Chen, Zhiyuan Ren, Guosheng Lin, Fred Morstatter, Yi Xu*<br>
arXiv preprint, 14 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.10000)]

**Director3D: Real-world Camera Trajectory and 3D Scene Generation from Text**<br>
*Xinyang Li, Zhangyu Lai, Linning Xu, Yansong Qu, Liujuan Cao, Shengchuan Zhang, Bo Dai, Rongrong Ji*<br>
arXiv preprint, 25 jUN 2024<br>
[[arXiv](https://arxiv.org/abs/2406.17601)] [[Code](https://github.com/imlixinyang/director3d)]

**A3D: Does Diffusion Dream about 3D Alignment?**<br>
*Savva Ignatyev, Nina Konovalova, Daniil Selikhanovych, Nikolay Patakin, Oleg Voynov, Dmitry Senushkin, Alexander Filippov, Anton Konushin, Peter Wonka, Evgeny Burnaev*<br>
arXiv preprint, 21 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.15020)]

**DreamDissector: Learning Disentangled Text-to-3D Generation from 2D Diffusion Priors**<br>
*Zizheng Yan, Jiapeng Zhou, Fanpeng Meng, Yushuang Wu, Lingteng Qiu, Zisheng Ye, Shuguang Cui, Guanying Chen, Xiaoguang Han*<br>
ECCV 2024, 23 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.16260)] [[Project](https://chester256.github.io/dreamdissector/)]

**HOTS3D: Hyper-Spherical Optimal Transport for Semantic Alignment of Text-to-3D Generation**<br>
*Zezeng Li, Weimin Wang, WenHai Li, Na Lei, Xianfeng Gu*<br>
arXiv preprint, 19 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.14419)]

**DreamCatalyst: Fast and High-Quality 3D Editing via Controlling Editability and Identity**<br>
*Jiwook Kim, Seonho Lee, Jaeyo Shin, Jiho Choi, Hyunjung Shim*<br>
arXiv preprint, 16 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.11394)] [[Project](https://dream-catalyst.github.io/)]

## Generalization

**Local Implicit Ray Function for Generalizable Radiance Field Representation**<br>
*Xin Huang, Qi Zhang, Ying Feng, Xiaoyu Li, Xuan Wang, Qing Wang*<br>
CVPR 2023, 25 Apr 2023<br>
[[arXiv](https://arxiv.org/abs/2304.12746)] [[Project](https://xhuangcv.github.io/lirf/)] [[Video](https://www.bilibili.com/video/BV1nm4y14743/)]

**MuRF: Multi-Baseline Radiance Fields**<br>
*Haofei Xu, Anpei Chen, Yuedong Chen, Christos Sakaridis, Yulun Zhang, Marc Pollefeys, Andreas Geiger, Fisher Yu*<br>
CVPR 2024, 7 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.04565)] [[Project](https://haofeixu.github.io/murf/)] [[Code](https://github.com/autonomousvision/murf)]

**GD^2-NeRF: Generative Detail Compensation via GAN and Diffusion for One-shot Generalizable Neural Radiance Fields**<br>
*Xiao Pan, Zongxin Yang, Shuai Bai, Yi Yang*<br>
arXiv preprint, 1 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.00616)]

**Learning Robust Generalizable Radiance Field with Visibility and Feature Augmented Point Representation**<br>
*Jiaxu Wang, Ziyi Zhang, Renjing Xu*<br>
arXiv preprint, 25 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.14354)]

**Generalizable Novel-View Synthesis using a Stereo Camera**<br>
*Haechan Lee, Wonjoon Jin, Seung-Hwan Baek, Sunghyun Cho*<br>
CVPR 2024, 21 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.13541)] [[Project](https://jinwonjoon.github.io/stereonerf/)] [[Code](https://github.com/Haechan21/StereoNeRF)]

**Geometry-aware Reconstruction and Fusion-refined Rendering for Generalizable Neural Radiance Fields**<br>
*Tianqi Liu, Xinyi Ye, Min Shi, Zihao Huang, Zhiyu Pan, Zhan Peng, Zhiguo Cao*<br>
CVPR 2024, 26 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.17528)] [[Project](https://gefucvpr24.github.io/)] [[Code](https://github.com/TQTQliu/GeFu)]


:fire:**LaRa: Efficient Large-Baseline Radiance Fields**<br>
*Anpei Chen, Haofei Xu, Stefano Esposito, Siyu Tang, Andreas Geiger*<br>
arXiv preprint, 5 Jul 2024<br>
<details span>
<summary><b>Abstract</b></summary>
Radiance field methods have achieved photorealistic novel view synthesis and geometry reconstruction. But they are mostly applied in per-scene optimization or small-baseline settings. While several recent works investigate feed-forward reconstruction with large baselines by utilizing transformers, they all operate with a standard global attention mechanism and hence ignore the local nature of 3D reconstruction. We propose a method that unifies local and global reasoning in transformer layers, resulting in improved quality and faster convergence. Our model represents scenes as Gaussian Volumes and combines this with an image encoder and Group Attention Layers for efficient feed-forward reconstruction. Experimental results demonstrate that our model, trained for two days on four GPUs, demonstrates high fidelity in reconstructing 360 deg radiance fields, and robustness to zero-shot and out-of-domain testing. Our project Page: this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2407.04699)]<br>


**GMT: Enhancing Generalizable Neural Rendering via Geometry-Driven Multi-Reference Texture Transfer**<br>
*Youngho Yoon, Hyun-Kurl Jang, Kuk-Jin Yoon*<br>
ECCV 2024, 1 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.00672)] [[Code](https://github.com/yh-yoon/GMT)]

**OPONeRF: One-Point-One NeRF for Robust Neural Rendering**<br>
*Yu Zheng, Yueqi Duan, Kangfu Zheng, Hongru Yan, Jiwen Lu, Jie Zhou*<br>
arXiv preprint, 30 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.20043)] [[Project](https://yzheng97.github.io/OPONeRF/)] [[Code](https://github.com/yzheng97/OPONeRF)]

**Towards Degradation-Robust Reconstruction in Generalizable NeRF**<br>
*Chan Ho Park, Ka Leong Cheng, Zhicheng Wang, Qifeng Chen*<br>
arXiv preprint, 18 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.11691)]

## Model Compression

**HollowNeRF: Pruning Hashgrid-Based NeRFs with Trainable Collision Mitigation**<br>
*Xiufeng Xie, Riccardo Gherardi, Zhihong Pan, Stephen Huang*<br>
ICCV 2023, 19 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.10122)]

**SPC-NeRF: Spatial Predictive Compression for Voxel Based Radiance Field**<br>
*Zetian Song, Wenhong Duan, Yuhuai Zhang, Shiqi Wang, Siwei Ma, Wen Gao*<br>
arXiv preprint, 26 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.16366)]

**NeRFCodec: Neural Feature Compression Meets Neural Radiance Fields for Memory-Efficient Scene Representation**<br>
*Sicheng Li, Hao Li, Yiyi Liao, Lu Yu*<br>
CVPR 2024, 2 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.02185)]

**How Far Can We Compress Instant-NGP-Based NeRF?**<br>
*Yihang Chen, Qianyi Wu, Mehrtash Harandi, Jianfei Cai*<br>
arXiv preprint, 6 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.04101)] [[Project](https://yihangchen-ee.github.io/project_cnc/)] [[Code](https://github.com/yihangchen-ee/cnc/)]

**Explicit_NeRF_QA: A Quality Assessment Database for Explicit NeRF Model Compression**<br>
*Yuke Xing, Qi Yang, Kaifa Yang, Yilin Xu, Zhu Li*<br>
arXiv preprint, 11 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.08165)]

**HPC: Hierarchical Progressive Coding Framework for Volumetric Video**<br>
*Zihan Zheng, Houqiang Zhong, Qiang Hu, Xiaoyun Zhang, Li Song, Ya Zhang, Yanfeng Wang*<br>
arXiv preprint, 12 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.09026)]

**Lagrangian Hashing for Compressed Neural Field Representations**<br>
*Shrisudhan Govindarajan, Zeno Sambugaro, Akhmedkhan (Ahan)Shabanov, Towaki Takikawa, Daniel Rebain, Weiwei Sun, Nicola Conci, Kwang Moo Yi, Andrea Tagliasacchi*<br>
arXiv preprint, 9 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.05334)] [[Project](https://theialab.github.io/laghashes/)]

**Plenoptic PNG: Real-Time Neural Radiance Fields in 150 KB**<br>
*Jae Yong Lee, Yuqun Wu, Chuhang Zou, Derek Hoiem, Shenlong Wang*<br>
arXiv preprint, 24 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.15689)]

**Disentangled Generation and Aggregation for Robust Radiance Fields**<br>
*Shihe Shen, Huachen Gao, Wangze Xu, Rui Peng, Luyang Tang, Kaiqiang Xiong, Jianbo Jiao, Ronggang Wang*<br>
ECCV 2024, 24 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.15715)] [[Project](https://gaohchen.github.io/DiGARR/)]

## NeRF Based 2D High Quality Image Synthesis

**GIRAFFE: Representing Scenes as Compositional Generative Neural Feature Fields**<br>
*Michael Niemeyer, Andreas Geiger*<br>
CVPR 2012, 24 Nov 2020<br>
[[arXiv](https://arxiv.org/abs/2011.12100)] [[Project](http://bit.ly/giraffe-project)] [[Github](https://github.com/autonomousvision/giraffe)]

## SDF Based Reconstruction / Other Geometry Based Reconstruction

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
<details span>
<summary><b>Abstract</b></summary>
We present a novel neural surface reconstruction method, called NeuS, for reconstructing objects and scenes with high fidelity from 2D image inputs. Existing neural surface reconstruction approaches, such as DVR and IDR, require foreground mask as supervision, easily get trapped in local minima, and therefore struggle with the reconstruction of objects with severe self-occlusion or thin structures. Meanwhile, recent neural methods for novel view synthesis, such as NeRF and its variants, use volume rendering to produce a neural scene representation with robustness of optimization, even for highly complex objects. However, extracting high-quality surfaces from this learned implicit representation is difficult because there are not sufficient surface constraints in the representation. In NeuS, we propose to represent a surface as the zero-level set of a signed distance function (SDF) and develop a new volume rendering method to train a neural SDF representation. We observe that the conventional volume rendering method causes inherent geometric errors (i.e. bias) for surface reconstruction, and therefore propose a new formulation that is free of bias in the first order of approximation, thus leading to more accurate surface reconstruction even without the mask supervision. Experiments on the DTU dataset and the BlendedMVS dataset show that NeuS outperforms the state-of-the-arts in high-quality surface reconstruction, especially for objects and scenes with complex structures and self-occlusion.
</details>

[[arXiv](https://arxiv.org/abs/2106.10689)] [[Project](https://lingjie0206.github.io/papers/NeuS/)] [[Github](https://github.com/Totoro97/NeuS)]<br>

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

:fire:**TensoSDF: Roughness-aware Tensorial Representation for Robust Geometry and Material Reconstruction**<br>
*Jia Li, Lu Wang, Lei Zhang, Beibei Wang*<br>
SIGGRAPH 2024, 5 Feb 2024<br>
<details span>
<summary><b>Abstract</b></summary>
Reconstructing objects with realistic materials from multi-view images is problematic, since it is highly ill-posed. Although the neural reconstruction approaches have exhibited impressive reconstruction ability, they are designed for objects with specific materials (e.g., diffuse or specular materials). To this end, we propose a novel framework for robust geometry and material reconstruction, where the geometry is expressed with the implicit signed distance field (SDF) encoded by a tensorial representation, namely TensoSDF. At the core of our method is the roughness-aware incorporation of the radiance and reflectance fields, which enables a robust reconstruction of objects with arbitrary reflective materials. Furthermore, the tensorial representation enhances geometry details in the reconstructed surface and reduces the training time. Finally, we estimate the materials using an explicit mesh for efficient intersection computation and an implicit SDF for accurate representation. Consequently, our method can achieve more robust geometry reconstruction, outperform the previous works in terms of relighting quality, and reduce 50% training times and 70% inference time.
</details>

[[arXiv](https://arxiv.org/abs/2402.02771)]<br>

**H2O-SDF: Two-phase Learning for 3D Indoor Reconstruction using Object Surface Fields**<br>
*Minyoung Park, Mirae Do, YeonJae Shin, Jaeseok Yoo, Jongkwang Hong, Joongrock Kim, Chul Lee*<br>
arXiv preprint, 13 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.08138)]

**MonoPatchNeRF: Improving Neural Radiance Fields with Patch-based Monocular Guidance**<br>
*Yuqun Wu, Jae Yong Lee, Chuhang Zou, Shenlong Wang, Derek Hoiem*<br>
arXiv preprint, 12 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.08252)]

**ActiveNeuS: Active 3D Reconstruction using Neural Implicit Surface Uncertainty**<br>
*Hyunseo Kim, Hyeonseo Yang, Taekyung Kim, YoonSung Kim, Jin-Hwa Kim, Byoung-Tak Zhang*<br>
arXiv preprint, 4 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.02568)]

**RPBG: Towards Robust Neural Point-based Graphics in the Wild**<br>
*Qingtian Zhu, Zizhuang Wei, Zhongtian Zheng, Yifan Zhan, Zhuyu Yao, Jiawang Zhang, Kejian Wu, Yinqiang Zheng*<br>
arXiv preprint, 9 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.05663)] [[Code](https://github.com/QT-Zhu/RPBG)]

**LDM: Large Tensorial SDF Model for Textured Mesh Generation**<br>
*Rengan Xie, Wenting Zheng, Kai Huang, Yizheng Chen, Qi Wang, Qi Ye, Wei Chen, Yuchi Huo*<br>
arXiv preprint, 23 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.14580)]

**RaNeuS: Ray-adaptive Neural Surface Reconstruction**<br>
*Yida Wang, David Joseph Tan, Nassir Navab, Federico Tombari*<br>
3DV 2024, 14 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.09801)]

**Neural Geometry Processing via Spherical Neural Surfaces**<br>
*Romy Williamson, Niloy J. Mitra*<br>
arXiv preprint, 10 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.07755)]

**ActiveNeRF: Learning Accurate 3D Geometry by Active Pattern Projection**<br>
*Jianyu Tao, Changping Hu, Edward Yang, Jing Xu, Rui Chen*<br>
arXiv preprint, 13 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.06592)]

**MGFs: Masked Gaussian Fields for Meshing Building based on Multi-View Images**<br>
*Tengfei Wang, Zongqian Zhan, Rui Xia, Linxia Ji, Xin Wang*<br>
arXiv preprint, 6 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.03060)]

**Neural Surface Reconstruction and Rendering for LiDAR-Visual Systems**<br>
*Jianheng Liu, Chunran Zheng, Yunfei Wan, Bowen Wang, Yixi Cai, Fu Zhang*<br>
arXiv preprint, 9 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.05310)] [[Code](https://github.com/hku-mars/M2Mapping)]

**Rethinking Directional Parameterization in Neural Implicit Surface Reconstruction**<br>
*Zijie Jiang, Tianhan Xu, Hiroharu Kato*<br>
ECCV 2024, 11 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.06923)]

## NeRF + Hardware Optimization/Acceleration

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

**Thermal-NeRF: Neural Radiance Fields from an Infrared Camera**<br>
*Tianxiang Ye, Qi Wu, Junyuan Deng, Guoqing Liu, Liu Liu, Songpengcheng Xia, Liang Pang, Wenxian Yu, Ling Pei*<br>
arXiv preprint, 15 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.10340)]

**URS-NeRF: Unordered Rolling Shutter Bundle Adjustment for Neural Radiance Fields**<br>
*Bo Xu, Ziao Liu, Mengqi Guo, Jiancheng Li, Gim Hee Li*<br>
arXiv preprint, 15 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.10119)]

**Spike-NeRF: Neural Radiance Field Based On Spike Camera**<br>
*Yijia Guo, Yuanxi Bai, Liwen Hu, Mianzhi Liu, Ziyi Guo, Lei Ma, Tiejun Huang*<br>
ICME 2024, 25 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.16410)]

**Mitigating Motion Blur in Neural Radiance Fields with Events and Frames**<br>
*Marco Cannici, Davide Scaramuzza*<br>
CVPR 2024, 28 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.19780)]

**SpikeNVS: Enhancing Novel View Synthesis from Blurry Images via Spike Camera**<br>
*Gaole Dai, Zhenyu Wang, Qinwen Xu, Wen Cheng, Ming Lu, Boxing Shi, Shanghang Zhang, Tiejun Huang*<br>
arXiv preprint, 10 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.06710)]

**Radiance Fields from Photons**<br>
*Sacha Jungerman, Mohit Gupta*<br>
arXiv preprint, 12 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.09386)]

**TeX-NeRF: Neural Radiance Fields from Pseudo-TeX Vision**<br>
*Chonghao Zhong, Chao Xu*<br>
arXiv preprint, 7 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.04873)]

**NeRF-enabled Analysis-Through-Synthesis for ISAR Imaging of Small Everyday Objects with Sparse and Noisy UWB Radar Data**<br>
*Md Farhan Tasnim Oshim, Albert Reed, Suren Jayasuriya, Tauhidur Rahman*<br>
arXiv preprint, 14 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.10085)]

## NeRF + Light Field Rendering

**DirectL: Efficient Radiance Fields Rendering for 3D Light Field Displays**<br>
*Zongyuan Yang, Baolin Liu, Yingde Song, Yongping Xiong, Lan Yi, Zhaohe Zhang, Xunbo Yu*<br>
arXiv preprint, 19 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.14053)] [[Project](https://direct-l.github.io/)]

## NeRF + Point Cloud / LiDAR

:fire:**Point-NeRF: Point-based Neural Radiance Fields**<br>
*Qiangeng Xu, Zexiang Xu, Julien Philip, Sai Bi, Zhixin Shu, Kalyan Sunkavalli, Ulrich Neumann*<br>
CVPR 2022, 21 Jan 2022 <br>
<details span>
<summary><b>Abstract</b></summary>
Volumetric neural rendering methods like NeRF generate high-quality view synthesis results but are optimized per-scene leading to prohibitive reconstruction time. On the other hand, deep multi-view stereo methods can quickly reconstruct scene geometry via direct network inference. Point-NeRF combines the advantages of these two approaches by using neural 3D point clouds, with associated neural features, to model a radiance field. Point-NeRF can be rendered efficiently by aggregating neural point features near scene surfaces, in a ray marching-based rendering pipeline. Moreover, Point-NeRF can be initialized via direct inference of a pre-trained deep network to produce a neural point cloud; this point cloud can be finetuned to surpass the visual quality of NeRF with 30X faster training time. Point-NeRF can be combined with other 3D reconstruction methods and handles the errors and outliers in such methods via a novel pruning and growing mechanism. The experiments on the DTU, the NeRF Synthetics , the ScanNet and the Tanks and Temples datasets demonstrate Point-NeRF can surpass the existing methods and achieve the state-of-the-art results.
</details>

[[arXiv](https://arxiv.org/abs/2201.08845)] [[Project](https://xharlie.github.io/projects/project_sites/pointnerf/index.html)] [[Github](https://github.com/Xharlie/pointnerf)]<br>

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

**Just Add $100 More: Augmenting NeRF-based Pseudo-LiDAR Point Cloud for Resolving Class-imbalance Problem**<br>
*Mincheol Chang, Siyeong Lee, Jinkyu Kim, Namil Kim*<br>
arXiv preprint, 18 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.11573)]

**GPN: Generative Point-based NeRF**<br>
*Haipeng Wang*<br>
arXiv preprint, 12 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.08312)]

**Hologram: Realtime Holographic Overlays via LiDAR Augmented Reconstruction**<br>
*Ekansh Agrawal*<br>
arXiv preprint, 12 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.07178)]

**A Probabilistic Formulation of LiDAR Mapping with Neural Radiance Fields**<br>
*Matthew McDermott, Jason Rife*<br>
arXiv preprint, 4 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.01725)] [[Code](https://github.com/mcdermatt/PLINK)]

## NeRF + Auto Data Collection

**AutoNeRF: Training Implicit Scene Representations with Autonomous Agents**<br>
*Pierre Marza, Laetitia Matignon, Olivier Simonin, Dhruv Batra, Christian Wolf, Devendra Singh Chaplot*<br>
arXiv preprint, 21 Apr 2023 <br>
[[arXiv](https://arxiv.org/abs/2304.11241)] [[Project](https://pierremarza.github.io/projects/autonerf/)] [[Video](https://www.bilibili.com/video/BV1iX4y1m7op/)]

**NerfBridge: Bringing Real-time, Online Neural Radiance Field Training to Robotics**<br>
*Javier Yu, Jun En Low, Keiko Nagami, Mac Schwager*<br>
ICRA 2023, 16 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.09761)] [[Github](https://github.com/javieryu/nerf_bridge)] [[Video](https://www.bilibili.com/video/BV1Bg4y1F7gD/)]


## NeRF + Avatar/Talking Head

:fire:**AD-NeRF: Audio Driven Neural Radiance Fields for Talking Head Synthesis**<br>
*Yudong Guo, Keyu Chen, Sen Liang, Yong-Jin Liu, Hujun Bao, Juyong Zhang*<br>
ICCV 2021, 20 Mar 2021 <br>
<details span>
<summary><b>Abstract</b></summary>
Generating high-fidelity talking head video by fitting with the input audio sequence is a challenging problem that receives considerable attentions recently. In this paper, we address this problem with the aid of neural scene representation networks. Our method is completely different from existing methods that rely on intermediate representations like 2D landmarks or 3D face models to bridge the gap between audio input and video output. Specifically, the feature of input audio signal is directly fed into a conditional implicit function to generate a dynamic neural radiance field, from which a high-fidelity talking-head video corresponding to the audio signal is synthesized using volume rendering. Another advantage of our framework is that not only the head (with hair) region is synthesized as previous methods did, but also the upper body is generated via two individual neural radiance fields. Experimental results demonstrate that our novel framework can (1) produce high-fidelity and natural results, and (2) support free adjustment of audio signals, viewing directions, and background images. Code is available at this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2103.11078)] [[Project](https://yudongguo.github.io/ADNeRF/)] [[Github](https://github.com/YudongGuo/AD-NeRF/)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
This paper presents a 3D generative model that uses diffusion models to automatically generate 3D digital avatars represented as neural radiance fields. A significant challenge in generating such avatars is that the memory and processing costs in 3D are prohibitive for producing the rich details required for high-quality avatars. To tackle this problem we propose the roll-out diffusion network (Rodin), which represents a neural radiance field as multiple 2D feature maps and rolls out these maps into a single 2D feature plane within which we perform 3D-aware diffusion. The Rodin model brings the much-needed computational efficiency while preserving the integrity of diffusion in 3D by using 3D-aware convolution that attends to projected features in the 2D feature plane according to their original relationship in 3D. We also use latent conditioning to orchestrate the feature generation for global coherence, leading to high-fidelity avatars and enabling their semantic editing based on text prompts. Finally, we use hierarchical synthesis to further enhance details. The 3D avatars generated by our model compare favorably with those produced by existing generative techniques. We can generate highly detailed avatars with realistic hairstyles and facial hair like beards. We also demonstrate 3D avatar generation from image or text as well as text-guided editability.
</details>

[[arXiv](https://arxiv.org/abs/2212.06135)] [[Project](https://3d-avatar-diffusion.microsoft.com/)] [[Video](https://www.bilibili.com/video/BV1m44y1Z7gr/)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
Representing human performance at high-fidelity is an essential building block in diverse applications, such as film production, computer games or videoconferencing. To close the gap to production-level quality, we introduce HumanRF, a 4D dynamic neural scene representation that captures full-body appearance in motion from multi-view video input, and enables playback from novel, unseen viewpoints. Our novel representation acts as a dynamic video encoding that captures fine details at high compression rates by factorizing space-time into a temporal matrix-vector decomposition. This allows us to obtain temporally coherent reconstructions of human actors for long sequences, while representing high-resolution details even in the context of challenging motion. While most research focuses on synthesizing at resolutions of 4MP or lower, we address the challenge of operating at 12MP. To this end, we introduce ActorsHQ, a novel multi-view dataset that provides 12MP footage from 160 cameras for 16 sequences with high-fidelity, per-frame mesh reconstructions. We demonstrate challenges that emerge from using such high-resolution data and show that our newly introduced HumanRF effectively leverages this data, making a significant step towards production-level quality novel view synthesis.
</details>

[[arXiv](https://arxiv.org/abs/2305.06356)] [[Project](https://synthesiaresearch.github.io/humanrf/)] [[Github](https://github.com/synthesiaresearch/humanrf)] [[Video](https://www.bilibili.com/video/BV1ug4y1V7cy/)] [[Notes](./paper_discussions/HumanRF.md)]<br>

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

**High-Quality Mesh Blendshape Generation from Face Videos via Neural Inverse Rendering**<br>
*Xin Ming, Jiawei Li, Jingwang Ling, Libo Zhang, Feng Xu*<br>
arXiv preprint, 16 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.08398)]

**Tri^2-plane: Volumetric Avatar Reconstruction with Feature Pyramid**<br>
*Luchuan Song, Pinxin Liu, Lele Chen, Celong Liu, Chenliang Xu*<br>
arXiv preprint, 17 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.09386)]

**Template-Free Single-View 3D Human Digitalization with Diffusion-Guided LRM**<br>
*Zhenzhen Weng, Jingyuan Liu, Hao Tan, Zhan Xu, Yang Zhou, Serena Yeung-Levy, Jimei Yang*<br>
arXiv preprint, 22 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.12175)]

**NeRF-AD: Neural Radiance Field with Attention-based Disentanglement for Talking Face Synthesis**<br>
*Chongke Bi, Xiaoxing Liu, Zhilei Liu*<br>
ICASSP 2024, 23 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.12568)]

**Emo-Avatar: Efficient Monocular Video Style Avatar through Texture Rendering**<br>
*Pinxin Liu, Luchuan Song, Daoan Zhang, Hang Hua, Yunlong Tang, Huaijin Tu, Jiebo Luo, Chenliang Xu*<br>
arXiv preprint, 1 Feb 2024<br>
[[arXiv](https://browse.arxiv.org/abs/2402.00827)]

**Learning Dynamic Tetrahedra for High-Quality Talking Head Synthesis**<br>
*Zicheng Zhang, Ruobing Zheng, Ziwen Liu, Congying Han, Tianqi Li, Meng Wang, Tiande Guo, Jingdong Chen, Bonan Li, Ming Yang*<br>
CVPR 2024, 27 Feb, 2024<br>
[[arXiv](https://arxiv.org/abs/2402.17364)]

**DivAvatar: Diverse 3D Avatar Generation with a Single Prompt**<br>
*Weijing Tao, Biwen Lei, Kunhao Liu, Shijian Lu, Miaomiao Cui, Xuansong Xie, Chunyan Miao*<br>
arXiv preprint, 27 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.17292)]

**PKU-DyMVHumans: A Multi-View Video Benchmark for High-Fidelity Dynamic Human Modeling**<br>
*Xiaoyun Zheng, Liwei Liao, Xufeng Li, Jianbo Jiao, Rongjie Wang, Feng Gao, Shiqi Wang, Ronggang Wang*<br>
CVPR 2024, 24 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.16080)] [[Project](https://pku-dymvhumans.github.io/] [[Code](https://github.com/zhengxyun/PKU-DyMVHumans)] [[Video](https://www.youtube.com/watch?v=4Q6B-nAIrZc)]

**MI-NeRF: Learning a Single Face NeRF from Multiple Identities**<br>
*Aggelina Chatziagapi, Grigorios G. Chrysos, Dimitris Samaras*<br>
arXiv preprint, 29 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.19920)] [[Project](https://aggelinacha.github.io/MI-NeRF/)]

**Talk3D: High-Fidelity Talking Portrait Synthesis via Personalized 3D Generative Prior**<br>
*Jaehoon Ko, Kyusun Cho, Joungbin Lee, Heeji Yoon, Sangmin Lee, Sangjun Ahn, Seungryong Kim*<br>
arXiv preprint, 29 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.20153)] [[Project](https://ku-cvlab.github.io/Talk3D/)] [[Code](https://github.com/KU-CVLAB/Talk3D)] [[Video](https://www.youtube.com/watch?v=OkQtwWN0q00)]

**StructLDM: Structured Latent Diffusion for 3D Human Generation**<br>
*Tao Hu, Fangzhou Hong, Ziwei Liu*<br>
arXiv preprint, 1 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.01241)] [[Project](https://taohuumd.github.io/projects/StructLDM/)] [[Code](https://github.com/TaoHuUMD/StructLDM)] [[Video](https://www.youtube.com/watch?v=cZ3PGqOcRqI)]

**MagicMirror: Fast and High-Quality Avatar Generation with a Constrained Search Space**<br>
*Armand Comas-Massagué, Di Qiu, Menglei Chai, Marcel Bühler, Amit Raj, Ruiqi Gao, Qiangeng Xu, Mark Matthews, Paulo Gotardo, Octavia Camps, Sergio Orts-Escolano, Thabo Beeler*<br>
arXiv preprint, 1 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.01296)]

**GHNeRF: Learning Generalizable Human Features with Efficient Neural Radiance Fields**<br>
*Arnab Dey, Di Yang, Rohith Agaram, Antitza Dantcheva, Andrew I. Comport, Srinath Sridhar, Jean Martinet*<br>
arXiv preprint, 9 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.06246)]

**HFNeRF: Learning Human Biomechanic Features with Neural Radiance Fields**<br>
*Arnab Dey, Di Yang, Antitza Dantcheva, Jean Martinet*<br>
arXiv preprint, 9 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.06152)]

**ArtNeRF: A Stylized Neural Field for 3D-Aware Cartoonized Face Synthesis**<br>
*Zichen Tang, Hongyu Yang*<br>
arXiv preprint, 21 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.13711)]

**Embedded Representation Learning Network for Animating Styled Video Portrait**<br>
*Tianyong Wang, Xiangyu Liang, Wangguandong Zheng, Dan Niu, Haifeng Xia, Siyu Xia*<br>
arXiv preprint, 29 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.19038)]

**NeRFFaceSpeech: One-shot Audio-driven 3D Talking Head Synthesis via Generative Prior**<br>
*Gihoon Kim, Kwanggyoon Seo, Sihun Cha, Junyong Noh*<br>
arXiv preprint, 9 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.05749)]

**HINT: Learning Complete Human Neural Representations from Limited Viewpoints**<br>
*Alessandro Sanvito, Andrea Ramazzina, Stefanie Walz, Mario Bijelic, Felix Heide*<br>
arXiv preprint, 30 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.19712)]

**Representing Animatable Avatar via Factorized Neural Fields**<br>
*Chunjin Song, Zhijie Wu, Bastian Wandt, Leonid Sigal, Helge Rhodin*<br>
arXiv preprint, 2 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.00637)]

**NLDF: Neural Light Dynamic Fields for Efficient 3D Talking Head Generation**<br>
*Niu Guanchen*<br>
arXiv preprint, 17 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.11259)]

**Semantic Communications for 3D Human Face Transmission with Neural Radiance Fields**<br>
*Guanlin Wu, Zhonghao Lyu, Juyong Zhang, Jie Xu*<br>
arXiv preprint, 19 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.13992)]

**Motion-Oriented Compositional Neural Radiance Fields for Monocular Dynamic Human Modeling**<br>
*Jaehyeok Kim, Dongyoon Wee, Dan Xu*<br>
ECCV 2024, 16 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.11962)] [[Project](https://stevejaehyeok.github.io/publications/moco-nerf/)]

:fire:**S^3D-NeRF: Single-Shot Speech-Driven Neural Radiance Field for High Fidelity Talking Head Synthesis**<br>
*Dongze Li, Kang Zhao, Wei Wang, Yifeng Ma, Bo Peng, Yingya Zhang, Jing Dong*<br>
ECCV 2024, 18 Aug 2024<br>
<details span>
<summary><b>Abstract</b></summary>
Talking head synthesis is a practical technique with wide applications. Current Neural Radiance Field (NeRF) based approaches have shown their superiority on driving one-shot talking heads with videos or signals regressed from audio. However, most of them failed to take the audio as driven information directly, unable to enjoy the flexibility and availability of speech. Since mapping audio signals to face deformation is non-trivial, we design a Single-Shot Speech-Driven Neural Radiance Field (S^3D-NeRF) method in this paper to tackle the following three difficulties: learning a representative appearance feature for each identity, modeling motion of different face regions with audio, and keeping the temporal consistency of the lip area. To this end, we introduce a Hierarchical Facial Appearance Encoder to learn multi-scale representations for catching the appearance of different speakers, and elaborate a Cross-modal Facial Deformation Field to perform speech animation according to the relationship between the audio signal and different face regions. Moreover, to enhance the temporal consistency of the important lip area, we introduce a lip-sync discriminator to penalize the out-of-sync audio-visual sequences. Extensive experiments have shown that our S^3D-NeRF surpasses previous arts on both video fidelity and audio-lip synchronization.
</details>

[[arXiv](https://arxiv.org/abs/2408.09347)]<br>

**TalkinNeRF: Animatable Neural Fields for Full-Body Talking Humans**<br>
*Aggelina Chatziagapi, Bindita Chaudhuri, Amit Kumar, Rakesh Ranjan, Dimitris Samaras, Nikolaos Sarafianos*<br>
ECCVW 2024, 25 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.16666)] [[Project](https://aggelinacha.github.io/TalkinNeRF/)]

**LightAvatar: Efficient Head Avatar as Dynamic Neural Light Field**<br>
*Huan Wang, Feitong Tan, Ziqian Bai, Yinda Zhang, Shichen Liu, Qiangeng Xu, Menglei Chai, Anish Prabhu, Rohit Pandey, Sean Fanello, Zeng Huang, Yun Fu*<br>
ECCV 2024 CADL Workshop, 26 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.18057)] [[Code](https://github.com/MingSun-Tse/LightAvatar-TensorFlow)]


**EG-HumanNeRF: Efficient Generalizable Human NeRF Utilizing Human Prior for Sparse View**<br>
*Zhaorong Wang, Yoshihiro Kanamori, Yuki Endo*<br>
arXiv preprint, 16 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.12242)] [[Code](https://github.com/LarsPh/EG-HumanNeRF)]

:fire:**Real-time 3D-aware Portrait Video Relighting**<br>
*Ziqi Cai, Kaiwen Jiang, Shu-Yu Chen, Yu-Kun Lai, Hongbo Fu, Boxin Shi, Lin Gao*<br>
CVPR 2024, 24 Oct 2024<br>
<details span>
<summary><b>Abstract</b></summary>
Synthesizing realistic videos of talking faces under custom lighting conditions and viewing angles benefits various downstream applications like video conferencing. However, most existing relighting methods are either time-consuming or unable to adjust the viewpoints. In this paper, we present the first real-time 3D-aware method for relighting in-the-wild videos of talking faces based on Neural Radiance Fields (NeRF). Given an input portrait video, our method can synthesize talking faces under both novel views and novel lighting conditions with a photo-realistic and disentangled 3D representation. Specifically, we infer an albedo tri-plane, as well as a shading tri-plane based on a desired lighting condition for each video frame with fast dual-encoders. We also leverage a temporal consistency network to ensure smooth transitions and reduce flickering artifacts. Our method runs at 32.98 fps on consumer-level hardware and achieves state-of-the-art results in terms of reconstruction quality, lighting error, lighting instability, temporal consistency and inference speed. We demonstrate the effectiveness and interactivity of our method on various portrait videos with diverse lighting and viewing conditions.
</details>

[[arXiv](https://arxiv.org/abs/2410.18355)] [[Project](http://geometrylearning.com/VideoRelighting/)]<br>

**Efficient Neural Implicit Representation for 3D Human Reconstruction**<br>
*Zexu Huang, Sarah Monazam Erfani, Siying Lu, Mingming Gong*<br>
arXiv preprint, 23 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.17741)] 

**Joker: Conditional 3D Head Synthesis with Extreme Facial Expressions**<br>
*Malte Prinzler, Egor Zakharov, Vanessa Sklyarova, Berna Kabadayi, Justus Thies*<br>
arXiv preprint, 21 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.16395)] [[Project](https://malteprinzler.github.io/projects/joker/)]

## NeRF + Imaging Tasks

:fire:**NeRF in the Dark: High Dynamic Range View Synthesis from Noisy Raw Images**<br>
*Ben Mildenhall, Peter Hedman, Ricardo Martin-Brualla, Pratul Srinivasan, Jonathan T. Barron*<br>
CVPR 2022, 26 Nov 2021 <br>
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Fields (NeRF) is a technique for high quality novel view synthesis from a collection of posed input images. Like most view synthesis methods, NeRF uses tonemapped low dynamic range (LDR) as input; these images have been processed by a lossy camera pipeline that smooths detail, clips highlights, and distorts the simple noise distribution of raw sensor data. We modify NeRF to instead train directly on linear raw images, preserving the scene's full dynamic range. By rendering raw output images from the resulting NeRF, we can perform novel high dynamic range (HDR) view synthesis tasks. In addition to changing the camera viewpoint, we can manipulate focus, exposure, and tonemapping after the fact. Although a single raw image appears significantly more noisy than a postprocessed one, we show that NeRF is highly robust to the zero-mean distribution of raw noise. When optimized over many noisy raw inputs (25-200), NeRF produces a scene representation so accurate that its rendered novel views outperform dedicated single and multi-image deep raw denoisers run on the same wide baseline input images. As a result, our method, which we call RawNeRF, can reconstruct scenes from extremely noisy images captured in near-darkness.
</details>

[[arXiv](https://arxiv.org/abs/2111.13679)] [[Project](https://bmild.github.io/rawnerf/)] [[Github](https://github.com/google-research/multinerf)]<br>

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

**Sharp-NeRF: Grid-based Fast Deblurring Neural Radiance Fields Using Sharpness Prior**<br>
*Byeonghyeon Lee, Howoong Lee, Usman Ali, Eunbyung Park*<br>
WACV 2024, 1 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.00825)] [[Project](https://benhenryl.github.io/SharpNeRF/)] [[Code](https://github.com/benhenryL/SharpNeRF)]

**RustNeRF: Robust Neural Radiance Field with Low-Quality Images**
*Mengfei Li, Ming Lu, Xiaofang Li, Shanghang Zhang*<br>
arXiv preprint, 6 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.03257)]

**Colorizing Monochromatic Radiance Fields**<br>
*Yean Cheng, Renjie Wan, Shuchen Weng, Chengxuan Zhu, Yakun Chang, Boxin Shi*<br>
AAAI 2024, 19 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.12184)] [[Project](https://liquidammonia.github.io/color-nerf/)] [[Code](https://github.com/LiquidAmmonia/colornerf)]

**SMURF: Continuous Dynamics for Motion-Deblurring Radiance Fields**<br>
*Jungho Lee, Dogyoon Lee, Minhyeok Lee, Donghyung Kim, Sangyoun Lee*<br>
arXiv preprint, 12 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.07547)] [[Code](https://github.com/Jho-Yonsei/SMURF)]

**DyBluRF: Dynamic Neural Radiance Fields from Blurry Monocular Video**<br>
*Huiqiang Sun, Xingyi Li, Liao Shen, Xinyi Ye, Ke Xian, Zhiguo Cao*<br>
CVPR 2024, 15 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.10103)] [[Project](https://huiqiang-sun.github.io/dyblurf/)] [[Code](https://github.com/huiqiang-sun/DyBluRF)]

**SCINeRF: Neural Radiance Fields from a Snapshot Compressive Image**<br>
*Yunhao Li, Xiaodong Wang, Ping Wang, Xin Yuan, Peidong Liu*<br>
arXiv preprint, 29 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.20018)] [[Code](https://github.com/WU-CVGL/SCINeRF)]

**DerainNeRF: 3D Scene Estimation with Adhesive Waterdrop Removal**<br>
*Yunhao Li, Jing Wu, Lingzhe Zhao, Peidong Liu*<br>
arXiv preprint, 29 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.20013)]

**IReNe: Instant Recoloring in Neural Radiance Fields**<br>
*Alessio Mazzucchelli, Adrian Garcia-Garcia, Elena Garces, Fernando Rivas-Manzaneque, Francesc Moreno-Noguer, Adrian Penate-Sanchez*<br>
arXiv preprint, 30 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.19876)]

**Bilateral Guided Radiance Field Processing**<br>
*Yuehao Wang, Chaoyi Wang, Bingchen Gong, Tianfan Xue*<br>
SIGGRAPH 2024, 1 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.00448)] [[Project](https://bilarfpro.github.io/)] [[Code](https://github.com/yuehaowang/bilarf)] [[Video](https://www.bilibili.com/video/BV1is421u7C5)]

**Deblurring Neural Radiance Fields with Event-driven Bundle Adjustment**<br>
*Yunshan Qi, Lin Zhu, Yifan Zhao, Nan Bao, Jia Li*<br>
arXiv preprint, 20 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.14360)]

**Style-NeRF2NeRF: 3D Style Transfer From Style-Aligned Multi-View Images**<br>
*Haruo Fujiwara, Yusuke Mukuta, Tatsuya Harada*<br>
arXiv preprint, 19 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.13393)] [[Project](https://haruolabs.github.io/style-n2n/)]

**Sparse-DeRF: Deblurred Neural Radiance Fields from Sparse View**<br>
*Dogyoon Lee, Donghyeong Kim, Jungho Lee, Minhyeok Lee, Seunghoon Lee, Sangyoun Lee*<br>
arXiv preprint, 9 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.06613)] [[Project](https://dogyoonlee.github.io/sparsederf/)]

**PanDORA: Casual HDR Radiance Acquisition for Indoor Scenes**<br>
*Mohammad Reza Karimi Dastjerdi, Frédéric Fortier-Chouinard, Yannick Hold-Geoffroy, Marc Hébert, Claude Demers, Nima Kalantari, Jean-François Lalonde*<br>
arXiv preprint, 8 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.06150)]

**LSE-NeRF: Learning Sensor Modeling Errors for Deblured Neural Radiance Fields with RGB-Event Stereo**<br>
*Wei Zhi Tang, Daniel Rebain, Kostantinos G. Derpanis, Kwang Moo Yi*<br>
arXiv preprint, 9 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.06104)] [[Code](https://github.com/ubc-vision/LSENeRF)]

**Deblur e-NeRF: NeRF from Motion-Blurred Events under High-speed or Low-light Conditions**<br>
*Weng Fei Low, Gim Hee Lee*<br>
ECCV 2024, 26 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.17988)] [[Project](https://wengflow.github.io/deblur-e-nerf/)] [[Code](https://github.com/wengflow/deblur-e-nerf)]

**LuSh-NeRF: Lighting up and Sharpening NeRFs for Low-light Scenes**<br>
*Zefan Qu, Ke Xu, Gerhard Petrus Hancke, Rynson W.H. Lau*<br>
NeurIPS 2024, 11 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.06757)] [[Code](https://github.com/quzefan/LuSh-NeRF)]

## NeRF + Super-resolution

**ASSR-NeRF: Arbitrary-Scale Super-Resolution on Voxel Grid for High-Quality Radiance Fields Reconstruction**<br>
*Ding-Jiun Huang, Zi-Ting Chou, Yu-Chiang Frank Wang, Cheng Sun*<br>
arXiv preprint, 28 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.20066)]

## NeRF + Indoor Scenes

**3D Reconstruction and New View Synthesis of Indoor Environments based on a Dual Neural Radiance Field**<br>
*Zhenyu Bao, Guibiao Liao, Zhongyuan Zhao, Kanglin Liu, Qing Li, Guoping Qiu*<br>
arXiv preprint, 26 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.14726)]

**NeRF-Det++: Incorporating Semantic Cues and Perspective-aware Depth Supervision for Indoor Multi-View 3D Detection**<br>
*Chenxi Huang, Yuenan Hou, Weicai Ye, Di Huang, Xiaoshui Huang, Binbin Lin, Deng Cai, Wanli Ouyang*<br>
arXiv preprint, 22 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.14464)] [[Code](https://github.com/mrsempress/NeRF-Detplusplus)]

**VF-NeRF: Learning Neural Vector Fields for Indoor Scene Reconstruction**<br>
*Albert Gassol Puigjaner, Edoardo Mello Rella, Erik Sandström, Ajad Chhatkuli, Luc Van Gool*<br>
arXiv preprint, 16 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.08766)]

## NeRF + Large Scale Scenes & Urban Scenes

:fire:**Urban Radiance Fields**<br>
*Konstantinos Rematas, Andrew Liu, Pratul P. Srinivasan, Jonathan T. Barron, Andrea Tagliasacchi, Thomas Funkhouser, Vittorio Ferrari*<br>
CVPR 2022, 29 Nov 2021 <br>
<details span>
<summary><b>Abstract</b></summary>
The goal of this work is to perform 3D reconstruction and novel view synthesis from data captured by scanning platforms commonly deployed for world mapping in urban outdoor environments (e.g., Street View). Given a sequence of posed RGB images and lidar sweeps acquired by cameras and scanners moving through an outdoor scene, we produce a model from which 3D surfaces can be extracted and novel RGB images can be synthesized. Our approach extends Neural Radiance Fields, which has been demonstrated to synthesize realistic novel images for small scenes in controlled settings, with new methods for leveraging asynchronously captured lidar data, for addressing exposure variation between captured images, and for leveraging predicted image segmentations to supervise densities on rays pointing at the sky. Each of these three extensions provides significant performance improvements in experiments on Street View data. Our system produces state-of-the-art 3D surface reconstructions and synthesizes higher quality novel views in comparison to both traditional methods (e.g.~COLMAP) and recent neural representations (e.g.~Mip-NeRF).
</details>

[[arXiv](https://arxiv.org/abs/2111.14643)] [[Project](https://urban-radiance-fields.github.io/)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
We use neural radiance fields (NeRFs) to build interactive 3D environments from large-scale visual captures spanning buildings or even multiple city blocks collected primarily from drones. In contrast to single object scenes (on which NeRFs are traditionally evaluated), our scale poses multiple challenges including (1) the need to model thousands of images with varying lighting conditions, each of which capture only a small subset of the scene, (2) prohibitively large model capacities that make it infeasible to train on a single GPU, and (3) significant challenges for fast rendering that would enable interactive fly-throughs.
To address these challenges, we begin by analyzing visibility statistics for large-scale scenes, motivating a sparse network structure where parameters are specialized to different regions of the scene. We introduce a simple geometric clustering algorithm for data parallelism that partitions training images (or rather pixels) into different NeRF submodules that can be trained in parallel.
We evaluate our approach on existing datasets (Quad 6k and UrbanScene3D) as well as against our own drone footage, improving training speed by 3x and PSNR by 12%. We also evaluate recent NeRF fast renderers on top of Mega-NeRF and introduce a novel method that exploits temporal coherence. Our technique achieves a 40x speedup over conventional NeRF rendering while remaining within 0.8 db in PSNR quality, exceeding the fidelity of existing fast renderers.
</details>

[[arXiv](https://arxiv.org/abs/2112.10703)] [[Project](https://meganerf.cmusatyalab.org/)] [[Github](https://github.com/cmusatyalab/mega-nerf)]<br>

:fire:**Block-NeRF: Scalable Large Scene Neural View Synthesis**<br>
*Matthew Tancik, Vincent Casser, Xinchen Yan, Sabeek Pradhan, Ben Mildenhall, Pratul P. Srinivasan, Jonathan T. Barron, Henrik Kretzschmar*<br>
CVPR 2022, 10 Feb 2022 <br>
<details span>
<summary><b>Abstract</b></summary>
We present Block-NeRF, a variant of Neural Radiance Fields that can represent large-scale environments. Specifically, we demonstrate that when scaling NeRF to render city-scale scenes spanning multiple blocks, it is vital to decompose the scene into individually trained NeRFs. This decomposition decouples rendering time from scene size, enables rendering to scale to arbitrarily large environments, and allows per-block updates of the environment. We adopt several architectural changes to make NeRF robust to data captured over months under different environmental conditions. We add appearance embeddings, learned pose refinement, and controllable exposure to each individual NeRF, and introduce a procedure for aligning appearance between adjacent NeRFs so that they can be seamlessly combined. We build a grid of Block-NeRFs from 2.8 million images to create the largest neural scene representation to date, capable of rendering an entire neighborhood of San Francisco.
</details>

[[arXiv](https://arxiv.org/abs/2202.05263)] [[Project](https://waymo.com/intl/zh-cn/research/block-nerf/)]<br>

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

**Global-guided Focal Neural Radiance Field for Large-scale Scene Rendering**<br>
*Mingqi Shao, Feng Xiong, Hang Zhang, Shuang Yang, Mu Xu, Wei Bian, Xueqian Wang*<br>
arXiv preprint, 19 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.12839)] [[Project](https://shaomq2187.github.io/GF-NeRF/)]

**Entity-NeRF: Detecting and Removing Moving Entities in Urban Scenes**<br>
*Takashi Otonari, Satoshi Ikehata, Kiyoharu Aizawa*<br>
CVPR 2024, 24 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.16141)] [[Project](https://otonari726.github.io/entitynerf/)]

**AG-NeRF: Attention-guided Neural Radiance Fields for Multi-height Large-scale Outdoor Scene Rendering**<br>
*Jingfeng Guo, Xiaohan Zhang, Baozhu Zhao, Qi Liu*<br>
arXiv preprint, 18 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.11897)]

**NeRF On-the-go: Exploiting Uncertainty for Distractor-free NeRFs in the Wild**<br>
*Weining Ren, Zihan Zhu, Boyang Sun, Jiaqi Chen, Marc Pollefeys, Songyou Peng*<br>
CVPR 2024, 29 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.18715)] [[Project](https://rwn17.github.io/nerf-on-the-go/)] [[Code](https://github.com/cvg/nerf-on-the-go)]

**Crowd-Sourced NeRF: Collecting Data from Production Vehicles for 3D Street View Reconstruction**<br>
*Tong Qin, Changze Li, Haoyang Ye, Shaowei Wan, Minzhen Li, Hongwei Liu, Ming Yang*<br>
arXiv preprint, 24 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.16289)]

## NeRF + Autonomous Driving

### NeRF Autonomous Driving Survey

**Neural Radiance Field in Autonomous Driving: A Survey**<br>
*Lei He, Leheng Li, Wenchao Sun, Zeyu Han, Yichen Liu, Sifa Zheng, Jianqiang Wang, Keqiang Li*<br>
arXiv preprint, 22 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.13816)]

### NeRF Autonomous Driving Progress

**READ: Large-Scale Neural Scene Rendering for Autonomous Driving**<br>
*Zhuopeng Li, Lu Li, Zeyu Ma, Ping Zhang, Junbo Chen, Jianke Zhu*<br>
AAAI 2023, 11 May 2022 <br>
[[arXiv](https://arxiv.org/abs/2205.05509)] [[Github](https://github.com/JOP-Lee/READ)] [[Video](https://www.bilibili.com/video/BV1124y1Q781/)]

:fire:**MARS: An Instance-aware, Modular and Realistic Simulator for Autonomous Driving**<br>
*Zirui Wu, Tianyu Liu, Liyi Luo, Zhide Zhong, Jianteng Chen, Hongmin Xiao, Chao Hou, Haozhe Lou, Yuantao Chen, Runyi Yang, Yuxin Huang, Xiaoyu Ye, Zike Yan, Yongliang Shi, Yiyi Liao, Hao Zhao*<br>
CICAI 2023, 27 Jul 2023<br>
<details span>
<summary><b>Abstract</b></summary>
Nowadays, autonomous cars can drive smoothly in ordinary cases, and it is widely recognized that realistic sensor simulation will play a critical role in solving remaining corner cases by simulating them. To this end, we propose an autonomous driving simulator based upon neural radiance fields (NeRFs). Compared with existing works, ours has three notable features: (1) Instance-aware. Our simulator models the foreground instances and background environments separately with independent networks so that the static (e.g., size and appearance) and dynamic (e.g., trajectory) properties of instances can be controlled separately. (2) Modular. Our simulator allows flexible switching between different modern NeRF-related backbones, sampling strategies, input modalities, etc. We expect this modular design to boost academic progress and industrial deployment of NeRF-based autonomous driving simulation. (3) Realistic. Our simulator set new state-of-the-art photo-realism results given the best module selection. Our simulator will be open-sourced while most of our counterparts are not. Project page: this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2307.15058)] [[Project](https://open-air-sun.github.io/mars/)] [[Code](https://github.com/OPEN-AIR-SUN/mars)] [[Video](https://www.youtube.com/watch?v=AdC-jglWvfU)]<br>

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

**Forging Vision Foundation Models for Autonomous Driving: Challenges, Methodologies, and Opportunities**<br>
*Xu Yan, Haiming Zhang, Yingjie Cai, Jingming Guo, Weichao Qiu, Bin Gao, Kaiqiang Zhou, Yue Zhao, Huan Jin, Jiantao Gao, Zhen Li, Lihui Jiang, Wei Zhang, Hongbo Zhang, Dengxin Dai, Bingbing Liu*<br>
arXiv preprint, 16 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.08045)] [[Code](https://github.com/zhanghm1995/Forge_VFM4AD)]

**CARFF: Conditional Auto-encoded Radiance Field for 3D Scene Forecasting**<br>
*Jiezhi Yang, Khushi Desai, Charles Packer, Harshil Bhatia, Nicholas Rhinehart, Rowan McAllister, Joseph Gonzalez*<br>
arXiv preprint, 31 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.18075)]

**PC-NeRF: Parent-Child Neural Radiance Fields Using Sparse LiDAR Frames in Autonomous Driving Environments**<br>
*Xiuzhong Hu, Guangming Xiong, Zheng Zang, Peng Jia, Yuxuan Han, Junyi Ma*<br>
arXiv preprint, 14 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.09325)] [[Code](https://github.com/biter0088/pc-nerf)]

**OccFlowNet: Towards Self-supervised Occupancy Estimation via Differentiable Rendering and Occupancy Flow**<br>
*Simon Boeder, Fabian Gigengack, Benjamin Risse*<br>
arXiv preprint, 20 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.12792)]

**Lightning NeRF: Efficient Hybrid Scene Representation for Autonomous Driving**<br>
*Junyi Cao, Zhichao Li, Naiyan Wang, Chao Ma*<br>
ICRA 2024, 9 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.05907)] [[Code](https://github.com/VISION-SJTU/Lightning-NeRF)]

**Are NeRFs ready for autonomous driving? Towards closing the real-to-simulation gap**<br>
*Carl Lindström, Georg Hess, Adam Lilja, Maryam Fatemi, Lars Hammarstrand, Christoffer Petersson, Lennart Svensson*<br>
CVPR 2024, 24 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.16092)] [[Project](https://research.zenseact.com/publications/closing-real2sim-gap/)]

**DriveEnv-NeRF: Exploration of A NeRF-Based Autonomous Driving Environment for Real-World Performance Validation**<br>
*Mu-Yi Shen, Chia-Chi Hsu, Hao-Yu Hou, Yu-Chen Huang, Wei-Fang Sun, Chia-Che Chang, Yu-Lun Liu, Chun-Yi Lee*<br>
arXiv preprint, 23 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.15791)] [[Project](https://muyishen2040.github.io/DriveEnvNeRF/)] [[Code](https://github.com/muyishen2040/DriveEnvNeRF?tab=readme-ov-file)] [[Video](https://www.youtube.com/watch?v=8wNflV_A5FM)]

**NeuroNCAP: Photorealistic Closed-loop Safety Testing for Autonomous Driving**<br>
*William Ljungbergh, Adam Tonderski, Joakim Johnander, Holger Caesar, Kalle Åström, Michael Felsberg, Christoffer Petersson*<br>
arXiv preprint, 11 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.07762)] [[Code](https://github.com/atonderski/neuro-ncap)]

**Searching Realistic-Looking Adversarial Objects For Autonomous Driving Systems**<br>
*Shengxiang Sun, Shenzhe Zhu*<br>
arXiv preprint, 19 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.11629)]


**HybridOcc: NeRF Enhanced Transformer-based Multi-Camera 3D Occupancy Prediction**<br>
*Xiao Zhao, Bo Chen, Mingyang Sun, Dingkang Yang, Youxing Wang, Xukun Zhang, Mingcheng Li, Dongliang Kou, Xiaoyi Wei, Lihua Zhang*<br>
IEEE RAL, 17 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.09104)]

**LeC^2O-NeRF: Learning Continuous and Compact Large-Scale Occupancy for Urban Scenes**<br>
*Zhenxing Mi, Dan Xu*<br>
18 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.11374)]

## NeRF + Editing

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
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Fields (NeRFs) have emerged as a popular approach for novel view synthesis. While NeRFs are quickly being adapted for a wider set of applications, intuitively editing NeRF scenes is still an open challenge. One important editing task is the removal of unwanted objects from a 3D scene, such that the replaced region is visually plausible and consistent with its context. We refer to this task as 3D inpainting. In 3D, solutions must be both consistent across multiple views and geometrically valid. In this paper, we propose a novel 3D inpainting method that addresses these challenges. Given a small set of posed images and sparse annotations in a single input image, our framework first rapidly obtains a 3D segmentation mask for a target object. Using the mask, a perceptual optimizationbased approach is then introduced that leverages learned 2D image inpainters, distilling their information into 3D space, while ensuring view consistency. We also address the lack of a diverse benchmark for evaluating 3D scene inpainting methods by introducing a dataset comprised of challenging real-world scenes. In particular, our dataset contains views of the same scene with and without a target object, enabling more principled benchmarking of the 3D inpainting task. We first demonstrate the superiority of our approach on multiview segmentation, comparing to NeRFbased methods and 2D segmentation approaches. We then evaluate on the task of 3D inpainting, establishing state-ofthe-art performance against other NeRF manipulation algorithms, as well as a strong 2D image inpainter baseline. Project Page: this https URL
</details>

[[arXiv](https://arxiv.org/abs/2211.12254)] [[Project](https://spinnerf3d.github.io/)] [[Github](https://github.com/SamsungLabs/SPIn-NeRF)] [[Video](https://www.bilibili.com/video/BV1Fm4y127TW/)] [[Notes](./paper_discussions/SPIn-NeRF.md)]<br>

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
<details span>
<summary><b>Abstract</b></summary>
In this paper, we propose a method that enables interactive geometry editing for neural radiance fields manipulation. We use two proxy cages(inner cage and outer cage) to edit a scene. The inner cage defines the operation target, and the outer cage defines the adjustment space. Various operations apply to the two cages. After cage selection, operations on the inner cage lead to the desired transformation of the inner cage and adjustment of the outer cage. Users can edit the scene with translation, rotation, scaling, or combinations. The operations on the corners and edges of the cage are also supported. Our method does not need any explicit 3D geometry representations. The interactive geometry editing applies directly to the implicit neural radiance fields. Extensive experimental results demonstrate the effectiveness of our approach.
</details>

[[arXiv](https://arxiv.org/abs/2303.11537)] [[Project](https://repo-sam.inria.fr/fungraph/nerfshop/)] [[Github](https://github.com/graphdeco-inria/nerfshop)] [[Video](https://www.bilibili.com/video/BV1qk4y1b7L4/)] [[Notes](./paper_discussions/NeRFShop.md)]<br>

:fire:**Instruct-NeRF2NeRF: Editing 3D Scenes with Instructions**<br>
*Ayaan Haque, Matthew Tancik, Alexei A. Efros, Aleksander Holynski, Angjoo Kanazawa*<br>
arXiv preprint, 22 Mar 2023 <br>
<details span>
<summary><b>Abstract</b></summary>
We propose a method for editing NeRF scenes with text-instructions. Given a NeRF of a scene and the collection of images used to reconstruct it, our method uses an image-conditioned diffusion model (InstructPix2Pix) to iteratively edit the input images while optimizing the underlying scene, resulting in an optimized 3D scene that respects the edit instruction. We demonstrate that our proposed method is able to edit large-scale, real-world scenes, and is able to accomplish more realistic, targeted edits than prior work.
</details>

[[arXiv](https://arxiv.org/abs/2303.12789)] [[Project](https://instruct-nerf2nerf.github.io/)] [[Github](https://github.com/ayaanzhaque/instruct-nerf2nerf)] [[Video](https://www.bilibili.com/video/BV1rb411o7gR/)]<br>

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

**InseRF: Text-Driven Generative Object Insertion in Neural 3D Scenes**<b
*Mohamad Shahbazi, Liesbeth Claessens, Michael Niemeyer, Edo Collins, Alessio Tonioni, Luc Van Gool, Federico Tombari*<br>
arXiv preprint, 10 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.05335)]

**Scaling Face Interaction Graph Networks to Real World Scenes**<br>
*Tatiana Lopez-Guevara, Yulia Rubanova, William F. Whitney, Tobias Pfaff, Kimberly Stachenfeld, Kelsey R. Allen*<br>
arXiv preprint, 22 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.11985)]

**Exploration and Improvement of Nerf-based 3D Scene Editing Techniques**<br>
*Shun Fang, Ming Cui, Xing Feng, Yanan Zhang*<br>
arXiv preprint, 23 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.12456)]

**ViCA-NeRF: View-Consistency-Aware 3D Editing of Neural Radiance Fields**<br>
*Jiahua Dong, Yu-Xiong Wang*<br>
NeurIPS 2023, 1 Feb 2024<br>
[[arXiv](https://browse.arxiv.org/abs/2402.00864)] [[Code(https://github.com/Dongjiahua/VICA-NeRF)]]

**Geometry Transfer for Stylizing Radiance Fields**<br>
*Hyunyoung Jung, Seonghyeon Nam, Nikolaos Sarafianos, Sungjoo Yoo, Alexander Sorkine-Hornung, Rakesh Ranjan*<br>
CVPR 2024, 1 Feb 2024<br>
[[arXiv](https://browse.arxiv.org/abs/2402.00863)] [[Project](https://hyblue.github.io/geo-srf/)] [[Code](https://github.com/hyBlue/Geo-SRF)]

**Consolidating Attention Features for Multi-view Image Editing**<br>
*Or Patashnik, Rinon Gal, Daniel Cohen-Or, Jun-Yan Zhu, Fernando De la Torre*<br>
arXiv preprint, 22 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.14792)] [[Project](https://qnerf-consolidation.github.io/qnerf-consolidation/)]

**SealD-NeRF: Interactive Pixel-Level Editing for Dynamic Scenes by Neural Radiance Fields**<br>
*Zhentao Huang, Yukun Shi, Neil Bruce, Minglun Gong*<br>
arXiv preprint, 21 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.13510)]

**StyleDyRF: Zero-shot 4D Style Transfer for Dynamic Neural Radiance Fields**<br>
*Hongbin Xu, Weitao Chen, Feng Xiao, Baigui Sun, Wenxiong Kang*<br>
arXiv preprint, 13 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.08310)] [[Code](https://github.com/ToughStoneX/StyleDyRF)]

**GenN2N: Generative NeRF2NeRF Translation**<br>
*Xiangyue Liu, Han Xue, Kunming Luo, Ping Tan, Li Yi*<br>
CVPR 2024, 3 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.02788)] [[Project](https://xiangyueliu.github.io/GenN2N/)] [[Code](https://xiangyueliu.github.io/GenN2N/)]

**Freditor: High-Fidelity and Transferable NeRF Editing by Frequency Decomposition**<br>
*Yisheng He, Weihao Yuan, Siyu Zhu, Zilong Dong, Liefeng Bo, Qixing Huang*<br>
arXiv preprint, 3 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.02514)]

**Taming Latent Diffusion Model for Neural Radiance Field Inpainting**<br>
*Chieh Hubert Lin, Changil Kim, Jia-Bin Huang, Qinbo Li, Chih-Yao Ma, Johannes Kopf, Ming-Hsuan Yang, Hung-Yu Tseng*<br>
arXiv preprint, 15 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.09995)] [[Project](https://hubert0527.github.io/MALD-NeRF/)]

**Depth Priors in Removal Neural Radiance Fields**<br>
*Zhihao Guo, Peng Wang*<br>
arXiv preprint, 1 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.00630)]

**NeRF-Insert: 3D Local Editing with Multimodal Control Signals**<br>
*Benet Oriol Sabat, Alessandro Achille, Matthew Trager, Stefano Soatto*<br>
arXiv preprint, 30 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.19204)]

**MVIP-NeRF: Multi-view 3D Inpainting on NeRF Scenes via Diffusion Prior**<br>
*Honghua Chen, Chen Change Loy, Xingang Pan*<br>
arXiv preprint, 5 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.02859)]

**Point Resampling and Ray Transformation Aid to Editable NeRF Models**<br>
*Zhenyang Li, Zilong Chen, Feifan Qu, Mingqing Wang, Yizhou Zhao, Kai Zhang, Yifan Peng*<br>
arXiv preprint, 12 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.07306)]

**ExtraNeRF: Visibility-Aware View Extrapolation of Neural Radiance Fields with Diffusion Models**<br>
*Meng-Li Shih, Wei-Chiu Ma, Lorenzo Boyice, Aleksander Holynski, Forrester Cole, Brian L. Curless, Janne Kontkanen*<br>
CVPR 2024, 10 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.06133)]

**NeRFDeformer: NeRF Transformation from a Single View via 3D Scene Flows**<br>
*Zhenggang Tang, Zhongzheng Ren, Xiaoming Zhao, Bowen Wen, Jonathan Tremblay, Stan Birchfield, Alexander Schwing*<br>
CVPR 2024, 15 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.10543)] [[Code](https://github.com/nerfdeformer/nerfdeformer)]

**IE-NeRF: Inpainting Enhanced Neural Radiance Fields in the Wild**<br>
*Shuaixian Wang, Haoran Xu, Yaokun Li, Jiwei Chen, Guang Tan*<br>
arXiv preprint, 15 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.10695)]

## NeRF + Relighting


**Relighting Neural Radiance Fields With Shadow and Highlight Hints**<br>
*Chong Zeng, Guojun Chen, Yue Dong, Pieter Peers, Hongzhi Wu, Xin Tong*<br>
SIGGRAPH 2023
[[Paper](https://nrhints.github.io/pdfs/nrhints-sig23.pdf)] [[Project](https://nrhints.github.io/)] [[Github](https://github.com/iamNCJ/NRHints)]

**Relighting Scenes with Object Insertions in Neural Radiance Fields**<br>
*Xuening Zhu, Renjiao Yi, Xin Wen, Chenyang Zhu, Kai Xu*<br>
arXiv preprint, 21 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.14806)]


**Baking Relightable NeRF for Real-time Direct/Indirect Illumination Rendering**<br>
*Euntae Choi, Vincent Carpentier, Seunghun Shin, Sungjoo Yoo*<br>
arXiv preprint, 16 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.10327)]

## NeRF + Open Surface Reconstruction and Cloth Simulation

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


## NeRF + Segmentation

**SSDNeRF: Semantic Soft Decomposition of Neural Radiance Fields**<br>
*Siddhant Ranade, Christoph Lassner, Kai Li, Christian Haene, Shen-Chi Chen, Jean-Charles Bazin, Sofien Bouaziz*<br>
arXiv preprint, 7 Dec 2022 <br>
[[arXiv](https://arxiv.org/abs/2212.03406)] [[Project](https://www.siddhantranade.com/research/2022/12/06/SSDNeRF-Semantic-Soft-Decomposition-of-Neural-Radiance-Fields.html)] [[Video](https://www.bilibili.com/video/BV1XR4y1C7Yf/)]

:fire:**Panoptic Lifting for 3D Scene Understanding with Neural Fields**<br>
*Yawar Siddiqui, Lorenzo Porzi, Samuel Rota Buló, Norman Müller, Matthias Nießner, Angela Dai, Peter Kontschieder*<br>
CVPR 2023, 19 Dec 2022 <br>
<details span>
<summary><b>Abstract</b></summary>
We propose Panoptic Lifting, a novel approach for learning panoptic 3D volumetric representations from images of in-the-wild scenes. Once trained, our model can render color images together with 3D-consistent panoptic segmentation from novel viewpoints.
Unlike existing approaches which use 3D input directly or indirectly, our method requires only machine-generated 2D panoptic segmentation masks inferred from a pre-trained network. Our core contribution is a panoptic lifting scheme based on a neural field representation that generates a unified and multi-view consistent, 3D panoptic representation of the scene. To account for inconsistencies of 2D instance identifiers across views, we solve a linear assignment with a cost based on the model's current predictions and the machine-generated segmentation masks, thus enabling us to lift 2D instances to 3D in a consistent way. We further propose and ablate contributions that make our method more robust to noisy, machine-generated labels, including test-time augmentations for confidence estimates, segment consistency loss, bounded segmentation fields, and gradient stopping.
Experimental results validate our approach on the challenging Hypersim, Replica, and ScanNet datasets, improving by 8.4, 13.8, and 10.6% in scene-level PQ over state of the art.
</details>

[[arXiv](https://arxiv.org/abs/2212.09802)] [[Project](https://nihalsid.github.io/panoptic-lifting/)] [[Github](https://github.com/nihalsid/panoptic-lifting)] [[Video](https://www.youtube.com/watch?v=QtsiL-6rSuM)]<br>

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

**Slot-guided Volumetric Object Radiance Fields**<br>
*Di Qi, Tong Yang, Xiangyu Zhang*<br>
NeurIPS 2023, 4 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.02241)]

**OpenNeRF: Open Set 3D Neural Scene Segmentation with Pixel-Wise Features and Rendered Novel Views**<br>
*Francis Engelmann, Fabian Manhardt, Michael Niemeyer, Keisuke Tateno, Marc Pollefeys, Federico Tombari*<br>
ICLR 2024, 4 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.03650)] [[Project](https://opennerf.github.io/)] [[Code](https://github.com/opennerf/opennerf)]

**Rethinking Open-Vocabulary Segmentation of Radiance Fields in 3D Space**<br>
*Hyunjee Lee, Youngsik Yun, Jeongmin Bae, Seoha Kim, Youngjung Uh*<br>
arXiv preprint, 14 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.07416)] [[Project](https://hyunji12.github.io/Open3DRF/)]

**DiscoNeRF: Class-Agnostic Object Field for 3D Object Discovery**<br>
*Corentin Dumery, Aoxiang Fan, Ren Li, Nicolas Talabot, Pascal Fua*<br>
arXiv preprint, 19 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.09928)]

**Multi-modal NeRF Self-Supervision for LiDAR Semantic Segmentation**<br>
*Xavier Timoneda, Markus Herb, Fabian Duerr, Daniel Goehring, Fisher Yu*<br>
IROS 2024, 5 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.02969)]

## NeRF + Multi-Modal

### NeRF Multi-Modal Survey

**When LLMs step into the 3D World: A Survey and Meta-Analysis of 3D Tasks via Multi-modal Large Language Models**<br>
*Xianzheng Ma, Yash Bhalgat, Brandon Smart, Shuai Chen, Xinghui Li, Jian Ding, Jindong Gu, Dave Zhenyu Chen, Songyou Peng, Jia-Wang Bian, Philip H Torr, Marc Pollefeys, Matthias Nießner, Ian D Reid, Angel X. Chang, Iro Laina, Victor Adrian Prisacariu*<br>
arXiv preprint, 16 Mar 2022<br>
[[arXiv](https://arxiv.org/abs/2405.10255)] [[Code](https://github.com/ActiveVisionLab/Awesome-LLM-3D)]

### NeRF Multi-Modal Progresses

**Exploring Multi-modal Neural Scene Representations With Applications on Thermal Imaging**<br>
*Mert Özer, Maximilian Weiherer, Martin Hundhausen, Bernhard Egger*<br>
arXiv preprint, 18 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.11865)] [[Project](https://mert-o.github.io/ThermalNeRF/)]

**Connecting NeRFs, Images, and Text**<br>
*Francesco Ballerini, Pierluigi Zama Ramirez, Roberto Mirabella, Samuele Salti, Luigi Di Stefano*<br>
CVPRW-INRV 2024, 11 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.07993)]

**NeRF: Multi-Modal Decomposition NeRF with 3D Feature Fields**<br>
*Ning Wang, Lefei Zhang, Angel X Chang*<br>
arXiv preprint, 8 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.05010)]

**Self-supervised Pre-training for Transferable Multi-modal Perception**<br>
*Xiaohao Xu, Tianyi Zhang, Jinrong Yang, Matthew Johnson-Roberson, Xiaonan Huang*<br>
arXiv preprint, 28 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.17942)]

## NeRF + Semantic/Understanding

**uSF: Learning Neural Semantic Field with Uncertainty**<br>
*Vsevolod Skorokhodov, Darya Drozdova, Dmitry Yudin*<br>
arXiv preprint, 13 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.08012)] [[Code](https://github.com/sevashasla/usf/)]

**GARField: Group Anything with Radiance Fields**<br>
*Chung Min Kim, Mingxuan Wu, Justin Kerr, Ken Goldberg, Matthew Tancik, Angjoo Kanazawa*<br>
CVPR 2024, 17 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.09419)] [[Project](https://www.garfield.studio/)] [[Code](https://github.com/chungmin99/garfield)]

**OV-NeRF: Open-vocabulary Neural Radiance Fields with Vision and Language Foundation Models for 3D Semantic Understanding**<br>
*Guibiao Liao, Kaichen Zhou, Zhenyu Bao, Kanglin Liu, Qing Li*<br>
avXiv preprint, 7 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.04648)]

**NeRF Analogies: Example-Based Visual Attribute Transfer for NeRFs**<br>
*Michael Fischer, Zhengqin Li, Thu Nguyen-Phuoc, Aljaz Bozic, Zhao Dong, Carl Marshall, Tobias Ritschel*<br>
arXiv preprint, 13 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.08784)]

**GSNeRF: Generalizable Semantic Neural Radiance Fields with Enhanced 3D Scene Understanding**<br>
*Zi-Ting Chou, Sheng-Yu Huang, I-Jieh Liu, Yu-Chiang Frank Wang*<br>
CVPR 2024, 6 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.03608)]

**Finding Waldo: Towards Efficient Exploration of NeRF Scene Space**<br>
*Evangelos Skartados, Mehmet Kerim Yucel, Bruno Manganelli, Anastasios Drosou, Albert Saà-Garriga*<br>
ACM MMSys 24, 7 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.04508)]

**NeRF-Supervised Feature Point Detection and Description**<br>
*Ali Youssef, Francisco Vasconcelos<br>
arXiv preprint, 13 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.08156)]

**Exploring 3D-aware Latent Spaces for Efficiently Learning Numerous Scenes**<br>
*Antoine Schnepf, Karim Kassab, Jean-Yves Franceschi, Laurent Caraffa, Flavian Vasile, Jeremie Mary, Andrew Comport, Valérie Gouet-Brunet**<br>
3DMV-CVPR 2024,  18 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.11678)] [[Project](https://3da-ae.github.io/)]

**Semantic Is Enough: Only Semantic Information For NeRF Reconstruction**<br>
*Ruibo Wang, Song Zhang, Ping Huang, Donghai Zhang, Wei Yan*<br>
arXiv preprint, 24 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.16043)]

**NeRF-MAE : Masked AutoEncoders for Self Supervised 3D representation Learning for Neural Radiance Fields**<br>
*Muhammad Zubair Irshad, Sergey Zakahrov, Vitor Guizilini, Adrien Gaidon, Zsolt Kira, Rares Ambrus*<br>
CVPR Neural Rendering Intelligence Workshop, 2024, 1 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.01300)] [[Project](https://nerf-mae.github.io/)]

**NeRF-MAE: Masked AutoEncoders for Self-Supervised 3D Representation Learning for Neural Radiance Fields**<br>
*Muhammad Zubair Irshad, Sergey Zakahrov, Vitor Guizilini, Adrien Gaidon, Zsolt Kira, Rares Ambrus*<br>
arXiv preprint, 1 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.01300)] [[Project](https://nerf-mae.github.io/)]

**NeRF-DetS: Enhancing Multi-View 3D Object Detection with Sampling-adaptive Network of Continuous NeRF-based Representation**<br>
*Chi Huang, Xinyang Li, Shengchuan Zhang, Liujuan Cao, Rongrong Ji*<br>
arXiv preprint, 22 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.13921)]

**Gear-NeRF: Free-Viewpoint Rendering and Tracking with Motion-aware Spatio-Temporal Sampling**<br>
*Xinhang Liu, Yu-Wing Tai, Chi-Keung Tang, Pedro Miraldo, Suhas Lohit, Moitreya Chatterjee*<br>
CVPR 2024, 6 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.03723)] [[Project](https://merl.com/research/highlights/gear-nerf)]

**OpenObj: Open-Vocabulary Object-Level Neural Radiance Fields with Fine-Grained Understanding**<br>
*Yinan Deng, Jiahui Wang, Jingyu Zhao, Jianyu Dou, Yi Yang, Yufeng Yue*<br>
arXiv preprint, 12 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.08009)] [[Project](https://openobj.github.io/)] [[Video](https://www.youtube.com/watch?v=BeUdxrjItDE)]

**Active Scout: Multi-Target Tracking Using Neural Radiance Fields in Dense Urban Environments**<br>
*Christopher D. Hsu, Pratik Chaudhari*<br>
arXiv preprint, 11 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.07431)]

**DistillNeRF: Perceiving 3D Scenes from Single-Glance Images by Distilling Neural Fields and Foundation Model Features**<br>
*Letian Wang, Seung Wook Kim, Jiawei Yang, Cunjun Yu, Boris Ivanovic, Steven L. Waslander, Yue Wang, Sanja Fidler, Marco Pavone, Peter Karkus*<br>
arXiv preprint, 17 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.12095)]

**LLaNA: Large Language and NeRF Assistant**<br>
*Andrea Amaduzzi, Pierluigi Zama Ramirez, Giuseppe Lisanti, Samuele Salti, Luigi Di Stefano*<br>
arXiv preprint, 17 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.11840)]

**Learning with Noisy Ground Truth: From 2D Classification to 3D Reconstruction**<br>
*Yangdi Lu, Wenbo He*<br>
arXiv preprint, 23 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.15982)]

**Fast and Efficient: Mask Neural Fields for 3D Scene Segmentation**<br>
*Zihan Gao, Lingling Li, Licheng Jiao, Fang Liu, Xu Liu, Wenping Ma, Yuwei Guo, Shuyuan Yang*<br>
arXiv preprintm, 1 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.01220)]

**Improving 3D Finger Traits Recognition via Generalizable Neural Rendering**
*Hongbin Xu, Junduan Huang, Yuer Ma, Zifeng Li, Wenxiong Kang*<br>
IJCV 2024, 12 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.09582)] [[Project](https://scut-bip-lab.github.io/fingernerf/)]



## NeRF + Mesh Extraction

:fire:**Delicate Textured Mesh Recovery from NeRF via Adaptive Surface Refinement**<br>
*Jiaxiang Tang, Hang Zhou, Xiaokang Chen, Tianshu Hu, Errui Ding, Jingdong Wang, Gang Zeng*<br>
arXiv preprint, 3 Mar 2023 <br>
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Fields (NeRF) have constituted a remarkable breakthrough in image-based 3D reconstruction. However, their implicit volumetric representations differ significantly from the widely-adopted polygonal meshes and lack support from common 3D software and hardware, making their rendering and manipulation inefficient. To overcome this limitation, we present a novel framework that generates textured surface meshes from images. Our approach begins by efficiently initializing the geometry and view-dependency decomposed appearance with a NeRF. Subsequently, a coarse mesh is extracted, and an iterative surface refining algorithm is developed to adaptively adjust both vertex positions and face density based on re-projected rendering errors. We jointly refine the appearance with geometry and bake it into texture images for real-time rendering. Extensive experiments demonstrate that our method achieves superior mesh quality and competitive rendering quality.
</details>

[[arXiv/](https://arxiv.org/abs/2303.02091)] [[Project](https://me.kiui.moe/nerf2mesh/)] [[Github](https://github.com/ashawkey/nerf2mesh)] [[Video](https://www.bilibili.com/video/BV18M41147JN/)]<br>

**TeTriRF: Temporal Tri-Plane Radiance Fields for Efficient Free-Viewpoint Video**<br>
*Minye Wu, Zehao Wang, Georgios Kouros, Tinne Tuytelaars*<br>
arXiv preprint, 10 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.06713)]

**R^2-Mesh: Reinforcement Learning Powered Mesh Reconstruction via Geometry and Appearance Refinement**<br>
*Haoyang Wang, Liming Liu, Quanlu Jia, Jiangkai Wu, Haodan Zhang, Peiheng Wang, Xinggong Zhang*<br>
arXiv preprint, 19 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.10135)]

## NeRF + Codec/Streaming

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
<details span>
<summary><b>Abstract</b></summary>
The success of the Neural Radiance Fields (NeRFs) for modeling and free-view rendering static objects has inspired numerous attempts on dynamic scenes. Current techniques that utilize neural rendering for facilitating free-view videos (FVVs) are restricted to either offline rendering or are capable of processing only brief sequences with minimal motion. In this paper, we present a novel technique, Residual Radiance Field or ReRF, as a highly compact neural representation to achieve real-time FVV rendering on long-duration dynamic scenes. ReRF explicitly models the residual information between adjacent timestamps in the spatial-temporal feature space, with a global coordinate-based tiny MLP as the feature decoder. Specifically, ReRF employs a compact motion grid along with a residual feature grid to exploit inter-frame feature similarities. We show such a strategy can handle large motions without sacrificing quality. We further present a sequential training scheme to maintain the smoothness and the sparsity of the motion/residual grids. Based on ReRF, we design a special FVV codec that achieves three orders of magnitudes compression rate and provides a companion ReRF player to support online streaming of long-duration FVVs of dynamic scenes. Extensive experiments demonstrate the effectiveness of ReRF for compactly representing dynamic radiance fields, enabling an unprecedented free-viewpoint viewing experience in speed and quality.
</details>

[[arXiv](https://arxiv.org/abs/2304.04452)] [[Project](https://aoliao12138.github.io/ReRF/)]<br>

**VideoRF: Rendering Dynamic Radiance Fields as 2D Feature Video Streams**<br>
*Liao Wang, Kaixin Yao, Chengcheng Guo, Zhirui Zhang, Qiang Hu, Jingyi Yu, Lan Xu, Minye Wu*<br>
arxiv preprint, 3 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.01407)] [[Project](https://aoliao12138.github.io/VideoRF)]

:fire:**SlimmeRF: Slimmable Radiance Fields**<br>
*Shiran Yuan, Hao Zhao*<br>
3DV 2024, 15 Dec 2023<br>
<details span>
<summary><b>Abstract</b></summary>
Neural Radiance Field (NeRF) and its variants have recently emerged as successful methods for novel view synthesis and 3D scene reconstruction. However, most current NeRF models either achieve high accuracy using large model sizes, or achieve high memory-efficiency by trading off accuracy. This limits the applicable scope of any single model, since high-accuracy models might not fit in low-memory devices, and memory-efficient models might not satisfy high-quality requirements. To this end, we present SlimmeRF, a model that allows for instant test-time trade-offs between model size and accuracy through slimming, thus making the model simultaneously suitable for scenarios with different computing budgets. We achieve this through a newly proposed algorithm named Tensorial Rank Incrementation (TRaIn) which increases the rank of the model's tensorial representation gradually during training. We also observe that our model allows for more effective trade-offs in sparse-view scenarios, at times even achieving higher accuracy after being slimmed. We credit this to the fact that erroneous information such as floaters tend to be stored in components corresponding to higher ranks. Our implementation is available at this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2312.10034)] [[Project](https://shiran-yuan.github.io/SlimmeRF/)] [[Code](https://github.com/Shiran-Yuan/SlimmeRF)]<br>

**Efficient Dynamic-NeRF Based Volumetric Video Coding with Rate Distortion Optimization**<br>
*Zhiyu Zhang, Guo Lu, Huanxiong Liang, Anni Tang, Qiang Hu, Li Song*<br>
arXiv preprint, 2 Feb 2024<br>
[[arXiv](https://browse.arxiv.org/abs/2402.01380)]

## NeRF + Model Conversion

**One is All: Bridging the Gap Between Neural Radiance Fields Architectures with Progressive Volume Distillation**<br>
*Shuangkang Fang, Weixin Xu, Heng Wang, Yi Yang, Yufeng Wang, Shuchang Zhou*<br>
AAAI 2023, 29 Nov 2022 <br>
[[arXiv](https://arxiv.org/abs/2211.15977)] [[Project](https://sk-fun.fun/PVD)] [[Github](https://github.com/megvii-research/AAAI2023-PVD)] [[PVD-AL Github](https://github.com/megvii-research/AAAI2023-PVD/tree/PVD-AL)]

**NeRFs to Gaussian Splats, and Back**<br>
*Siming He, Zach Osman, Pratik Chaudhari*<br>
arXiv preprint, 15 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.09717)] [[Code](https://github.com/grasp-lyrl/NeRFtoGSandBack)]

## NeRF + Medical/Biology

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

**BioNeRF: Biologically Plausible Neural Radiance Fields for View Synthesis**<br>
*Leandro A. Passos, Douglas Rodrigues, Danilo Jodas, Kelton A. P. Costa, João Paulo Papa*<br>
arXiv preprint, 11 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.07310)]

**NeRF Solves Undersampled MRI Reconstruction**<br>
*Tae Jun Jang, Chang Min Hyun*<br>
arXiv preprint, 20 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.13226)]

**FLex: Joint Pose and Dynamic Radiance Fields Optimization for Stereo Endoscopic Videos**<br>
*Florian Philipp Stilz, Mert Asim Karaoglu, Felix Tristram, Nassir Navab, Benjamin Busam, Alexander Ladikos*<br>
arXiv preprint, 18 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.12198)]

**High-fidelity Endoscopic Image Synthesis by Utilizing Depth-guided Neural Surfaces**<br>
*Baoru Huang, Yida Wang, Anh Nguyen, Daniel Elson, Francisco Vasconcelos, Danail Stoyanov*<br>
arXiv preprint, 20 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.13437)]

**DPER: Diffusion Prior Driven Neural Representation for Limited Angle and Sparse View CT Reconstruction**<br>
*Chenhe Du, Xiyue Lin, Qing Wu, Xuanyu Tian, Ying Su, Zhe Luo, Hongjiang Wei, S. Kevin Zhou, Jingyi Yu, Yuyao Zhang*<br>
arXiv preprint, 27 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.17890)]

**3D Vessel Reconstruction from Sparse-View Dynamic DSA Images via Vessel Probability Guided Attenuation Learning**<br>
*Zhentao Liu, Huangxuan Zhao, Wenhui Qin, Zhenghong Zhou, Xinggang Wang, Wenping Wang, Xiaochun Lai, Chuansheng Zheng, Dinggang Shen, Zhiming Cui*<br>
arXiv preprint, 17 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.10705)]

**Neural Radiance Fields for Novel View Synthesis in Monocular Gastroscopy**<br>
*Zijie Jiang, Yusuke Monno, Masatoshi Okutomi, Sho Suzuki, Kenji Miki*<br>
EMBC 2024, 29 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.18863)]

**Shorter SPECT Scans Using Self-supervised Coordinate Learning to Synthesize Skipped Projection Views**<br>
*Zongyu Li, Yixuan Jia, Xiaojian Xu, Jason Hu, Jeffrey A. Fessler, Yuni K. Dewaraja*<br>
arXiv preprint, 27 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.18840)]

**3D Reconstruction of Protein Structures from Multi-view AFM Images using Neural Radiance Fields (NeRFs)**<br>
*Jaydeep Rade, Ethan Herron, Soumik Sarkar, Anwesha Sarkar, Adarsh Krishnamurthy*<br>
arXiv preprint, 12 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.06244)]

**NeRF-US: Removing Ultrasound Imaging Artifacts from Neural Radiance Fields in the Wild**<br>
*Rishit Dagli, Atsuhiro Hibi, Rahul G. Krishnan, Pascal N. Tyrrell*<br>
arXiv preprint, 13 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.10258)]

**NeRF-CA: Dynamic Reconstruction of X-ray Coronary Angiography with Extremely Sparse-views**<br>
*Kirsten W.H. Maas, Danny Ruijters, Anna Vilanova, Nicola Pezzotti*<br>
arXiv preprint, 29 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.16355)]

**UC-NeRF: Uncertainty-aware Conditional Neural Radiance Fields from Endoscopic Sparse Views**<br>
*Jiaxin Guo, Jiangliu Wang, Ruofeng Wei, Di Kang, Qi Dou, Yun-hui Liu*<br>
arXiv preprint, 4 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.02917)]

**Intraoperative Registration by Cross-Modal Inverse Neural Rendering**<br>
*Maximilian Fehrentz, Mohammad Farid Azampour, Reuben Dorent, Hassan Rasheed, Colin Galvin, Alexandra Golby, William M. Wells, Sarah Frisken, Nassir Navab, Nazim Haouchine*<br>
arXiv preprint, 18 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.11983)] [[Project](https://maxfehrentz.github.io/style-ngp/)]

**HybridNeRF-Stereo Vision: Pioneering Depth Estimation and 3D Reconstruction in Endoscopy**<br>
*Pengcheng Chen, Wenhao Li, Nicole Gunderson, Jeremy Ruthberg, Randall Bly, Waleed M. Abuzeid, Zhenglong Sun, Eric J. Seibel*<br>
arXiv preprint, 10 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.04041)]

**Neural rendering enables dynamic tomography**<br>
*Ivan Grega, William F. Whitney, Vikram S. Deshpande*<br>
NeurIPS 2024, 27 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.20558)] [[Project](https://neural-xray.github.io/nerfxray/)]

## NeRF + Inverse Rendering

:fire:**Multi-view Inverse Rendering for Large-scale Real-world Indoor Scenes**<br>
*Zhen Li, Lingli Wang, Mofang Cheng, Cihui Pan, Jiaqi Yang*<br>
CVPR 2023, 18 Nov 2022 <br>
<details span>
<summary><b>Abstract</b></summary>
We present a efficient multi-view inverse rendering method for large-scale real-world indoor scenes that reconstructs global illumination and physically-reasonable SVBRDFs. Unlike previous representations, where the global illumination of large scenes is simplified as multiple environment maps, we propose a compact representation called Texture-based Lighting (TBL). It consists of 3D mesh and HDR textures, and efficiently models direct and infinite-bounce indirect lighting of the entire large scene. Based on TBL, we further propose a hybrid lighting representation with precomputed irradiance, which significantly improves the efficiency and alleviates the rendering noise in the material optimization. To physically disentangle the ambiguity between materials, we propose a three-stage material optimization strategy based on the priors of semantic segmentation and room segmentation. Extensive experiments show that the proposed method outperforms the state-of-the-art quantitatively and qualitatively, and enables physically-reasonable mixed-reality applications such as material editing, editable novel view synthesis and relighting. The project page is at this https URL.
</details>

[[arXiv](https://arxiv.org/abs/2211.10206)] [[Project](http://yodlee.top/TexIR/)] [[Github](http://github.com/LZleejean/TexIR_code)] [[Video](https://www.bilibili.com/video/BV1gM411K7ik/)]<br>

:fire:**TensoIR: Tensorial Inverse Rendering**<br>
*Haian Jin, Isabella Liu, Peijia Xu, Xiaoshuai Zhang, Songfang Han, Sai Bi, Xiaowei Zhou, Zexiang Xu, Hao Su*<br>
CVPR 2023, 24 Apr 2023 <br>
<details span>
<summary><b>Abstract</b></summary>
We propose TensoIR, a novel inverse rendering approach based on tensor factorization and neural fields. Unlike previous works that use purely MLP-based neural fields, thus suffering from low capacity and high computation costs, we extend TensoRF, a state-of-the-art approach for radiance field modeling, to estimate scene geometry, surface reflectance, and environment illumination from multi-view images captured under unknown lighting conditions. Our approach jointly achieves radiance field reconstruction and physically-based model estimation, leading to photo-realistic novel view synthesis and relighting results. Benefiting from the efficiency and extensibility of the TensoRF-based representation, our method can accurately model secondary shading effects (like shadows and indirect lighting) and generally support input images captured under single or multiple unknown lighting conditions. The low-rank tensor representation allows us to not only achieve fast and compact reconstruction but also better exploit shared information under an arbitrary number of capturing lighting conditions. We demonstrate the superiority of our method to baseline methods qualitatively and quantitatively on various challenging synthetic and real-world scenes.
</details>

[[arXiv](https://arxiv.org/abs/2304.12461)] [[Project](https://haian-jin.github.io/TensoIR/)] [[Github](https://github.com/Haian-Jin/TensoIR)] [[Video](https://www.bilibili.com/video/BV1Fc411n7Gb/)]<br>

:fire:**Inverse Global Illumination using a Neural Radiometric Prior**<br>
*Saeed Hadadan, Geng Lin, Jan Novák, Fabrice Rousselle, Matthias Zwicker*<br>
SIGGRAPH 2023, 3 May 2023 <br>
<details span>
<summary><b>Abstract</b></summary>
Inverse rendering methods that account for global illumination are becoming more popular, but current methods require evaluating and automatically differentiating millions of path integrals by tracing multiple light bounces, which remains expensive and prone to noise. Instead, this paper proposes a radiometric prior as a simple alternative to building complete path integrals in a traditional differentiable path tracer, while still correctly accounting for global illumination. Inspired by the Neural Radiosity technique, we use a neural network as a radiance function, and we introduce a prior consisting of the norm of the residual of the rendering equation in the inverse rendering loss. We train our radiance network and optimize scene parameters simultaneously using a loss consisting of both a photometric term between renderings and the multi-view input images, and our radiometric prior (the residual term). This residual term enforces a physical constraint on the optimization that ensures that the radiance field accounts for global illumination. We compare our method to a vanilla differentiable path tracer, and more advanced techniques such as Path Replay Backpropagation. Despite the simplicity of our approach, we can recover scene parameters with comparable and in some cases better quality, at considerably lower computation times.
</details>

[[arXiv](https://arxiv.org/abs/2305.02192)] [[Notes](./paper_discussions/InverseGlobalIllumination.md)]<br>

**SplitNeRF: Split Sum Approximation Neural Field for Joint Geometry, Illumination, and Material Estimation**<br>
*Jesus Zarzar, Bernard Ghanem*<br>
arXiv preprint, 28 Nov 2023<br>
[[arXiv](https://arxiv.org/abs/2311.16671)] 

**NeRF as Non-Distant Environment Emitter in Physics-based Inverse Rendering**<br>
*Jingwang Ling, Ruihan Yu, Feng Xu, Chun Du, Shuang Zhao*<br>
SIGGRAPH 2024, 7 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.04829)] [[Project](https://nerfemitterpbir.github.io/)]

**Inverse Rendering of Glossy Objects via the Neural Plenoptic Function and Radiance Fields**<br>
*Haoyuan Wang, Wenbo Hu, Lei Zhu, Rynson W. H. Lau*<br>
CVPR 2024, 24 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.16224)] [[Project](https://whyy.site/paper/nep)]

**IntrinsicAnything: Learning Diffusion Priors for Inverse Rendering Under Unknown Illumination**<br>
*Xi Chen, Sida Peng, Dongchen Yang, Yuan Liu, Bowen Pan, Chengfei Lv, Xiaowei Zhou*<br>
arXiv preprint, 17 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.11593)] [[Project](https://zju3dv.github.io/IntrinsicAnything/)]

**MIRReS: Multi-bounce Inverse Rendering using Reservoir Sampling**<br>
*Yuxin Dai, Qi Wang, Jingsen Zhu, Dianbing Xi, Yuchi Huo, Chen Qian, Ying He*<br>
arXiv preprint, 24 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.16360)] [[Project](https://brabbitdousha.github.io/MIRReS/)] [[Video](https://www.bilibili.com/video/BV18E421N7fU/)]

**RRM: Relightable assets using Radiance guided Material extraction**<br>
*Diego Gomez, Julien Philip, Adrien Kaiser, Élie Michel*<br>
CGI 2024, 8 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.06397)]

**Material Transforms from Disentangled NeRF Representations**<br>
*Ivan Lopes, Jean-François Lalonde, Raoul de Charette*<br>
arXiv preprint, 12 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.08037)] [[Code](https://github.com/astra-vision/BRDFTransform)]

## NeRF + Texture Synthesis

**NeRF-Tex: Neural Reflectance Field Textures**<br>
*Hendrik Baatz, Jonathan Granskog, Marios Papas, Fabrice Rousselle, Jan Novák*<br>
EGSR 2021, 22 Jun, 2021<br>
[[Paper](https://d1qx31qr3h6wln.cloudfront.net/publications/NeRFTex.pdf)] [[Project](https://research.nvidia.com/publication/2021-06_nerf-tex-neural-reflectance-field-textures)]

**NeRF-Texture: Texture Synthesis With Neural Radiance Fields**<br>
*Yihua Huang, Yan-Pei Cao, Yu-Kun Lai, Ying Shan, Lin Gao*<br>
SIGGRAPH 2023<br>
[[Video](https://www.bilibili.com/video/BV1UW4y1f7oK/)]

## NeRF + Robotics

### NeRF Robotics Survey

**NeRF in Robotics: A Survey**<br>
*Guangming Wang, Lei Pan, Songyou Peng, Shaohui Liu, Chenfeng Xu, Yanzi Miao, Wei Zhan, Masayoshi Tomizuka, Marc Pollefeys, Hesheng Wang*<br>
arXiv preprint,  2 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.01333)]

**Benchmarking Neural Radiance Fields for Autonomous Robots: An Overview**<br>
*Yuhang Ming, Xingrui Yang, Weihan Wang, Zheng Chen, Jinglun Feng, Yifan Xing, Guofeng Zhang*<br>
arXiv preprint, 9 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.05526)]

**A Survey on Occupancy Perception for Autonomous Driving: The Information Fusion Perspective**<br>
*Huaiyuan Xu, Junliang Chen, Shiyu Meng, Yi Wang, Lap-Pui Chau*<br>
arXiv preprint, 8 May 2024<br>
[[arXiv](https://github.com/HuaiyuanXu/3D-Occupancy-Perception)]

### NeRF Robotics Progresses

**MACS: Mass Conditioned 3D Hand and Object Motion Synthesis**<br>
*Soshi Shimada, Franziska Mueller, Jan Bednarik, Bardia Doosti, Bernd Bickel, Danhang Tang, Vladislav Golyanik, Jonathan Taylor, Christian Theobalt, Thabo Beeler*<br>
arXiv preprint, 22 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.14929)]

**Fit-NGP: Fitting Object Models to Neural Graphics Primitives**<br>
*Marwan Taher, Ignacio Alzugaray, Andrew J. Davison*<br>
arXiv preprint, 4 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.02357)]

**6-DoF Grasp Pose Evaluation and Optimization via Transfer Learning from NeRFs**<br>
*Gergely Sóti, Xi Huang, Christian Wurll, Björn Hein*<br>
arXiv preprint, 15 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.07935)] [[Project](https://gergely-soti.github.io/grasp/)]

**Physical Priors Augmented Event-Based 3D Reconstruction**<br>
*Jiaxu Wang, Junhao He, Ziyi Zhang, Renjing Xu*<br>
ICRA 2024, 30 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.17121)] [[Code](https://github.com/Mercerai/PAEv3d)]

**Di-NeRF: Distributed NeRF for Collaborative Learning with Unknown Relative Poses**<br>
*Mahboubeh Asadi, Kourosh Zareinia, Sajad Saeedi*<br>
arXiv preprint, 2 Feb 2024<br>
[[arXiv](https://browse.arxiv.org/abs/2402.01485)] [[Project](https://sites.google.com/view/di-nerf/home)]

**Reg-NF: Efficient Registration of Implicit Surfaces within Neural Fields**<br>
*Stephen Hausler, David Hall, Sutharsan Mahendren, Peyman Moghadam*<br>
ICRA 2024, 15 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.09722)]

**DeformNet: Latent Space Modeling and Dynamics Prediction for Deformable Object Manipulation**<br>
*Chenchang Li, Zihao Ai, Tong Wu, Xiaosa Li, Wenbo Ding, Huazhe Xu*<br>
ICRA 2024, 12 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.07648)]

**Closing the Visual Sim-to-Real Gap with Object-Composable NeRFs**<br>
*Nikhil Mishra, Maximilian Sieb, Pieter Abbeel, Xi Chen*<br>
ICRA 2024, 7 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.04114)]

**SiLVR: Scalable Lidar-Visual Reconstruction with Neural Radiance Fields for Robotic Inspection**<br>
*Yifu Tao, Yash Bhalgat, Lanke Frank Tarimo Fu, Matias Mattamala, Nived Chebrolu, Maurice Fallon*<br>
ICRA 2024, 11 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.06877)] [[Project](https://ori-drs.github.io/projects/silvr/)] [[Video](https://www.youtube.com/watch?si=IchOIkatoFJl0B9Z&v=kA11bdMbhMo&feature=youtu.be)]

**MULAN-WC: Multi-Robot Localization Uncertainty-aware Active NeRF with Wireless Coordination**><br>
*Weiying Wang, Victor Cai, Stephanie Gil*<br>
arXiv preprint, 20 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.13348)]

**NVINS: Robust Visual Inertial Navigation Fused with NeRF-augmented Camera Pose Regressor and Uncertainty Quantification**<br>
*Juyeop Han, Lukas Lao Beyer, Guilherme V. Cavalheiro, Sertac Karaman*<br>
arXiv preprint, 1 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.01400)]

**Uncertainty-aware Active Learning of NeRF-based Object Models for Robot Manipulators using Visual and Re-orientation Actions**<br>
*Saptarshi Dasgupta, Akshat Gupta, Shreshth Tuli, Rohan Paul*<br>
arXiv preprint, 2 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.01812)]

**NeRF-Guided Unsupervised Learning of RGB-D Registration**<br>
*Zhinan Yu, Zheng Qin, Yijie Tang, Yongjun Wang, Renjiao Yi, Chenyang Zhu, Kai Xu*<br>
arXiv preprint, 1 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.00507)]

**Novel View Synthesis with Neural Radiance Fields for Industrial Robot Applications**<br>
*Markus Hillemann, Robert Langendörfer, Max Heiken, Max Mehltretter, Andreas Schenk, Martin Weinmann, Stefan Hinz, Christian Heipke, Markus Ulrich*<br>
arXiv preprint, 7 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.04345)]

**Neural Visibility Field for Uncertainty-Driven Active Mapping**<br>
*Shangjie Xue, Jesse Dill, Pranay Mathur, Frank Dellaert, Panagiotis Tsiotra, Danfei Xu*<br>
CVPR 2024, 11 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.06948)] [[Project](https://sites.google.com/view/nvf-cvpr24/)]

**dGrasp:NeRF-Informed Implicit Grasp Policies with Supervised Optimization Slopes**<br>
*Gergely Sóti, Xi Huang, Christian Wurll, Gergely Sóti<br>
arXiv preprint,  14 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.09939)]

**Articulate your NeRF: Unsupervised articulated object modeling via conditional view synthesis**<br>
*Jianning Deng, Kartic Subr, Hakan Bilen*<br>
arXiv preprint, 24 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.16623)]

**GeoNLF: Geometry guided Pose-Free Neural LiDAR Fields**<br>
*Weiyi Xue, Zehan Zheng, Fan Lu, Haiyun Wei, Guang Chen, Changjun Jiang*<br>
arXiv preprint, 8 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.05597)]

**AirNeRF: 3D Reconstruction of Human with Drone and NeRF for Future Communication Systems**<br>
*Alexey Kotcov, Maria Dronova, Vladislav Cheremnykh, Sausar Karaf, Dzmitry Tsetserukou*<br>
arXiv preprint, 15 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.10865)]

**LEIA: Latent View-invariant Embeddings for Implicit 3D Articulation**<br>
*Archana Swaminathan, Anubhav Gupta, Kamal Gupta, Shishira R. Maiya, Vatsal Agarwal, Abhinav Shrivastava*<br>
ECCV 2024, 10 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.06703)] [[Project](https://archana1998.github.io/leia/)] [[Code](https://github.com/archana1998/LEIA/)]

**From Words to Poses: Enhancing Novel Object Pose Estimation with Vision Language Models**<br>
*Tessa Pulli, Stefan Thalhammer, Simon Schwaiger, Markus Vincze*<br>
arXiv preprint, 9 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.05413)]

**NARF24: Estimating Articulated Object Structure for Implicit Rendering**<br>
*Stanley Lewis, Tom Gao, Odest Chadwicke Jenkins*<br>
ICRA 2024, 15 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.09829)]

**Active Neural Mapping at Scale**<br>
*Zijia Kuang, Zike Yan, Hao Zhao, Guyue Zhou, Hongbin Zha*<br>
arXiv preprint, 30 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.20276)]

**Distributed NeRF Learning for Collaborative Multi-Robot Perception**<br>
*Hongrui Zhao, Boris Ivanovic, Negar Mehr*<br>
arXiv preprint, 30 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.20289)]

**Enhancing Exploratory Capability of Visual Navigation Using Uncertainty of Implicit Scene Representation**<br>
*Yichen Wang, Qiming Liu, Zhe Liu, Hesheng Wang*<br>
arXiv preprint, 5 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.03487)]

**NeRF-Aug: Data Augmentation for Robotics with Neural Radiance Fields**<br<
*Eric Zhu, Mara Levy, Matthew Gwilliam, Abhinav Shrivastava*<br>
arXiv preprint, 4 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.02482)] [[Project](https://nerf-aug.github.io/)]

## NeRF + Transparent and Specular

**NeRRF: 3D Reconstruction and View Synthesis for Transparent and Specular Objects with Neural Refractive-Reflective Fields**<br>
*Xiaoxue Chen, Junchen Liu, Hao Zhao, Guyue Zhou, Ya-Qin Zhang*<br>
arXiv preprint, 22 Sep 2023<br>
[[arXiv](https://arxiv.org/abs/2309.13039)]

**Neural Radiance Fields for Transparent Object Using Visual Hull**<br>
*Heechan Yoon, Seungkyu Lee*<br>
arXiv preprint, 13 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.08118)]
 
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

**GNeRP: Gaussian-guided Neural Reconstruction of Reflective Objects with Noisy Polarization Priors**<br>
*LI Yang, WU Ruizheng, LI Jiyong, CHEN Ying-cong*<br>
ICLR 2024, 18 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.11899)] [[Project](https://yukiumi13.github.io/gnerp_page/)] [[Code](https://github.com/yukiumi13/GNeRP)]

:fire:**REFRAME: Reflective Surface Real-Time Rendering for Mobile Devices**<br>
*Chaojie Ji, Yufeng Li, Yiyi Liao*<br>
arXiv preprint, 25 Mar 2024<br>
<details span>
<summary><b>Abstract</b></summary>
This work tackles the challenging task of achieving real-time novel view synthesis for reflective surfaces across various scenes. Existing real-time rendering methods, especially those based on meshes, often have subpar performance in modeling surfaces with rich view-dependent appearances. Our key idea lies in leveraging meshes for rendering acceleration while incorporating a novel approach to parameterize view-dependent information. We decompose the color into diffuse and specular, and model the specular color in the reflected direction based on a neural environment map. Our experiments demonstrate that our method achieves comparable reconstruction quality for highly reflective surfaces compared to state-of-the-art offline methods, while also efficiently enabling real-time rendering on edge devices such as smartphones.
</details>

[[arXiv](https://arxiv.org/abs/2403.16481)] [[Project](https://xdimlab.github.io/REFRAME/)]<br>

**SAID-NeRF: Segmentation-AIDed NeRF for Depth Completion of Transparent Objects**<br>
*Avinash Ummadisingu, Jongkeum Choi, Koki Yamane, Shimpei Masuda, Naoki Fukaya, Kuniyuki Takahashi*<br>
arXiv preprint, 28 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.19607)] [[Video](https://www.youtube.com/watch?v=S4NCoUq4bmE)]

**Residual-NeRF: Learning Residual NeRFs for Transparent Object Manipulation**<br>
*Bardienus P. Duisterhof, Yuemin Mao, Si Heng Teng, Jeffrey Ichnowski*<br>
arXiv preprint, 10 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.06181)]

**NeRF-Casting: Improved View-Dependent Appearance with Consistent Reflections**<br>
*Dor Verbin, Pratul P. Srinivasan, Peter Hedman, Ben Mildenhall, Benjamin Attal, Richard Szeliski, Jonathan T. Barron*<br>
arXiv preprint, 23 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.14871)] [[Project](https://nerf-casting.github.io/)]

**Neural Directional Encoding for Efficient and Accurate View-Dependent Appearance Modeling**<br>
*Liwen Wu, Sai Bi, Zexiang Xu, Fujun Luan, Kai Zhang, Iliyan Georgiev, Kalyan Sunkavalli, Ravi Ramamoorthi*<br>
CVPR 2024 , 23 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.14847)] [[Project](https://lwwu2.github.io/nde/)] [[Code](https://github.com/lwwu2/nde)]

**Planar Reflection-Aware Neural Radiance Fields**<br>
*Chen Gao, Yipeng Wang, Changil Kim, Jia-Bin Huang, Johannes Kopf*<br>
arXiv preprint, 7 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.04984)]

## Other 3D Generative Work

:fire:**Patch-based 3D Natural Scene Generation from a Single Example**<br>
*Weiyu Li, Xuelin Chen, Jue Wang, Baoquan Chen*<br>
CVPR 2023, 25 Apr 2023 <br>
<details span>
<summary><b>Abstract</b></summary>
We target a 3D generative model for general natural scenes that are typically unique and intricate. Lacking the necessary volumes of training data, along with the difficulties of having ad hoc designs in presence of varying scene characteristics, renders existing setups intractable. Inspired by classical patch-based image models, we advocate for synthesizing 3D scenes at the patch level, given a single example. At the core of this work lies important algorithmic designs w.r.t the scene representation and generative patch nearest-neighbor module, that address unique challenges arising from lifting classical 2D patch-based framework to 3D generation. These design choices, on a collective level, contribute to a robust, effective, and efficient model that can generate high-quality general natural scenes with both realistic geometric structure and visual appearance, in large quantities and varieties, as demonstrated upon a variety of exemplar scenes.
</details>

[[arXiv](https://arxiv.org/abs/2304.12670)] [[Project](http://weiyuli.xyz/Sin3DGen/)] [[Github](https://github.com/wyysf-98/Sin3DGen)] [[Notes](./paper_discussions/Sin3DGen.md)]<br>

## NeRF + Other applications

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

**A Deep Learning Framework for Wireless Radiation Field Reconstruction and Channel Prediction**<br>
*Haofan Lu, Christopher Vattheuer, Baharan Mirzasoleiman, Omid Abari*<br>
arXiv preprint, 5 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2403.03241)]

**Neural radiance fields-based holography**<br>
*Minsung Kang, Fan Wang, Kai Kumano, Tomoyoshi Ito, Tomoyoshi Shimobaba*<br>
arXiv preprint, 2 Mar 2023<br>
[[arXiv](https://arxiv.org/abs/2403.01137)]

**Leveraging Neural Radiance Field in Descriptor Synthesis for Keypoints Scene Coordinate Regression**<br>
*Huy-Hoang Bui, Bach-Thuan Bui, Dinh-Tuan Tran, Joo-Ho Lee*<br>
arXiv preprint, 15 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.10297)]

**ThermoNeRF: Multimodal Neural Radiance Fields for Thermal Novel View Synthesis**<br>
*Mariam Hassan, Florent Forest, Olga Fink, Malcolm Mielle*<br>
arXiv preprint, 18 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.12154)]

**Exploring Accurate 3D Phenotyping in Greenhouse through Neural Radiance Fields**<br>
*Junhong Zhao, Wei Ying, Yaoqiang Pan, Zhenfeng Yi, Chao Chen, Kewei Hu, Hanwen Kang*<br>
arXiv preprint, 24 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.15981)]

**Blending Distributed NeRFs with Tri-stage Robust Pose Optimization**<br>
*Baijun Ye, Caiyun Liu, Xiaoyu Ye, Yuantao Chen, Yuhai Wang, Zike Yan, Yongliang Shi, Hao Zhao, Guyue Zhou*<br>
arXiv preprint, 5 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.02880)]

**R-NeRF: Neural Radiance Fields for Modeling RIS-enabled Wireless Environments**<br>
*Huiying Yang, Zihan Jin, Chenhao Wu, Rujing Xiong, Robert Caiming Qiu, Zenan Ling*<br>
arXiv preprint, 19 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.11541)]

**Bayesian uncertainty analysis for underwater 3D reconstruction with neural radiance fields**<br>
*Haojie Lian, Xinhao Li, Yilin Qu, Jing Du, Zhuxuan Meng, Jie Liu, Leilei Chen*<br>
arXiv preprint, 11 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.08154)]

**Physics-Informed Learning of Characteristic Trajectories for Smoke Reconstruction**<br>
*Yiming Wang, Siyu Tang, Mengyu Chu*<br>
SIGGRAPH 2024, 12 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.09679)] [[Project](https://19reborn.github.io/PICT_Smoke.github.io/)] [[Video](https://youtu.be/DXQO4E-ShbI)] [[Code](https://github.com/19reborn/PICT_smoke)]

**Feasibility of Neural Radiance Fields for Crime Scene Video Reconstruction**<br>
*Shariq Nadeem Malik, Min Hao Chee, Dayan Mario Anthony Perera, Chern Hong Lim*<br>
arXiv preprint, 11 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.08795)]

**PanicleNeRF: low-cost, high-precision in-field phenotyping of rice panicles with smartphone**<br>
*Xin Yang, Xuqi Lu, Pengyao Xie, Ziyue Guo, Hui Fang, Haowei Fu, Xiaochun Hu, Zhenbiao Sun, Haiyan Cen*<br>
arXiv preprint, 4 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.02053)]

**AgriNeRF: Neural Radiance Fields for Agriculture in Challenging Lighting Conditions**<br>
*Samarth Chopra, Fernando Cladera, Varun Murali, Vijay Kumar*<br>
arXiv preprint, 23 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.15487)]

**NeRF-Accelerated Ecological Monitoring in Mixed-Evergreen Redwood Forest**<br>
*Adam Korycki, Cory Yeaton, Gregory S. Gilbert, Colleen Josephson, Steve McGuire*<br>
arXiv preprint, 9 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.07418)] [[Code](https://github.com/harelab-ucsc/RedwoodNeRF)]


## NeRF + Gaming

**Video2Game: Real-time, Interactive, Realistic and Browser-Compatible Environment from a Single Video**<br>
*Hongchi Xia, Zhi-Hao Lin, Wei-Chiu Ma, Shenlong Wang*<br>
CVPR 2024, 15 Apr 2024<br>
[[arXiv](https://arxiv.org/abs/2404.09833)] [[Project](https://video2game.github.io/)] [[Code](https://github.com/video2game/video2game)]

## NeRF + Quality Metric

**Towards a Robust Framework for NeRF Evaluation**<br>
*Adrian Azzarelli, Nantheera Anantrasirichai, David R Bull*<br>
arXiv preprint, 29 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.18079)]

**NeRF View Synthesis: Subjective Quality Assessment and Objective Metrics Evaluation**<br>
*Pedro Martin, Antonio Rodrigues, Joao Ascenso, Maria Paula Queluz*<br>
arXiv preprint, 30 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.20078)]

## NeRF + CAD

**Magic NeRF Lens: Interactive Fusion of Neural Radiance Fields for Virtual Facility Inspection**<br>
*Ke Li, Susanne Schmidt, Tim Rolff, Reinhard Bacher, Wim Leemans, Frank Steinicke*<br>
TCVG, 19 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.09860)]

**CAD-NeRF: Learning NeRFs from Uncalibrated Few-view Images by CAD Model Retrieval**<br>
*Xin Wen, Xuening Zhu, Renjiao Yi, Zhifeng Wang, Chenyang Zhu, Kai Xu*<br>
Frontiers of Computer Science, 5 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.02979)]

## NeRF + GIS

**Improving NeRF with Height Data for Utilization of GIS Data**<br>
*Hinata Aoki, Takao Yamanaka*<br>
ICIP 2023, 15 Jul 2023<br>
[[arXiv](https://arxiv.org/abs/2307.07729)]

## NeRF + Terrain

**Neural Elevation Models for Terrain Mapping and Path Planning**<br>
*Adam Dai, Shubh Gupta, Grace Gao*<br>
arXiv preprint, 24 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.15227)]

## NeRF + Satellite Images / Radar

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

**Dynamic Occupancy Grids for Object Detection: A Radar-Centric Approach**<br>
*Max Peter Ronecker, Markus Schratter, Lukas Kuschnig, Daniel Watzenig*<br>
ICRA 2024, 2 Feb 2024<br>
[[arXiv](https://browse.arxiv.org/abs/2402.01488)]

**BirdNeRF: Fast Neural Reconstruction of Large-Scale Scenes From Aerial Imagery**<br>
*Huiqing Zhang, Yifei Xue, Ming Liao, Yizhen Lao*<br>
arXiv preprint, 7 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.04554)]

**Aerial Lifting: Neural Urban Semantic and Building Instance Lifting from Aerial Imagery**<br>
*Yuqi Zhang, Guanying Chen, Jiaxing Chen, Shuguang Cui*<br>
CVPR 2024, 18 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.11812)] [[Project](https://zyqz97.github.io/Aerial_Lifting/)] [[Code](https://github.com/zyqz97/Aerial_lifting)] [[Video](https://www.youtube.com/watch?v=w_0FZJVOmfQ&feature=youtu.be)]

**SAT-NGP : Unleashing Neural Graphics Primitives for Fast Relightable Transient-Free 3D reconstruction from Satellite Imagery**<br>
*Camille Billouard, Dawa Derksen, Emmanuelle Sarrazin, Bruno Vallet*<br>
IGARSS 2024, 27 Mar 2024<br>
[[arXiv](https://arxiv.org/abs/2403.18711)] [[Code](https://github.com/Ellimac0/SAT-NGP)]

**Aerial-NeRF: Adaptive Spatial Partitioning and Sampling for Large-Scale Aerial Rendering**<br>
*Xiaohan Zhang, Yukui Qiu, Zhenyu Sun, Qi Liu*<br>
arXiv preprint, 10 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.06214)]

**Multiplane Prior Guided Few-Shot Aerial Scene Rendering&**<br>
*Zihan Gao, Licheng Jiao, Lingling Li, Xu Liu, Fang Liu, Puhua Chen, Yuwei Guo*<br>
CVPR 2024, 7 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.04961)]

**psPRF:Pansharpening Planar Neural Radiance Field for Generalized 3D Reconstruction Satellite Imagery**<br>
*Tongtong Zhang, Yuanxiang Li*<br>
arXiv preprint, 22 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.15707)]

**Domain Generalization for 6D Pose Estimation Through NeRF-based Image Synthesis**<br>
*Antoine Legrand, Renaud Detry, Christophe De Vleeschouwer*<br>
arXiv preprint, 15 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.10762)]

**BRDF-NeRF: Neural Radiance Fields with Optical Satellite Images and BRDF Modelling**<br>
*Lulin Zhang, Ewelina Rupnik, Tri Dung Nguyen, Stéphane Jacquemoud, Yann Klinger*<br>
arXiv preprint, 18 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.12014)]

**Exploring Seasonal Variability in the Context of Neural Radiance Fields for 3D Reconstruction on Satellite Imagery**<br>
*Liv Kåreborn, Erica Ingerstad, Amanda Berg, Justus Karlsson, Leif Haglund*<br>
arXiv preprint, 5 Nov 2024<br>
[[arXiv](https://arxiv.org/abs/2411.02972)]

## NeRF + UAV/Drone

**Active Human Pose Estimation via an Autonomous UAV Agent**<br>
*Jingxi Chen, Botao He, Chahat Deep Singh, Cornelia Fermuller, Yiannis Aloimonos*<br>
arXiv preprint, 1 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.01811)]

**Radiance Field Learners As UAV First-Person Viewers**<br>
*Liqi Yan, Qifan Wang, Junhan Zhao, Qiang Guan, Zheng Tang, Jianhui Zhang, Dongfang Li*<br>
ECCV 2024, 10 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.05533)] [[Project](https://fpv-nerf.github.io/)]

## NeRF + Copyright protection and Security

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

**Noise-NeRF: Hide Information in Neural Radiance Fields using Trainable Noise**<br>
*Qinglong Huang, Yong Liao, Yanbin Hao, Pengyuan Zhou*<br>
arXiv preprint, 2 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.01216)]

**WateRF: Robust Watermarks in Radiance Fields for Protection of Copyrights**<br>
*Youngdong Jang, Dong In Lee, MinHyuk Jang, Jong Wook Kim, Feng Yang, Sangpil Kim*<br>
arXiv preprint, 3 May 2024<br>
[[arXiv](https://arxiv.org/abs/2405.02066)]

**Protecting NeRFs' Copyright via Plug-And-Play Watermarking Base Model**<br>
*Qi Song, Ziyuan Luo, Ka Chun Cheung, Simon See, Renjie Wan*<br>
ECCV 2024, 10 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.07735)] [[Project](https://qsong2001.github.io/NeRFProtector/)]

**GeometrySticker: Enabling Ownership Claim of Recolorized**<br>
*Xiufeng Huang, Ka Chun Cheung, Simon See, Renjie Wan*<br>
arXiv preprint, 18 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.13390)] [[Project](https://kevinhuangxf.github.io/GeometrySticker/)]

**IPA-NeRF: Illusory Poisoning Attack Against Neural Radiance Fields**<br>
*Wenxiang Jiang, Hanwei Zhang, Shuo Zhao, Zhongwen Guo, Hao Wang*<br>
arXiv preprint, 16 Jul 2024<br>
[[arXiv](https://arxiv.org/abs/2407.11921)] [[Code](https://github.com/jiang-wenxiang/IPA-NeRF)]

**NeRF: Privacy-preserving Training Framework for NeRF**<br>
*Bokang Zhang, Yanglin Zhang, Zhikun Zhang, Jinglan Yang, Lingying Huang, Junfeng Wu*<br>
arXiv preprint, 3 Sep 2024<br>
[[arXiv](https://arxiv.org/abs/2409.01661)]

## NeRF + Motion Detection

**3D Motion Magnification: Visualizing Subtle Motions with Time Varying Radiance Fields**<br>
*Brandon Y. Feng, Hadi Alzayer, Michael Rubinstein, William T. Freeman, Jia-Bin Huang*<br>
ICCV 2023, 7 Aug 2023<br>
[[arXiv](https://arxiv.org/abs/2308.03757)] [[Project](https://3d-motion-magnification.github.io/)]

**C-NERF: Representing Scene Changes as Directional Consistency Difference-based NeRF**<br>
*Rui Huang, Binbin Jiang, Qingyi Zhao, William Wang, Yuxiang Zhang, Qing Guo*<br>
arXiv 2023, 5 Dec 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02751)]

## NeRF Defect Detection

**Irregularity Inspection using Neural Radiance Field**<br>
*Tianqi Ding, Dawei Xiang*<br>
arXiv preprint, 21 Aug 2024<br>
[[arXiv](https://arxiv.org/abs/2408.11251)]

## Datasets

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

**Implicit-Zoo: A Large-Scale Dataset of Neural Implicit Functions for 2D Images and 3D Scenes**<br>
*Qi Ma, Danda Pani Paudel, Ender Konukoglu, Luc Van Gool*<br>
arXiv preprint, 25 Jun 2024<br>
[[arXiv](https://arxiv.org/abs/2406.17438)]

## Neural Surface Reconstruction

**Neural Kernel Surface Reconstruction**<br>
*Jiahui Huang, Zan Gojcic, Matan Atzmon, Or Litany, Sanja Fidler, Francis Williams*<br>
CVPR 2023, 31 May 2023<br>
[[arXiv](https://arxiv.org/abs/2305.19590)]

**Neuralangelo: High-Fidelity Neural Surface Reconstruction**<br>
*Zhaoshuo Li, Thomas Müller, Alex Evans, Russell H. Taylor, Mathias Unberath, Ming-Yu Liu, Chen-Hsuan Lin*<br>
CVPR 2023, 5 Jun 2023<br>
[[arXiv](https://arxiv.org/abs/2306.03092)] [[Project](https://research.nvidia.com/labs/dir/neuralangelo)] [[Video](https://www.bilibili.com/video/BV1mh4y1d7rX/)]

**GridFormer: Point-Grid Transformer for Surface Reconstruction**<br>
*Shengtao Li, Ge Gao, Yudong Liu, Yu-Shen Liu, Ming Gu*<br>
arXiv preprint, 4 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.02292)] [[Code](https://github.com/list17/GridFormer)]

**PSDF: Prior-Driven Neural Implicit Surface Learning for Multi-view Reconstruction**<br>
*Wanjuan Su, Chen Zhang, Qingshan Xu, Wenbing Tao*<br>
arXiv preprint, 23 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.12751)]

**Binary Opacity Grids: Capturing Fine Geometric Detail for Mesh-Based View Synthesis**<br>
*Christian Reiser, Stephan Garbin, Pratul P. Srinivasan, Dor Verbin, Richard Szeliski, Ben Mildenhall, Jonathan T. Barron, Peter Hedman, Andreas Geiger*<br>
SIGGRAPH 2024, 19 Feb 2024<br>
[[arXiv](https://arxiv.org/abs/2402.12377)] [[Project](https://creiser.github.io/binary_opacity_grid/)] [[Video](https://www.youtube.com/v/2TPUmGRg8bM)]

## Other Important Related Work

### Depth Estimation

**Repurposing Diffusion-Based Image Generators for Monocular Depth Estimation**<br>
*Bingxin Ke, Anton Obukhov, Shengyu Huang, Nando Metzger, Rodrigo Caye Daudt, Konrad Schindler*<br>
CVPR 2024, 4 Dec, 2023<br>
[[arXiv](https://arxiv.org/abs/2312.02145)] [[Project](https://marigoldmonodepth.github.io/)] [[Code](https://github.com/prs-eth/marigold)]

**NeRFmentation: NeRF-based Augmentation for Monocular Depth Estimation**<br>
*Casimir Feldmann, Niall Siegenheim, Nikolas Hars, Lovro Rabuzin, Mert Ertugrul, Luca Wolfart, Marc Pollefeys, Zuria Bauer, Martin R. Oswald*<br>
arXiv preprint, 8 Jan 2024<br>
[[arXiv](https://arxiv.org/abs/2401.03771)]

:fire:**DepthCrafter: Generating Consistent Long Depth Sequences for Open-world Videos**<br>
*Wenbo Hu, Xiangjun Gao, Xiaoyu Li, Sijie Zhao, Xiaodong Cun, Yong Zhang, Long Quan, Ying Shan*<br>
arXiv preprint, 3 Sep 2024<br>
<details span>
<summary><b>Abstract</b></summary>
Despite significant advancements in monocular depth estimation for static images, estimating video depth in the open world remains challenging, since open-world videos are extremely diverse in content, motion, camera movement, and length. We present DepthCrafter, an innovative method for generating temporally consistent long depth sequences with intricate details for open-world videos, without requiring any supplementary information such as camera poses or optical flow. DepthCrafter achieves generalization ability to open-world videos by training a video-to-depth model from a pre-trained image-to-video diffusion model, through our meticulously designed three-stage training strategy with the compiled paired video-depth datasets. Our training approach enables the model to generate depth sequences with variable lengths at one time, up to 110 frames, and harvest both precise depth details and rich content diversity from realistic and synthetic datasets. We also propose an inference strategy that processes extremely long videos through segment-wise estimation and seamless stitching. Comprehensive evaluations on multiple datasets reveal that DepthCrafter achieves state-of-the-art performance in open-world video depth estimation under zero-shot settings. Furthermore, DepthCrafter facilitates various downstream applications, including depth-based visual effects and conditional video generation.
</details>

[[arXiv](https://arxiv.org/abs/2409.02095)] [[Project](https://depthcrafter.github.io/)] [[Code](https://github.com/Tencent/DepthCrafter)]<br>

### Diffusion Surveys

**Diffusion Models in Low-Level Vision: A Survey**<Br>
*Chunming He, Yuqi Shen, Chengyu Fang, Fengyang Xiao, Longxiang Tang, Yulun Zhang, Wangmeng Zuo, Zhenhua Guo, Xiu Li*<br>
arXiv preprint, 17 Jun 2024<br>
[[arXiv0](https://arxiv.org/abs/2406.11138)] [[Code](https://github.com/ChunmingHe/awesome-diffusion-models-in-low-level-vision)]

## New Ideas

**EEG-Driven 3D Object Reconstruction with Color Consistency and Diffusion Prior**<br>
*Xin Xiang, Wenhui Zhou, Guojun Dai*<br>
arXiv preprint, 28 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.20981)]

**GUMBEL-NERF: Representing Unseen Objects as Part-Compositional Neural Radiance Fields**<br>
*Yusuke Sekikawa, Chingwei Hsu, Satoshi Ikehata, Rei Kawakami, Ikuro Sato*<br>
ICIP 2024, 27 Oct 2024<br>
[[arXiv](https://arxiv.org/abs/2410.20306)]

## Contributors

Thanks to the community and hoping more and more people are joining us and submit commits and PRs!<br>

<a href = "https://github.com/yangjiheng/nerf_and_beyond_docs/graphs/contributors">
  <img src = "https://contrib.rocks/image?repo=yangjiheng/nerf_and_beyond_docs"/>
</a>

Made with [contributors-img](https://contrib.rocks).

## License

CC-0
