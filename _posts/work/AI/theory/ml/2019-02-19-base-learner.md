---
title:  "「ML」 基学习器"
mathjax: true
key: base-learner-20190219
toc: true
toc_sticky: true
sidebar:
  nav: ML_Ensemble
category: [AI, ML, ensemble_learning]
---
<span id='head'></span>

## 一、 基分类器
**1. 常用的基分类器**[^1]  
最常用的基分类器是「决策树」：  
- 决策树不稳定，适合用集成学习来提升效果；  

除了决策树以外，神经网络也很适合；  

**2. 可否将随机森林中的基分类器由决策树替换为线性分类器或 KNN？**[^1]  
随机森林属于 Bagging 类的集成学习；Bagging 最大的好处就是集成后，分类器方差更小；  
而线性分类器和 KNN 都是较为稳定的分类器，本身方差就不大；使用 Bagging 后并不能获得更好的表现；甚至可能因为 Bagging 的采样，而导致他们在训练中更难收敛，从而增大了集成分类器的偏差；    

-------------------  
[TOP](#head){: .btn .btn--primary }


## 附录
### A 推荐资料

### B 参考资料
[^1]: 诸葛越. 百面机器学习[M]. 北京:人民邮电出版社. 2018.   

[^2]: 周志华. 机器学习[M]. 北京:清华大学出版社, 2016.   
