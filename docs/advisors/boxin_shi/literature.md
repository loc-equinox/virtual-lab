# 施柏鑫老师组部分论文整理

[实验室论文列表](https://camera.pku.edu.cn/publication?view=list)

## 方向一：智能传感与计算成像（Sensor）

### 基础背景
施老师组长期做 computational photography、computer vision，以及 event camera / neuromorphic camera 等新型视觉传感问题。

### 建议阅读论文
- [EventAid: Benchmarking event-aided image/video enhancement algorithms with real-captured hybrid dataset](https://camera.pku.edu.cn/publication?view=list)  
  TPAMI 2025。适合了解“事件相机 + 图像/视频增强”的 benchmark 思路，也能帮助你快速认识这个子领域到底在评测什么、难点是什么。

- [Self-supervised shutter unrolling with events](https://camera.pku.edu.cn/publication?view=list)  
  IJCV 2025。适合了解事件流如何帮助恢复快门过程中的时序信息，理解“传感机制 + 学习”的结合方式。

- [Dense metric depth estimation via event-based differential focus volume prompting](https://camera.pku.edu.cn/publication?view=list)  
  NeurIPS 2025。关注事件相机与深度估计，适合作为“事件数据不只是做重建，也可以做几何”的例子。

- [V2V: Scaling event-based vision through efficient video-to-voxel simulation](https://camera.pku.edu.cn/publication?view=list)  
  NeurIPS 2025。适合看“数据模拟器”路线：如果真实事件数据难采集、难标注，能不能从视频高效生成训练所需表示。

- [Learning to deblur polarized images](https://camera.pku.edu.cn/publication?view=list)  
  IJCV 2025。适合接触“偏振成像 + 低层视觉恢复”。

- [Revisiting one-stage deep uncalibrated photometric stereo via fourier embedding](https://camera.pku.edu.cn/publication?view=list)  
  TPAMI 2025。适合对光度立体、形状恢复和经典视觉问题感兴趣的同学。

---

## 方向二：生成式视觉与 AIGC

### 基础背景
从主页新闻和近两年论文可以看出，团队在视频生成、图像编辑、可控生成、全景视频、音视频同步生成等方向投入很多。2026 年 CVPR 接收工作里就包含 lighting-grounded video generation、audio-synced video editing、storyboard-to-cinematic multi-shot synthesis 等主题；2025 年 NeurIPS 接收工作也包含全景视频和音视频同步生成。  
来源：https://camera.pku.edu.cn/  
来源：https://camera.pku.edu.cn/publication?view=list

### 建议阅读论文
- [OpenCIR: Conditional image repainting with open condition mixture](https://camera.pku.edu.cn/publication?view=list)  
  TPAMI 2025。适合看“条件图像编辑”的更通用设定。

- [Affective image editing: Shaping emotional factors via text descriptions](https://camera.pku.edu.cn/publication?view=list)  
  IJCV 2025。一个比较有意思的方向：不仅编辑内容，也尝试编辑图像呈现的情绪因素。

- [Towards deeper emotional reflection: Crafting affective image filters with generative priors](https://camera.pku.edu.cn/publication?view=list)  
  TPAMI 2025。和上面一篇可以放在一起看，帮助理解“生成先验 + 情感表达”的结合方式。

- [PanoWan: Lifting diffusion video generation models to 360° with latitude/longitude-aware mechanisms](https://camera.pku.edu.cn/publication?view=list)  
  NeurIPS 2025。适合对视频生成、全景表示、几何一致性感兴趣的同学。

- [Audio-sync video generation with multi-stream temporal control](https://camera.pku.edu.cn/publication?view=list)  
  NeurIPS 2025。体现了团队在“可控视频生成”上的一条路线：不仅要生成，还要对齐音频和时序控制。
---

## 方向三：具身智能相关接口

### 基础背景
施老师组的“具身智能”更适合从感知与传感接口理解，而不是只把它看作机器人控制。论文页中能看到 camera-based tactile sensor、3D surface reconstruction、event-based depth 等议题，这些都与 embodied system 的 perception 模块密切相关。  
来源：https://camera.pku.edu.cn/publication?view=list

### 建议阅读论文
- [Gellight: Illumination design, modeling, and optimization for camera-based tactile sensor](https://camera.pku.edu.cn/publication?view=list)  
  AIS 2025。非常适合作为“视觉传感如何服务具身系统”的入门论文。它不是通用大模型式的 embodied AI，而是非常具体地处理 tactile sensing 这一关键问题。

- [Efficient 3D surface super-resolution via normal-based multimodal restoration](https://camera.pku.edu.cn/publication?view=list)  
  TPAMI 2025。适合把它看成“为操作、建模、交互提供更高质量表面几何”的支撑模块。

- [Reconstructing satellites in 3D from amateur telescope images](https://camera.pku.edu.cn/publication?view=list)  
  TPAMI 2025。虽然不是具身智能论文，但很适合作为“3D reconstruction + challenging imaging setup”的案例，帮助理解团队如何处理现实世界困难感知条件。
