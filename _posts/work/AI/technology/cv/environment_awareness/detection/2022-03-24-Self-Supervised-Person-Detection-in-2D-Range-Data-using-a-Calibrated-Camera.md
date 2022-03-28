---
title:  "「论文解读」Self-Supervised Person Detection in 2D Range Data using a Calibrated Camera"
mathjax: true
key: SSPD
toc: true
toc_sticky: true
tags: Faster-RCNN
category: [AI, CV, retrieval, paper_reading]
---
<span id='head'></span>

>
论文发表时间：2020年12月  
论文地址：<https://arxiv.org/abs/2012.08890>  
官方代码：<https://github.com/VisualComputingInstitute/2D_lidar_person_detection>  

# 1 概述
为了解决单线激光行人检测缺乏数据集，引入相机，将图像中的检测结果映射到单线激光上，生成伪标签来做训练；    

# 2 主要工作
第一步： 生成伪标签   
<center class="half">
  <img src="/assets/images/cv/detection/SSPD/gen_pseudo_label.png" /><br>图1：生成伪标签&emsp;
</center>   

第二步：分析伪标签的质量    
第三步：提出新的训练策略     

# 3 细节
## 3.1 概念
**图像标签**：矩形框；    
**lidar 标签**：滑窗（中心点 + 半径）；     
**partially Huberized cross-entropy loss**:[^1]    
**mixup regularization**:[^2]   

## 3.2 基本操作

<span id="GenLabel">**确定标签**</span> ：   
- lidar 点裁剪
  - 根据外参，将图片检测结果的坐标映射到 lidar 坐标系，直接裁剪；    
- lidar 中行人位置的确定
  - k-means 聚类，聚出前景和背景两类；   
  - 取前景的中心为初始中心点；   
  - 用 0.5m 半径的均值漂移修正中心点；得到最终的位置；    


<span id="train">**训练**</span> ：   
0.4m 内作为分类的正样本；0.8m 内作为边界回归的正样本；`为什么要这么复杂`{: .notice--warning}     

## 3.3 问题
**生成标签失效的情况：**：

| 原因 | 示例1 | 示例2 |
| --- | --- | --- |
| heavy occlusion | <img src="/assets/images/cv/detection/SSPD/occlusion_0.png" /> | <img src="/assets/images/cv/detection/SSPD/occlusion_1.png" />  |
| background distraction | <img src="/assets/images/cv/detection/SSPD/background_distraction_0.png" /> | <img src="/assets/images/cv/detection/SSPD/background_distraction_1.png" /> |
| sparse LiDAR points at far distance | <img src="/assets/images/cv/detection/SSPD/sparse_0.png" /> | <img src="/assets/images/cv/detection/SSPD/sparse_1.png" /> |
| faulty calibration or synchronization between sensors | <img src="/assets/images/cv/detection/SSPD/faulty_calibration.png" /> | <img src="/assets/images/cv/detection/SSPD/faulty_sync.png" /> |

注：图片左边是相机中检测的人，右边的 + 是生成的激光伪标签（裁剪所得激光点，从中心向外扩展 0.5m）；     

# 4 实验
## 4.1 数据集


## 4.2 实验结果


# 5 总结

# 6 存在的问题
## 6.1 疑问
1 必须全部自己采集吗，能否复用开源数据集；    
{: .notice--success}   
需要图片和 lidar 同时采集才可以；也就意味着开源图片数据集无法复用；或许可以考虑 KITTI 等数据集；    

2 图像检测框只有左右，那么前后是怎么裁剪的；      
{: .notice--success}      
前后没有裁剪，只裁减了左右；当然，论文中过滤掉了检测框中心位置以上的 lidar 点；       

3 具体裁剪的流程是什么，怎么映射的；     
{: .notice--success}   
见[确定标签](#GenLabel)    

## 6.2 难点
- 针对标签失效的几个问题均无法处理；


-------------------  
[TOP](#head){: .btn .btn--primary }


[^1]: A. K. Menon, A. S. Rawat, S. J. Reddi, and S. Kumar, “Can gradient clipping mitigate label noise?,” in International    
[^2]: Conference on Learning Representations, 2020. H. Zhang, M. Cisse, Y. N. Dauphin, and D. Lopez-Paz, “mixup:
Beyond Empirical Risk Minimization,” in International Conference on Learning Representations, 2018.    

# 附录
## A 推荐资料
**损失函数**   
1. [A Detailed Guide to 7 Loss Functions for Machine Learning Algorithms with Python Code download Share](https://www.analyticsvidhya.com/blog/2019/08/detailed-guide-7-loss-functions-machine-learning-python-code/)   
1. [Machine Learning Glossary](https://ml-cheatsheet.readthedocs.io/en/latest/loss_functions.html)   

# 参考文献
