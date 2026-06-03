# Paper List

本文件根据当前 Zotero 本地库整理。3DGS 核心论文来自 `三维重建 / 3DGS / 3dgs` 集合中的基础方法；LucidDreamer 相关论文来自 `三维重建 / 3DGS / Luciddreamer` 集合，另将 `Luciddreamer其他论文` 集合作为补充列表。作者、年份和 Zotero Key 以本地 Zotero 元数据为准；缺失信息暂记为“未标注”。

## 3DGS Core Papers

这里只保留 3DGS 的基础核心论文，不展开列入 3DGS 扩展、应用型论文或综述。

| Title | Authors | Year | Zotero Key | Notes |
| --- | --- | --- | --- | --- |
| 3D Gaussian Splatting for Real-Time Radiance Field Rendering | Bernhard Kerbl; Georgios Kopanas; Thomas Leimkühler; George Drettakis | 2023 | QG4X6IF8 | 3DGS 原始方法论文，是本项目理解 LucidDreamer 场景表示与优化阶段的核心基础。 |

## LucidDreamer Collection

### LucidDreamer / 3D Scene Generation

| Title | Authors | Year | Zotero Key | Notes |
| --- | --- | --- | --- | --- |
| LucidDreamer: Domain-free Generation of 3D Gaussian Splatting Scenes | Jaeyoung Chung; Suyoung Lee; Hyeongjin Nam; Jaerin Lee; Kyoung Mu Lee | 2023 | EMGRSNNZ | 本项目直接研究对象。 |
| Text2Room: Extracting Textured 3D Meshes from 2D Text-to-Image Models | Lukas Höllein; Ang Cao; Andrew Owens; Justin Johnson; Matthias Nießner | 2023 | BDMBDBFH | 可作为两阶段视角扩展与补全流程的参考。 |
| SceneScape: Text-Driven Consistent Scene Generation | Rafail Fridman; Amit Abecasis; Yoni Kasten; Tali Dekel | 2023 | BCQQCMZ7 | 文本驱动一致性场景生成参考。 |
| WonderJourney: Going from Anywhere to Everywhere | Hong-Xing Yu; Haoyi Duan; Junhwa Hur; Kyle Sargent; Michael Rubinstein; William T. Freeman | 2024 | LBW8PNYN | 开放式场景扩展与连续生成参考。 |
| WonderWorld: Interactive 3D Scene Generation from a Single Image | 未标注 | 未标注 | 756KGSCJ | 交互式 3D 场景生成参考。 |
| PanoDreamer: Optimization-Based Single Image to 360 3D Scene With Diffusion | Avinash Paliwal; Xilong Zhou; Andrii Tsarov; Nima Khademi Kalantari | 2025 | K4RDDW6F | 单图到 360 场景生成参考。 |

### Camera Trajectory / NBV / Active View Selection

| Title | Authors | Year | Zotero Key | Notes |
| --- | --- | --- | --- | --- |
| Director3D: Real-world Camera Trajectory and 3D Scene Generation from Text | Xinyang Li; Zhangyu Lai; Linning Xu; Yansong Qu; Liujuan Cao; Shengchuan Zhang | 2024 | MWZG8Q8R | 文本条件相机轨迹生成，可作为全局 trajectory prior。 |
| GenDoP: Auto-regressive Camera Trajectory Generation as a Director of Photography | Mengchen Zhang; Tong Wu; Jing Tan; Ziwei Liu; Gordon Wetzstein; Dahua Lin | 2025 | G3BIYPIS | 自回归相机轨迹生成参考。 |
| CameraCtrl: Enabling Camera Control for Text-to-Video Generation | Hao He; Yinghao Xu; Yuwei Guo; Gordon Wetzstein; Bo Dai; Hongsheng Li | 2025 | KBG94LTV | 文本/视频生成中的相机控制参考。 |
| DG-NBV: A Cognitive Framework for Direct Generation of Next Best View in Continuous View Space | Zhicheng Liu; Zhiqiang Cao; Jianjie Li; Peiyu Guan; Junzhi Yu | 2025 | G5WVA8M2 | 连续空间中直接生成下一视角，可启发 pose generator。 |
| VIN-NBV: A View Introspection Network for Next-Best-View Selection | Noah Frahm; Dongxu Zhao; Andrea Dunn Beltran; Ron Alterovitz; Jan-Michael Frahm; Junier Oliva | 2025 | IVMY6T3D | 用视角价值预测重建质量提升，可启发 view evaluator。 |
| POp-GS: Next Best View in 3D-Gaussian Splatting with P-Optimality | Joey Wilson; Marcelino Almeida; Sachit Mahajan; Martin Labrie; Maani Ghaffari; Omid Ghasemalizadeh | 2025 | 37NE4VXM | 3DGS 专用 NBV 评分，可用于不确定性/信息增益。 |
| FisherRF: Active View Selection and Uncertainty Quantification for Radiance Fields using Fisher Information | Wen Jiang; Boshu Lei; Kostas Daniilidis | 2023 | U3LH655U | 基于 Fisher 信息的主动视角选择参考。 |
| ActiveNeRF: Learning Where to See with Uncertainty Estimation | Xuran Pan; Zihang Lai; Shiji Song; Gao Huang | 2022 | 3AB8EI6Y | NeRF 主动视角选择与不确定性估计参考。 |
| Neural Visibility Field for Uncertainty-Driven Active Mapping | Shangjie Xue; Jesse Dill; Pranay Mathur; Frank Dellaert; Panagiotis Tsiotras; Danfei Xu | 2024 | 3MUM22UG | 可见性不确定性建模参考。 |
| Active Neural Mapping at Scale | Zijia Kuang; Zike Yan; Hao Zhao; Guyue Zhou; Hongbin Zha | 2024 | BVZI6EDB | 大规模主动神经建图参考。 |

### RGB-D / Geometry / Multi-view Priors

| Title | Authors | Year | Zotero Key | Notes |
| --- | --- | --- | --- | --- |
| JointNet: Extending Text-to-Image Diffusion for Dense Distribution Modeling | Jingyang Zhang; Shiwei Li; Yuanxun Lu; Tian Fang; David McKinnon; Yanghai Tsin | 2023 | HDFDCQR4 | RGB-D 联合/稠密预测方向的重要参考。 |
| JointDiT: Enhancing RGB-Depth Joint Modeling with Diffusion Transformers | Kwon Byung-Ki; Qi Dai; Lee Hyoseok; Chong Luo; Tae-Hyun Oh | 2025 | BPTK7CKW | RGB-Depth 联合建模参考。 |
| DUSt3R: Geometric 3D Vision Made Easy | Shuzhe Wang; Vincent Leroy; Yohann Cabon; Boris Chidlovskii; Jerome Revaud | 2024 | UUPDV99E | 通用几何先验与匹配/重建参考。 |
| VGGT: Visual Geometry Grounded Transformer | Jianyuan Wang; Minghao Chen; Nikita Karaev; Andrea Vedaldi; Christian Rupprecht; David Novotny | 2025 | ZZHZ7YFM | 视觉几何基础模型参考。 |
| PanoVGGT: Feed-Forward 3D Reconstruction from Panoramic Imagery | Yijing Guo; Mengjun Chao; Luo Wang; Tianyang Zhao; Haizhao Dai; Yingliang Zhang | 2026 | SH5NHEXP | 全景输入下的前馈 3D 重建参考。 |
| ViewCrafter: Taming Video Diffusion Models for High-fidelity Novel View Synthesis | Wangbo Yu; Jinbo Xing; Li Yuan; Wenbo Hu; Xiaoyu Li; Zhipeng Huang | 2024 | X8CXFGAA | 视频扩散与新视角合成参考。 |

### 3DGS-related Generation / Refinement

| Title | Authors | Year | Zotero Key | Notes |
| --- | --- | --- | --- | --- |
| SA-ResGS: Self-Augmented Residual 3D Gaussian Splatting for Next Best View Selection | Kim Jun-Seong; Tae-Hyun Oh; Eduardo Pérez-Pellitero; Youngkyoon Jang | 2026 | PPS8VMPN | 3DGS 与 NBV 结合的近期参考。 |
| G4Splat: Geometry-Guided Gaussian Splatting with Generative Prior | Junfeng Ni; Yixin Chen; Zhifei Yang; Yu Liu; Ruijie Lu; Song-Chun Zhu | 2026 | C43255TP | 几何引导与生成先验结合的 3DGS 参考。 |

## LucidDreamer Other Papers

以下条目来自 Zotero 的 `Luciddreamer其他论文` 集合，主要作为场景生成、全景/多视图生成、视频世界模型和相关生成先验的补充阅读。

| Title | Authors | Year | Zotero Key |
| --- | --- | --- | --- |
| Text2Room: Extracting Textured 3D Meshes from 2D Text-to-Image Models | Lukas Höllein; Ang Cao; Andrew Owens; Justin Johnson; Matthias Nießner | 2023 | BDMBDBFH |
| WonderJourney: Going from Anywhere to Everywhere | Hong-Xing Yu; Haoyi Duan; Junhwa Hur; Kyle Sargent; Michael Rubinstein; William T. Freeman | 2024 | LBW8PNYN |
| DimensionX: Create Any 3D and 4D Scenes from a Single Image with Controllable Video Diffusion | Wenqiang Sun; Shuo Chen; Fangfu Liu; Zilong Chen; Yueqi Duan; Jun Zhang | 2024 | 56CWBCUD |
| 4Real: Towards Photorealistic 4D Scene Generation via Video Diffusion Models | Heng Yu; Chaoyang Wang; Peiye Zhuang; Willi Menapace; Aliaksandr Siarohin; Junli Cao | 2024 | M68CK5IS |
| 4K4DGen: Panoramic 4D Generation at 4K Resolution | Renjie Li; Panwang Pan; Bangbang Yang; Dejia Xu; Shijie Zhou; Xuanyang Zhang | 2024 | E2I2PFU2 |
| GenXD: Generating Any 3D and 4D Scenes | Yuyang Zhao; Chung-Ching Lin; Kevin Lin; Zhiwen Yan; Linjie Li; Zhengyuan Yang | 2024 | ZYT6D32S |
| MagicDrive: Street View Generation with Diverse 3D Geometry Control | Ruiyuan Gao; Kai Chen; Enze Xie; Lanqing Hong; Zhenguo Li; Dit-Yan Yeung | 2024 | 4SYXGDTD |
| Vista: A Generalizable Driving World Model with High Fidelity and Versatile Controllability | Shenyuan Gao; Jiazhi Yang; Li Chen; Kashyap Chitta; Yihang Qiu; Andreas Geiger | 2024 | YLRNX3TL |
| GameGen-X: Interactive Open-world Game Video Generation | Haoxuan Che; Xuanhua He; Quande Liu; Cheng Jin; Hao Chen | 2024 | YJKT4UQM |
| Guided Co-Modulated GAN for 360° Field of View Extrapolation | Mohammad Reza Karimi Dastjerdi; Yannick Hold-Geoffroy; Jonathan Eisenmann; Siavash Khodadadeh; Jean-François Lalonde | 2022 | 432RXRVW |
| LayerPano3D: Layered 3D Panorama for Hyper-Immersive Scene Generation | Shuai Yang; Jing Tan; Mengchen Zhang; Tong Wu; Yixuan Li; Gordon Wetzstein | 2025 | A2SH24HE |
| MVDiffusion: Enabling Holistic Multi-view Image Generation with Correspondence-Aware Diffusion | Shitao Tang; Fuyang Zhang; Jiacheng Chen; Peng Wang; Yasutaka Furukawa | 2023 | 4NHB3DPQ |
| Taming Stable Diffusion for Text to 360° Panorama Image Generation | Cheng Zhang; Qianyi Wu; Camilo Cruz Gambardella; Xiaoshui Huang; Dinh Phung; Wanli Ouyang | 2024 | JGKDIUG5 |
| PERF: Panoramic Neural Radiance Field from a Single Panorama | Guangcong Wang; Peng Wang; Zhaoxi Chen; Wenping Wang; Chen Change Loy; Ziwei Liu | 2023 | YWUPNRRG |
| Geometry-Free View Synthesis: Transformers and no 3D Priors | Robin Rombach; Patrick Esser; Bjorn Ommer | 2021 | UJ2YN7ZG |
| Infinite Nature: Perpetual View Generation of Natural Scenes from a Single Image | Andrew Liu; Richard Tucker; Varun Jampani; Ameesh Makadia; Noah Snavely; Angjoo Kanazawa | 2021 | 439ZNFTV |
| PixelSynth: Generating a 3D-Consistent Experience from a Single Image | Chris Rockwell; David F. Fouhey; Justin Johnson | 2021 | I83YHDB6 |
| Text2NeRF: Text-Driven 3D Scene Generation with Neural Radiance Fields | Jingbo Zhang; Xiaoyu Li; Ziyu Wan; Can Wang; Jing Liao | 2024 | RBY2EBUR |
| 3D Cinemagraphy from a Single Image | Xingyi Li; Zhiguo Cao; Huiqiang Sun; Jianming Zhang; Ke Xian; Guosheng Lin | 2023 | SSQE3R9N |
