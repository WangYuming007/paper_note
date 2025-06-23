- **Exploring Hierarchical Spatial Layout Cues for 3D Point Cloud Based Scene Graph Prediction** · *Mingtao Feng et al.* · **IEEE Trans. Broadcast. 2023** · [Link](https://ieeexplore.ieee.org/abstract/document/10130401) · 引用 31

  对输入点云进行关系梳理，先垂直分层，再同层整理关系（用图卷积网络）

  ![image-20250618132717471](D:\files\typorapic\image-20250618132717471.png)

  - VoteNet 是一个用于 3D 点云目标检测的网络，VoteNet 给出了 i 个物体候选，每个候选对应一个特征向量 qᵢ。
  - Bi-LSTM（双向长短期记忆网络） 会对序列 {q₁, q₂, …, qᵢ} 同时从前向和后向进行编码，将前后两个方向的隐藏状态拼接（或相加）后，得到 cᵢ，表示第 i 个候选物体在全局对象序列中的上下文感知特征。
  - 单向 LSTM 层接受 cᵢ 作为输入，进一步通过一个单向 LSTM（通常是前向的)生成新的隐藏状态 hᵢ。
  - 输出：预测每个物体的类别 ô₁, ô₂, …, ôᵢ,Lobj是“分类损失”

- **LAM3D: Large Image-Point-Cloud Alignment Model for 3D Reconstruction   from Single Image** · *Ruikai Cui et al.* · **NeurIPS 2024** · [Link](https://arxiv.org/abs/2405.15622) · 引用 5

  让这个图像特征对齐点云特征。具体方法是第一阶段训练一个基于点云的encoder-decoder结构。第二阶段让图像特征对齐第一阶段的latent tri-plane。具体的对齐方法是用扩散模型。

  训练时需要图片+**对应的点云**，推理过程只需要图片。

  ![image-20250618152319509](D:\files\typorapic\image-20250618152319509.png)

- **SGRec3D: Self-Supervised 3D Scene Graph Learning via Object-Level Scene   Reconstruction** · *Sebastian Koch et al.* · **WACV 2024** · [Link](https://arxiv.org/abs/2309.15702) · 引用 16

- **CAST: Component-Aligned 3D Scene Reconstruction from an RGB Image** · *Kaixin Yao et al.* · **SIGRAPH 2025** · [Link](https://arxiv.org/abs/2502.12894) · 引用 0

  cast里面讲点云，标签，图像特征（而不是图像）输入扩散模型进行生成，具体方法参考下面的文献。

  ![image-20250620100853780](D:\files\typorapic\image-20250620100853780.png)

- **3DShape2VecSet: A 3D Shape Representation for Neural Fields and   Generative Diffusion Models** · *Biao Zhang et al.* · **SIGGRAPH 2023** · [Link](https://arxiv.org/abs/2301.11445) · 引用 0

  
  
  
  
  
  
  
