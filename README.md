# Road Sign Detection and Embedded Modeling Using Oblique Aerial Images

### 1. Abstract

Oblique photogrammetry-based three-dimensional (3D) urban models are widely used
for smart cities. In 3D urban models, road signs are small but provide valuable information for
navigation. However, due to the problems of sliced shape features, blurred texture and high incline
angles, road signs cannot be fully reconstructed in oblique photogrammetry, even with state-of-theart
algorithms. The poor reconstruction of road signs commonly leads to less informative guidance
and unsatisfactory visual appearance. In this paper, we present a pipeline for embedding road sign
models based on deep convolutional neural networks (CNNs). First, we present an end-to-end
balanced-learning framework for small object detection that takes advantage of the region-based
CNN and a data synthesis strategy. Second, under the geometric constraints placed by the bounding
boxes, we use the scale-invariant feature transform (SIFT) to extract the corresponding points on
the road signs. Third, we obtain the coarse location of a single road sign by triangulating the
corresponding points and refine the location via outlier removal. Least-squares fitting is then applied
to the refined point cloud to fit a plane for orientation prediction. Finally, we replace the road signs
with computer-aided design models in the 3D urban scene with the predicted location and orientation.
The experimental results show that the proposed method achieves a high mAP in road sign detection
and produces visually plausible embedded results, which demonstrates its effectiveness for road
sign modeling in oblique photogrammetry-based 3D scene reconstruction.

Please refer to the overall framework as bellow.

<img src="https://github.com/zmaomia/Road-Sign-Synthetic-Dataset/blob/main/Framework.png" width="900px">

### 2. Dataset Download

(1) Via 百度网盘

链接：https://pan.baidu.com/s/1M7uy1p05qQQ6MXh3y_QCSA

提取码：rsdd 


### 3. Demo for Triangulation

Triangulation code link: https://github.com/zmaomia/Triangulation-Projection


### 4. Paper 

Link:

https://www.mdpi.com/2072-4292/13/5/879

If our work is helpful, please cite with:

Mao, Zhu, Fan Zhang, Xianfeng Huang, Xiangyang Jia, Yiping Gong, and Qin Zou. 2021. "Deep Neural Networks for Road Sign Detection and Embedded Modeling Using Oblique Aerial Images" Remote Sensing 13, no. 5: 879. https://doi.org/10.3390/rs13050879
