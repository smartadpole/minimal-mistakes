---
title:  "「CV」 深度估计资源汇总"
mathjax: true
key: depth-prediction-foundation-20190403
toc: true
toc_sticky: true
category: [AI, CV, 2.5D, depth_prediction]
tags: 资源
---
<span id='head'></span>  
>**深度估计**：根据单张图像得到深度图；        
[深度估计概述](/ai/cv/2.5d/depth_prediction/survey)    


`Monocular Depth` · `Stereo Consistency` · `Depth Estimation` · `Depth Completion` · `Depth Fusion`   

<!--more-->  

# 1 综述
## 1.1 单目

1. [Monocular Depth Estimation: A Survey](https://arxiv.org/abs/1901.09402)   
*2019-01-27* [paper](https://arxiv.org/abs/1901.09402)   

1. [How do neural networks see depth in single images?](https://arxiv.org/abs/1905.07005)   
*2019-05-16* [paper](https://arxiv.org/abs/1905.07005)   

1. [Monocular Depth Estimation Based On Deep Learning: An Overview](https://arxiv.org/abs/2003.06620)   
*2020-07-03* [paper](https://arxiv.org/abs/2003.06620) | [blog](https://cloud.tencent.com/developer/article/1759027)       

1. [Deep Learning based Monocular Depth Prediction: Datasets, Methods and Applications](https://arxiv.org/abs/2011.04123)    
*2022-02-18* [paper](https://arxiv.org/abs/2011.04123)   

# 2 理论

# 3 单目

## 3.1 回归任务

###  3.1.1 监督

1. [Depth Map Prediction from a Single Image using a Multi-Scale Deep Network](https://arxiv.org/abs/1406.2283)     
nips 2014 *2014-06-09* [paper](https://arxiv.org/abs/1406.2283) | [home](https://cs.nyu.edu/~deigen/depth/)   

1. [Predicting Depth, Surface Normals and Semantic Labels with a Common Multi-Scale Convolutional Architecture](https://arxiv.org/abs/1411.4734)   
iccv 2015 *2014-11-18* [paper](https://arxiv.org/abs/1411.4734) | [home](https://cs.nyu.edu/~deigen/dnl/)    


1. [Single-Image Depth Perception in the Wild](https://arxiv.org/abs/1604.03901)    
nips 2016 *2016-04-13* [paper](https://arxiv.org/abs/1604.03901) | [home](http://www-personal.umich.edu/~wfchen/depth-in-the-wild/)      


1. [A Two-Streamed Network for Estimating Fine-Scaled Depth Maps from Single RGB Images](https://arxiv.org/abs/1607.00730)    
iccv 2017 *2016-07-04* [paper](https://arxiv.org/abs/1607.00730)    


1. [Structured Attention Guided Convolutional Neural Fields for Monocular Depth Estimation](https://arxiv.org/abs/1803.11029)    
cvpr 2018 *2018-03-29* [paper](https://arxiv.org/abs/1803.11029) | [caffe](https://github.com/danxuhk/StructuredAttentionDepthEstimation)-official       

1. [PAD-Net: Multi-Tasks Guided Prediction-and-Distillation Network](https://arxiv.org/abs/1805.04409)    
cvpr 2018 *2018-05-11* [paper](https://arxiv.org/abs/1805.04409)     

1. [GeoNet: Geometric Neural Network for Joint Depth and Surface Normal Estimation](https://arxiv.org/abs/2012.06980)    
cvpr 2018 *2020-12-13* [paper](https://arxiv.org/abs/2012.06980)  | [tensorflow](https://github.com/xjqi/GeoNet)-official   
GeoNet


1. [Deep Ordinal Regression Network for Monocular Depth Estimation](https://arxiv.org/abs/1806.02446)    
cvpr 2018 *2018-06-06* [paper](https://arxiv.org/abs/1806.02446) | [caffe](https://github.com/hufu6371/DORN.git) | [pytorch](https://github.com/dontLoveBugs/DORN_pytorch.git)    
DORN    

1. [Joint Task-Recursive Learning for Semantic Segmentation and Depth Estimation](https://openaccess.thecvf.com/content_ECCV_2018/papers/Zhenyu_Zhang_Joint_Task-Recursive_Learning_ECCV_2018_paper.pdf)    
eccv 2018 *2018* [paper](https://openaccess.thecvf.com/content_ECCV_2018/papers/Zhenyu_Zhang_Joint_Task-Recursive_Learning_ECCV_2018_paper.pdf)    

1. [Look Deeper into Depth: Monocular Depth Estimation with Semantic Booster and Attention-Driven Loss](https://openaccess.thecvf.com/content_ECCV_2018/papers/Jianbo_Jiao_Look_Deeper_into_ECCV_2018_paper.pdf)    
eccv 2018 *2018* [paper](https://openaccess.thecvf.com/content_ECCV_2018/papers/Jianbo_Jiao_Look_Deeper_into_ECCV_2018_paper.pdf)   

1. [Depth Esimation via Affinity Learning with Convolutional Spatial Propagation Network](https://arxiv.org/abs/1808.00150)   
eccv 2018 *2018-08-01* [paper](https://arxiv.org/abs/1808.00150) | [pytorch](https://github.com/XinJCheng/CSPN)    
CSPN       

1. [SOSD-Net: Joint Semantic Object Segmentation and Depth Estimation from Monocular images](https://arxiv.org/abs/2101.07422)    
*2021-01-19* [paper](https://arxiv.org/abs/2101.07422)    


### 3.1.2 无/半监督

### 3.1.3 其他
1. [Deep Convolutional Neural Fields for Depth Estimation from a Single Image](http://arxiv.org/abs/1411.6387)    
cvpr 2015 *2014-12-18* [paper](http://arxiv.org/abs/1411.6387)    


## 3.2 分类任务


###  3.2.1 监督

1. [Deeper Depth Prediction with Fully Convolutional Residual Networks](http://cn.arxiv.org/abs/1606.00373)     
3dv 2016 *2016-06-01* [paper](https://arxiv.org/abs/1606.00373) | [tensorflow/matlab](https://github.com/MightyChaos/FCRN-DepthPrediction) | [tensorflow/matlab](https://github.com/iro-cp/FCRN-DepthPrediction)-official | [blog](https://blog.csdn.net/yjl9122/article/details/78670009)      
FCRN   


1. [Monocular depth estimation using relative depth maps](https://openaccess.thecvf.com/content_CVPR_2019/papers/Lee_Monocular_Depth_Estimation_Using_Relative_Depth_Maps_CVPR_2019_paper.pdf)    
cvpr 2019 *2019* [paper](https://openaccess.thecvf.com/content_CVPR_2019/papers/Lee_Monocular_Depth_Estimation_Using_Relative_Depth_Maps_CVPR_2019_paper.pdf) | [caffe](https://github.com/jaehanlee-mcl/monocular-depth-estimation-using-relative-depth-maps)-official     

1. [From Big to Small: Multi-Scale Local Planar Guidance for Monocular Depth Estimation](https://arxiv.org/abs/1907.10326)    
*2019-07-24* [paper](https://arxiv.org/abs/1907.10326)  | [pytorch-tensorflow](https://github.com/cleinc/bts)       
bts    

1. [Pattern-Affinitive Propagation across Depth, Surface Normal and Semantic Segmentation](https://arxiv.org/abs/1906.03525)    
cvpr 2019 *2019-06-08* [paper](https://arxiv.org/abs/1906.03525)   

1. [Exploiting temporal consistency for real-time video depth estimation](https://arxiv.org/abs/1908.03706)    
iccv 2019 *2019-08-10* [paper](https://arxiv.org/abs/1908.03706) | [pytorch](https://github.com/weihaox/ST-CLSTM)       


###  3.2.2 无/半监督


### 3.2.3 其他

1. [Estimating Depth from Monocular Images as Classification Using Deep Fully Convolutional Residual Networks](https://arxiv.org/abs/1605.02305)    
*2016-05-08* [paper](https://arxiv.org/abs/1605.02305)    


1. [Single image depth estimation by dilated deep residual convolutional neural network and soft-weight-sum inference](https://arxiv.org/abs/1705.00534)    
*2017-04-27* [paper](https://arxiv.org/abs/1705.00534)    
这篇论文主要采用了跳连接来改进网络结构，跳连接的结构有利于多尺度的融合，此外还使用了空洞卷积的方法来增加感受野。

## 3.3 其他


# 4 双目
3D CycleGAN   

# 5 其他
1. <span id="Make3DPDF">[Make3D: Learning 3D Scene Structure from a Single Still Image](http://www.cs.cornell.edu/~asaxena/reconstruction3d/saxena_make3d_learning3dstructure.pdf)</span>   
*2014* [paper](http://www.cs.cornell.edu/~asaxena/reconstruction3d/saxena_make3d_learning3dstructure.pdf)    
提出了 [Make3D](#Make3D) 数据集；        

1. [Deep3D: Automatic 2D-to-3D Video Conversion with Deep Convolutional Neural Networks](http://cn.arxiv.org/abs/1604.03650)   
2016 [Paper](https://arxiv.org/abs/1604.03650) | [MXNet](https://github.com/piiswrong/deep3d)        


1. <span id="ReDWebPDF">[Monocular Relative Depth Perception With Web Stereo Data Supervision](https://openaccess.thecvf.com/content_cvpr_2018/papers/Xian_Monocular_Relative_Depth_CVPR_2018_paper.pdf)</span>    
cvpr 2018 *2018* [paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Xian_Monocular_Relative_Depth_CVPR_2018_paper.pdf) | [home](https://sites.google.com/site/redwebcvpr18)     
提出了 [ReDWeb](#ReDWeb) 数据集；

1. <span id="IBimsPDF">[Evaluation of CNN-based Single-Image Depth Estimation Methods](https://arxiv.org/abs/1805.01328)</span>    
eccv 2018 *2018-05-03* [paper](https://arxiv.org/abs/1805.01328)    
提出了 [IBims-1](#IBims) 数据集；单反相机拍摄；并提出了一套新的评估标准；      


1. <span id="MannequinPDF">[Learning the Depths of Moving People by Watching Frozen People](https://arxiv.org/abs/1904.11111)</span>    
cvpr 2019 *2019-04-25* [paper](https://arxiv.org/abs/1904.11111) | [tensorflow](https://github.com/google/mannequinchallenge)-official   
提出了 [MannequinChallenge](#Mannequin) 数据集；   

1. [SharpNet: Fast and Accurate Recovery of Occluding Contours in Monocular Depth Estimation](http://cn.arxiv.org/abs/1905.08598)   
*2019-05-21* [paper](https://arxiv.org/abs/1905.08598)   

1. [Enhancing self-supervised monocular depth estimation with traditional visual odometry](http://cn.arxiv.org/abs/1908.03127)    
*2019-08-08* [paper](https://arxiv.org/abs/1908.03127)    

1. <span id="AIP-BrownPDF">[AI Playground: Unreal Engine-based Data Ablation Tool for Deep Learning](https://arxiv.org/abs/2007.06153)</span>    
*2020-07-13* [paper](https://arxiv.org/abs/2007.06153) | [pytorch](https://github.com/MMehdiMousavi/AIPlayground)      
**AIP-Brown**   

1. <span id="LeRes">[Learning to Recover 3D Scene Shape from a Single Image](https://arxiv.org/abs/2012.09365)</span>    
cvpr 2021 *2020-12-17* [paper](https://arxiv.org/abs/2012.09365) | [pytorch](https://github.com/aim-uofa/AdelaiDepth)-official | [pytorch](https://github.com/compphoto/BoostingMonocularDepth)-compphoto     
**LeRes**    

1. [Towards Continual, Online, Unsupervised Depth](https://arxiv.org/abs/2103.00369)    
*2021-03-02* [paper](https://arxiv.org/abs/2103.00369) | [pytorch](https://github.com/umarKarim/cou_stereo)-stereo-official | [pytorch](https://github.com/umarKarim/cou_sfm)-sfm-official     


1. <span id="MiDasPDF">[Boosting Monocular Depth Estimation Models to High-Resolution via Content-Adaptive Multi-Resolution Merging](https://arxiv.org/abs/2105.14021)</span>    
cvpr 2021 *2021-05-28* [paper](https://arxiv.org/abs/2105.14021) | [home](http://yaksoy.github.io/highresdepth/) | [pytorch](https://github.com/compphoto/BoostingMonocularDepth)-official      
**MiDas**    


1. <span id="GCNDepthPDF">[GCNDepth: Self-supervised Monocular Depth Estimation based on Graph Convolutional Network](https://arxiv.org/abs/2112.06782)</span>    
*2021-12-13* [paper](https://arxiv.org/abs/2112.06782) | [pytorch](https://github.com/ArminMasoumian/GCNDepth)-official     
**GCNDepth**   


1. <span id="GLPDepthPDF">[Global-Local Path Networks for Monocular Depth Estimation with Vertical CutDepth](https://arxiv.org/abs/2201.07436)</span>    
*2022-01-25* [paper](https://arxiv.org/abs/2201.07436) | [pytorch](https://github.com/vinvino02/GLPDepth) | [onnx](https://github.com/ibaiGorordo/ONNX-GLPDepth)       
**GLPDepth**   

# 6 顶会
## 6.1 CVPR 2020

1. [Generating and Exploiting Probabilistic Monocular Depth Estimates](https://arxiv.org/abs/1906.05739)    
cvpr 2020 *2019-06-13* [paper](https://arxiv.org/abs/1906.05739) | [tensorflow](https://github.com/likesum/prdepth)-official      
通用的有监督深度估计

1. [Uncertainty-Aware CNNs for Depth Completion: Uncertainty from Beginning to End](https://arxiv.org/abs/2006.03349)   
cvpr 2020 *2020-06-05* [paper](https://arxiv.org/abs/2006.03349)     
有监督深度补全，给出了不确定性度量   

1. [Structure-Guided Ranking Loss for Single Image Depth Prediction](https://openaccess.thecvf.com/content_CVPR_2020/papers/Xian_Structure-Guided_Ranking_Loss_for_Single_Image_Depth_Prediction_CVPR_2020_paper.pdf)    
cvpr 2020 *2020* [paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Xian_Structure-Guided_Ranking_Loss_for_Single_Image_Depth_Prediction_CVPR_2020_paper.pdf) | [pyctorch](https://github.com/KexianHust/Structure-Guided-Ranking-Loss)-official
有监督深度估计，提出了更好的loss

1. [Online Depth Learning Against Forgetting in Monocular Videos](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_Online_Depth_Learning_Against_Forgetting_in_Monocular_Videos_CVPR_2020_paper.pdf)    
*2020* [paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_Online_Depth_Learning_Against_Forgetting_in_Monocular_Videos_CVPR_2020_paper.pdf)     
实时深度学习搞定深度估计    

1. [Du2Net: Learning Depth Estimation from Dual-Cameras and Dual-Pixels](https://arxiv.org/abs/2003.14299)     
cvpr 2020 *2020-03-31* [paper](https://arxiv.org/abs/2003.14299)    


-------------------  
[TOP](#head){: .btn .btn--primary }


# 附录
## A 资源
1. [Robust Vision Challenge 2020](http://www.robustvision.net/index.php)   

### 文章
1. [基于深度学习的单目图像深度估计](https://zhuanlan.zhihu.com/p/47292734)     
1. [深度估计论文list](https://www.sunyehao.com/2019/04/11/%E6%B7%B1%E5%BA%A6%E4%BC%B0%E8%AE%A1%E8%AE%BA%E6%96%87list/)    
1. [https://github.com/scott89/awesome-depth](https://github.com/scott89/awesome-depth)   
1. [基于深度学习的单目深度估计综述](https://zhuanlan.zhihu.com/p/111759578)
1. [深度学习之单目深度估计 (Chapter.2)：无监督学习篇](https://zhuanlan.zhihu.com/p/29968267)
1. [单目深度估计技术进展综述](https://blog.csdn.net/MengYa_Dream/article/details/119924346)
1. [深度学习之单目深度估计](https://zhuanlan.zhihu.com/p/29864012)   

### 代码  
1. [https://github.com/nianticlabs/monodepth2](https://github.com/nianticlabs/monodepth2)（ICCV 2019）无监督   
2. [https://github.com/dwofk/fast-depth](https://github.com/dwofk/fast-depth) （ICRA 2019）   
3. [https://github.com/wangq95/KITTI_Dense_Depth](https://github.com/wangq95/KITTI_Dense_Depth)  监督学习  
4. [https://github.com/JunjH/Revisiting_Single_Depth_Estimation](https://github.com/JunjH/Revisiting_Single_Depth_Estimation) 监督学习   
1. [paper with code](https://paperswithcode.com/task/monocular-depth-estimation)    

## B 参考资料

## C 数据集

| 数据集 | 类型 | 数量（训练/验证/测试） | 分辨率 | 说明 | 发布日期 | best model | 论文 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [KITTI](http://www.cvlibs.net/datasets/kitti/) |  |  |  | 2个灰度相机，2个彩色相机，64线3D激光，1个GPS；<br>标签包含立体匹配结果、光流、场景流、深度估计、视觉测距、2D/3D目标检测、跟踪、道路/车道线检测、分割 |  | [GLPDepth](#GLPDepthPDF), DIFFNet |  |
| [NYUv2](https://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html) |  |  |  |  |  | [GLPDepth](#GLPDepthPDF), Semantic-aware NN |  |
| <span id="Make3D">[Make3D](http://make3d.cs.cornell.edu/data.html#make3d)</span> |  |  |  |  |  | [GCNDepth](#GCNDepthPDF) | [Make3D](#Make3DPDF) |
| [Middlebury2014](https://vision.middlebury.edu/stereo/data/scenes2014/) |  |  |  |  |  | [MiDas](#MiDasPDF) | [MiDas](#MiDasPDF) |
| [DIODE](https://diode-dataset.org/) |  |  |  | 室内场景 |  | [LeRes](#LeRes), [AIP-Brown](#AIP-BrownPDF) |  |
| <span id="ReDWeb">[ReDWeb](https://sites.google.com/site/redwebcvpr18)</span> |  |  |  | 室内外密集场景 |  |  | [ReDWeb](#ReDWebPDF) |
| <span id="Mannequin">[Mannequin](https://google.github.io/mannequinchallenge/www/index.html)</span> |  |  |  | 手持相机拍摄 |  |  | [Mannequin](#MannequinPDF) |
| <span id="IBims">[IBims-1](https://www.asg.ed.tum.de/lmf/ibims1/)</span> |  |  |  | 室内 |  | [LeRes](#LeRes) | [IBims](#IBimsPDF) |
| [WSVD]() |  |  |  | Web 视频 |  |  |  |
| [vKITTI](https://europe.naverlabs.com/Research/Computer-Vision/Proxy-Virtual-Worlds/) |  |  |  | KITTI 的虚拟数据集，“虚拟”指的是：旋转、清晨、晴天、多云、雾天、下雨等增强，共 14G 原始 RGB 图像，<br>包含检测、跟踪、分割；<br>这一数据集的意义在于可以缓解深度信息对于光线的敏感问题 |  |  |  |
| [Cityscapes](https://www.cityscapes-dataset.com/login/) |  |  |  | 德国的50多个城市的户外场景，包扩左右目图像、视差深度图、相机校准、车辆测距、行人检测、目标分割等，同时也包含有类似于vKITTI的虚拟渲染场景图像；<br>其中简单的左视角图像、相机标定、目标分割等数据需要利用学生账号注册获取，其他数据需要联系管理员获取； |  |  |  |
| []() ] |  |  |  |  |  |  |  |
| []() ] |  |  |  |  |  |  |  |
