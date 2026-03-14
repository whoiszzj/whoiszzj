🌐 Language / 语言

- **中文（默认）**
- <a href="#english-version">English</a>

---

<details open>
<summary><strong>🇨🇳 中文版本</strong></summary>

# 👋 你好，我是曾兆杰 | Zhaojie Zeng

华中科技大学博士生 | 3D视觉研究者  
多视图立体重建 · 神经渲染 · 3D Gaussian Splatting  

📧 zhaojiezeng@hust.edu.cn  
🔗 https://github.com/whoiszzj  

---

## 🧠 关于我

我目前是 **华中科技大学（HUST）计算机科学与技术学院** 的博士研究生，导师为 **管涛教授**。

我的研究方向主要包括：

- 多视图立体重建（Multi-View Stereo, MVS）
- 神经辐射场（Neural Radiance Fields, NeRF）
- 3D 高斯泼溅（3D Gaussian Splatting, 3DGS）
- 新视角合成（Novel View Synthesis）
- 大规模三维重建

### 学习路线

SfM → MVS → NeRF → 3DGS → GaussianImage / VGGT

---

## 🎓 教育经历

**华中科技大学（HUST）**  
计算机科学与技术学院

- 计算机科学与技术（ACM班） 本科，2017 – 2021  
  - 成绩排名前 5% （GPA: 3.97）
  - 国家奖学金（2019）

- 计算机科学与技术 全日制学术型硕士（保研），2021 – 2023  
- 计算机科学与技术 博士，2023 – 至今  

导师：管涛 教授

---

## 📄 学术论文

### 🏆 CCF-A 会议

**Adaptive Patch Deformation for Textureless-Resilient Multi-View Stereo**  
CVPR 2023  
[paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Wang_Adaptive_Patch_Deformation_for_Textureless-Resilient_Multi-View_Stereo_CVPR_2023_paper.pdf) | [github](https://github.com/whoiszzj/APD-MVS)
<details>
<summary>📄 摘要</summary>
在多视图立体重建（MVS）中，弱纹理区域由于缺乏可靠的视觉特征，难以建立稳定的像素匹配关系，因此一直是三维重建中的核心挑战。现有深度学习方法通常通过构建大规模代价体或扩大感受野来缓解该问题，但这会带来显著的显存开销并降低方法的可扩展性。本文提出一种自适应形变匹配框架 **Adaptive Patch Deformation (APD)**，通过根据局部几何结构对匹配 patch 进行动态形变，使其更好地贴合潜在的场景表面。该策略能够在保持较低计算开销的同时提升弱纹理区域的匹配鲁棒性。大量实验结果表明，该方法在多个标准数据集上显著提升了重建的完整性与精度，并优于现有的主流 MVS 方法。
</details>

**Frequency-Aware Density Control via Reparameterization for High-Quality Rendering of 3D Gaussian Splatting**  
AAAI 2025  
[paper](https://dl.acm.org/doi/10.1609/aaai.v39i9.33066) | [github](https://github.com/whoiszzj/FDS-GS)
<details>
<summary>📄 摘要</summary>
3D Gaussian Splatting（3DGS）是一种近年来提出的高效显式场景表示方法，能够实现实时的新视角渲染。然而，现有方法在整个场景范围内缺乏对 **高斯密度与尺度之间关系的显式约束**，导致模型常常使用尺度不合适的高斯来表达高频细节，从而影响渲染精度并增加冗余表示。针对这一问题，本文提出一种 **基于参数重参数化的密度—尺度耦合机制**，通过显式约束使高斯密度能够随频率变化而合理调整。在此基础上，进一步提出一种 **频率感知的密度控制策略**，包括在高频区域进行自适应 densification，以及通过尺度一致性过滤删除不合理尺度的高斯。实验结果表明，该方法在多个数据集上能够在使用更少高斯数量的情况下获得更高质量的渲染效果，并显著优于现有的 3DGS 方法。
</details>

**Instant GaussianImage: A Generalizable and Self-Adaptive Image Representation via 2D Gaussian Splatting**  
ICCV 2025  
[paper](https://openaccess.thecvf.com/content/ICCV2025/papers/Zeng_Instant_GaussianImage_A_Generalizable_and_Self-Adaptive_Image_Representation_via_2D_ICCV_2025_paper.pdf) | [github](https://github.com/whoiszzj/Instant-GI)
<details>
<summary>📄 摘要</summary>
近年来，高斯泼溅表示在高效场景建模和渲染方面展现出巨大潜力。然而，现有方法通常依赖场景特定的优化过程，在跨图像泛化能力方面仍然存在不足。本文提出 **Instant GaussianImage**，一种基于 **二维高斯表示的图像建模方法**，通过一组自适应高斯基元对图像进行紧凑表示。该方法通过高效的参数化与优化策略，实现快速训练，同时保持良好的结构和外观表达能力。实验结果表明，该方法在保证高质量图像重建的同时具有较强的泛化能力，为传统图像表示与基于高斯的神经渲染方法之间提供了一种新的统一视角。
</details>

### 🏅 期刊论文

**Matching Ambiguity-Resilient Multi-View Stereo via Adaptive Patch Deformation**  
Pattern Recognition（SCI Q1）  
[paper](https://www.sciencedirect.com/science/article/pii/S0031320325012567) | [github](https://github.com/whoiszzj/APDe-MVS)
<details>
<summary>📄 摘要</summary>
匹配歧义是多视图立体重建中的核心难题之一，尤其在弱纹理或重复纹理区域更为严重。本文提出一种 **基于自适应 patch 形变的抗歧义多视图立体重建方法**。与传统固定匹配窗口不同，该方法根据局部场景结构动态调整 patch 的形状，使其更好地适应真实表面结构，从而提升匹配的可靠性。同时，该方法在 PatchMatch 优化框架中结合光度一致性与几何约束，以进一步提升深度估计精度。大量实验结果表明，该方法在复杂场景下显著提高了三维重建的完整性与鲁棒性。
</details>

---

## 🚀 研究兴趣

- 几何感知的神经渲染（Geometry-aware Neural Rendering）
- 高效三维表示（Efficient 3D Representations）
- 基于高斯模型的密度控制（Density Control in Gaussian-based Models）
- 城市级可扩展三维重建（Scalable City-level 3D Reconstruction）
- 2D–3D 混合表示（Hybrid 2D–3D Representations）

---

## 🤝 合作与交流

欢迎以下类型的合作：

- 学术合作
- 科研实习
- 工业界 3D视觉应用
- 神经渲染系统工程

---

⭐ 如果你对 **3D Vision / Neural Rendering** 感兴趣，欢迎浏览我的仓库或与我联系！

</details>

---

<a name="english-version"></a>

<details>
<summary><strong>🇬🇧 English Version</strong></summary>

<!-- ↓↓↓ 下面这一段保持你原来的 README 完全不变 ↓↓↓ -->

# 👋 Hi, I'm Zhaojie Zeng (曾兆杰)

Ph.D. Candidate @ HUST | 3D Vision Researcher  
Multi-View Stereo · Neural Rendering · 3D Gaussian Splatting  

📧 zhaojiezeng@hust.edu.cn  
🔗 https://github.com/whoiszzj  

---

## 🧠 About Me

I am a Ph.D. candidate at **Huazhong University of Science and Technology (HUST)**, advised by Prof. Tao Guan.

My research focuses on:

- Multi-View Stereo (MVS)
- Neural Radiance Fields (NeRF)
- 3D Gaussian Splatting (3DGS)
- Novel View Synthesis
- Large-scale 3D Reconstruction

### Research Evolution

SfM → MVS → NeRF → 3DGS → GaussianImage / VGGT

---

## 🎓 Education

**Huazhong University of Science and Technology (HUST)**  
School of Computer Science & Technology

- B.E., Computer Science (ACM Class), 2017 – 2021  
  - Ranked Top 5% in cohort (GPA: 3.97)
  - National Scholarship (2019)

- M.S., Computer Science (Recommended Admission), 2021 – 2023  
- Ph.D., Computer Science, 2023 – Present

Advisor: Prof. Tao Guan

---

## 📄 Publications

### 🏆 CCF-A Conferences

**Adaptive Patch Deformation for Textureless-Resilient Multi-View Stereo**  
CVPR 2023, [paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Wang_Adaptive_Patch_Deformation_for_Textureless-Resilient_Multi-View_Stereo_CVPR_2023_paper.pdf), [github](https://github.com/whoiszzj/APD-MVS)
<details>
<summary>Abstract</summary>
Textureless regions remain a major challenge for multi-view stereo (MVS) because reliable correspondences are difficult to establish when local appearance lacks discriminative patterns. 
Most learning-based MVS methods address this issue by enlarging the receptive field or constructing large cost volumes, which leads to heavy memory consumption and limited scalability. 
This paper proposes Adaptive Patch Deformation (APD), a framework that dynamically deforms matching patches according to local geometric structures. 
By allowing patches to adapt to underlying surfaces, APD improves matching robustness in weak-texture areas while maintaining computational efficiency. 
Extensive experiments on benchmark datasets demonstrate that the proposed method significantly improves reconstruction completeness and accuracy compared with existing state-of-the-art MVS approaches.
</details>

**Frequency-Aware Density Control via Reparameterization for High-Quality Rendering of 3D Gaussian Splatting**  
AAAI 2025, [paper](https://dl.acm.org/doi/10.1609/aaai.v39i9.33066), [github](https://github.com/whoiszzj/FDS-GS)
<details>
<summary>📄 Abstract</summary>
3D Gaussian Splatting (3DGS) has recently emerged as an efficient explicit representation for real-time novel view synthesis. 
However, existing methods lack an explicit mechanism linking Gaussian density and scale across the scene, which often leads to improper-scale Gaussians being used to represent high-frequency details. 
This mismatch reduces rendering accuracy and introduces redundancy in the representation. 
To address this issue, this paper proposes a reparameterization strategy that explicitly couples Gaussian density with scale, ensuring consistency between the two factors during optimization. 
Based on this formulation, a frequency-aware density control framework is developed, including adaptive densification in high-frequency regions and scale-based filtering to remove improperly scaled Gaussians. 
Experimental results demonstrate that the proposed method achieves higher rendering quality while using fewer Gaussian primitives compared with state-of-the-art 3DGS approaches.
</details>

**Instant GaussianImage: A Generalizable and Self-Adaptive Image Representation via 2D Gaussian Splatting**  
ICCV 2025, [paper](https://openaccess.thecvf.com/content/ICCV2025/papers/Zeng_Instant_GaussianImage_A_Generalizable_and_Self-Adaptive_Image_Representation_via_2D_ICCV_2025_paper.pdf), [github](https://github.com/whoiszzj/Instant-GI)
<details>
<summary>📄 Abstract</summary>
Recent advances in Gaussian splatting have demonstrated strong potential for efficient scene representation and rendering. 
However, existing methods mainly focus on scene-specific optimization and often lack generalization ability across images. 
This paper introduces **Instant GaussianImage**, a novel 2D Gaussian-based representation that models images using adaptive Gaussian primitives. 
The proposed framework enables fast optimization while preserving structural and appearance information in a compact representation. 
By leveraging adaptive Gaussian parameterization and efficient optimization strategies, the method achieves high-quality image reconstruction and strong generalization ability across diverse image distributions. 
Experimental results show that Instant GaussianImage provides an effective bridge between traditional image representations and Gaussian-based neural rendering techniques.
</details>

### 🏅 Journal

**Matching Ambiguity-Resilient Multi-View Stereo via Adaptive Patch Deformation**  
Pattern Recognition (SCI Q1), [paper](https://www.sciencedirect.com/science/article/pii/S0031320325012567), [github](https://github.com/whoiszzj/APDe-MVS)
<details>
<summary>📄 Abstract</summary>
Matching ambiguity is a fundamental challenge in multi-view stereo reconstruction, particularly in regions with weak textures or repetitive patterns. 
This work proposes an ambiguity-resilient MVS framework based on adaptive patch deformation. 
Instead of relying on fixed matching windows, the proposed approach dynamically adjusts patch geometry according to local scene structures, enabling more reliable correspondence estimation. 
The method further integrates photometric consistency and geometric constraints within a PatchMatch-based optimization framework to improve depth estimation accuracy. 
Extensive experiments demonstrate that the proposed approach significantly improves reconstruction completeness and robustness in challenging scenarios.
</details>

---

## 🚀 Research Interests

- Geometry-aware neural rendering
- Efficient 3D representations
- Density control in Gaussian-based models
- Scalable city-level 3D reconstruction
- Hybrid 2D–3D representations

---

## 🤝 Open To

- Academic collaborations
- Research internships
- Industrial 3D vision applications
- Neural rendering systems engineering

---

⭐ If you are interested in 3D Vision / Neural Rendering, feel free to explore my repositories or reach out!

---

</details>
