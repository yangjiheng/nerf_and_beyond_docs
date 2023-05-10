# Discussion on "MVImgNet: A Large-scale Dataset of Multi-view Images"

## Summary

Highlight:
1.  MVImgNet，大规模多视角真实世界图片数据集，从22万视频中提取238个分类的650万帧数据，包含标记以及object mask，相机参数、点云数据
2. 使用MVImgNet，验证了在NeRF重建、multi-view stereo和view-consistent image understanding的效果，达到了满意的效果
3. MVPNet，3D点云数据集，包含标注了的150个分类的87200个样本
4. 数据集已开放下载

Limitations:
1. 数据集更聚焦在与人日常生活相关的分类中，其他自然界分类数据相对少一些
2. 数据集不考虑特别复杂背景，但应该可以使用domain adaptation or knowledge distillation类的方法解决

## Questions
