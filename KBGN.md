## KBGN:Knowledge-Bridge Graph Network for Adaptive Vision-Text Reasoning in Visual Dialogue

**URL:**[https://arxiv.org/abs/2008.04858](https://arxiv.org/abs/2008.04858)  
**Code:**  
**Jnl./Conf.:**  ACM MM2020  
**Rate:**  

## 论文简介
视觉对话是一个动态持续性的过程。已有的方法仅仅将某一模态的全局表示作用于另一模态，忽略了不同模态实体与实体之间的隐含语义关系。本文提出知识桥图网络对视觉和文本信息间的语义关系更细粒度地建模，同时自适应地检索所需要的知识。另外，可以将推理过程展现出来。

## 创新点
2. 首次在视觉对话中使用图结构捕捉视觉和文本信息间潜在的语义关系。
## 方法
模型由知识编码，知识存储和知识检索三部分组成。
![](./images/KBGN01.png)
**知识编码部分:**   
分别对图像和文本信息进行编码，构建图结构。视觉的图节点是由Faster R-CNN提取到的对象,边由预训练好的边提取器初始化；文本中的图节点是每轮QA对。  
通过Qt分别对模态内的节点和边进行更新。
![](./images/KBGN02.png)   
![](./images/KBGN03.png)  
**知识存储：**   
将重要的知识和存储起来，并构建视觉和文本信息之间的隐含关系。  
![](./images/KBGN06.png)    
**知识检索：**  
![](./images/KBGN07.png)   
![](http://chart.googleapis.com/chart?cht=tx&chl= $M_F$)
## 启发
对Visual Dialogue这个任务不是很理解，可能需要去看下基础的论文。
