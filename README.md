# 
PCPNET :Learning Local Shape Properties from Raw Point Clouds（EG18）
提出基于局部面片的法向量估计方法，以PointNet作为网络结构，有单尺度和多尺度。
Nesti-Net: Normal Estimation for Unstructured 3D Point Clouds using Convolutional Neural Networks（cvpr19）
使用专家网络来实现输入点云的邻域大小的自定义选择。
Neighbourhood-Insensitive Point Cloud Normal Estimation Network（BMVC20(oral)）
将自注意力机制引入到PCPNet框架中来进行法向量估计。
Geometric Attention for Prediction of Differential Properties in 3D Point Clouds（IAPR20）
对DGCNN进行改进，引入语义特征构建几何注意力矩阵，用以指导KNN。
DeepFit: 3D Surface Fitting via Neural Network Weighted Least Squares（ECCV20）
使用神经网络学习点云逐点点权重，用于加权最小二乘法的曲面拟合。
AdaFit: Rethinking Learning-based Normal Estimation on Point Clouds
在预测逐点权重的同时，为每个点预测一个位置偏移以迫使邻域曲面接近特定阶数。
Improvement of Normal Estimation for PointClouds via Simplifying Surface Fitting
在预测邻域中每个点的权重后，采用Top-K算法取最大的K个点以聚焦于关键部位来进行后续曲面的拟合。
Point Cloud Upsampling and Normal Estimation using Deep Learning for Robust Surface Reconstruction（cvpr2021）
以PointNet为主干，提取了局部面片和整体的特征进行拼接。再对拼接的特征进行MLP和reshape处理，回归个数扩充后的六维特征（点坐标、法向量）。提出一种复合损失函数。
Geometry and Learning Co-Supported Normal Estimation for Unstructured Point Cloud（cvpr20）
将所有点分为候选点（接近尖锐特征）和平滑点（远离尖锐特征），平滑点的法线通过PCA简单地计算，对于接近尖锐特征的候选点，采用不同尺度的邻域进行平面拟合计算法向量，如此一个尺度对应多个不同的法向量。接着通过为每一个尺度的局部邻域构建高度图，将法线和高度图输入到深度网络(NH-Net)中对法线进行微调。
DNF-Net: a Deep Normal Filtering Network for Mesh Denoising（tvcg20）
网格上的法向量滤波方法，使用多尺度的特征嵌入和残差网络实现法向量去噪。
