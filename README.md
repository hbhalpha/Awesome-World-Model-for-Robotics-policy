# Awesome World Models for Robotic Policy Learning

A curated list of papers, code, and resources on world models for robotic policy learning.

## World Model as Policy（Video-Generation / Image-Generation）

## Table of Contents
- [World Model as Policy ](#world-models-as-policy)
- [World Model as Simulator ](#world-models-as-simulator)
- [World Model for Video Generation](#world-models-for-gen)
- [Benchmarks for Evaluation World-Model](#benchmarks-for-evaluation-world-model)
- [Datasets](#datasets)

---

<a id="world-models-as-policy"></a>
## World Model as Policy

- **[NeurIPS'23] UniPi** — *Learning Universal Policies via Text-Guided Video Generation*
- [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=bo8q5MRcwy)[![arXiv](https://img.shields.io/badge/arXiv-2302.00111-b31b1b.svg)](https://arxiv.org/abs/2302.00111)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://universal-policy.github.io/)

- **[ICLR'24] GR-1** — *Unleashing Large-Scale Video Generative Pre-training for Visual Robot Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=NxoFmGgWC9)[![arXiv](https://img.shields.io/badge/arXiv-2312.13139-b31b1b.svg)](https://arxiv.org/abs/2312.13139)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/bytedance/GR-1)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gr1-manipulation.github.io/)

- **[arXiv'24.10] GR-2** — *GR-2: A Generative Video-Language-Action Model with Web-Scale Knowledge for Robot Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2410.06158-b31b1b.svg)](https://arxiv.org/abs/2410.06158)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gr2-manipulation.github.io/)

- **[NeurIPS'24] VidMan** — *VidMan: Exploiting Implicit Dynamics from Video Diffusion Model for Effective Robot Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=YbhHz0X2j5)[![arXiv](https://img.shields.io/badge/arXiv-2411.09153-b31b1b.svg)](https://arxiv.org/abs/2411.09153)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://jirufengyu.github.io/VidMan/)

- **[ICML'25] VPP** — *Video Prediction Policy: A Generalist Robot Policy with Predictive Visual Representations*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=c0dhw1du33)[![arXiv](https://img.shields.io/badge/arXiv-2412.14803-b31b1b.svg)](https://arxiv.org/abs/2412.14803)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/roboterax/video-prediction-policy)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://video-prediction-policy.github.io/)

- **[RSS'25] UVA** — *Unified Video Action Model*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://www.roboticsproceedings.org/rss21/p074.pdf)[![arXiv](https://img.shields.io/badge/arXiv-2503.00200-b31b1b.svg)](https://arxiv.org/abs/2503.00200)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/ShuangLI59/unified_video_action)

- **[RSS'25] UWM** — *Unified World Models: Coupling Video and Action Diffusion for Pretraining on Large Robotic Datasets*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://roboticsconference.org/program/papers/15/)[![arXiv](https://img.shields.io/badge/arXiv-2504.02792-b31b1b.svg)](https://arxiv.org/abs/2504.02792)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/WEIRDLabUW/unified-world-model)

- **[arXiv'25.06] Unified VLA (UniVLA)** — *Unified Vision-Language-Action Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2506.19850-b31b1b.svg)](https://arxiv.org/abs/2506.19850)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/baaivision/UniVLA)

- **[arXiv'25.07] DreamVLA** — *DreamVLA: A Vision-Language-Action Model Dreamed with Comprehensive World Knowledge*  
  [![arXiv](https://img.shields.io/badge/arXiv-2507.04447-b31b1b.svg)](https://arxiv.org/abs/2507.04447)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Zhangwenyao1/DreamVLA)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://zhangwenyao1.github.io/DreamVLA/)

- **[arXiv'25.08] VideoPolicy** — *Video Generators are Robot Policies*  
  [![arXiv](https://img.shields.io/badge/arXiv-2508.00795-b31b1b.svg)](https://arxiv.org/abs/2508.00795)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/cvlab-columbia/videopolicy)

- **[arXiv'25.08] Genie Envisioner** — *Genie Envisioner: A Unified World Foundation Platform for Robotic Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2508.05635-b31b1b.svg)](https://arxiv.org/abs/2508.05635)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/Genie-Envisioner)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://genie-envisioner.github.io/)

- **[arXiv'25.11] UD-VLA** — *Unified Diffusion VLA: Vision-Language-Action Model via Joint Discrete Denoising Diffusion Process*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.01718-b31b1b.svg)](https://arxiv.org/abs/2511.01718)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://irpn-eai.github.io/UD-VLA.github.io/)

- **[arXiv'25.11] RynnVLA-002** — *RynnVLA-002: A Unified Vision-Language-Action and World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.17502-b31b1b.svg)](https://arxiv.org/abs/2511.17502)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/alibaba-damo-academy/RynnVLA-002)

- **[arXiv'25.12] Video2Act** — *Video2Act: A Dual-System Video Diffusion Policy with Robotic Spatio-Motional Modeling*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.03044-b31b1b.svg)](https://arxiv.org/abs/2512.03044)

- **[arXiv'25.12] VideoVLA** — *VideoVLA: Video Generators Can Be Generalizable Robot Manipulators*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.06963-b31b1b.svg)](https://arxiv.org/abs/2512.06963)

- **[arXiv'25.12] Motus** — *Motus: A Unified Latent Action World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.13030-b31b1b.svg)](https://arxiv.org/abs/2512.13030)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/thu-ml/Motus)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://motus-robotics.github.io/motus)

- **[arXiv'25.12] mimic-video** — *mimic-video: Video-Action Models for Generalizable Robot Control Beyond VLAs*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.15692-b31b1b.svg)](https://arxiv.org/abs/2512.15692)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://mimic-video.github.io/)

- **[arXiv'25.12] LVP** — *Large Video Planner Enables Generalizable Robot Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.15840-b31b1b.svg)](https://arxiv.org/abs/2512.15840)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/buoyancy99/large-video-planner)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.boyuan.space/large-video-planner/)

- **[arXiv'25.12] Vidarc** — *Vidarc: Embodied Video Diffusion Model for Closed-loop Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.17661-b31b1b.svg)](https://arxiv.org/abs/2512.17661)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/thu-ml/vidar)

- **[arXiv'26.01] InternVLA-A1** — *InternVLA-A1: Unifying Understanding, Generation and Action for Robotic Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.02456-b31b1b.svg)](https://arxiv.org/abs/2601.02456)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/InternRobotics/InternVLA-A1)

- **[arXiv'26.01] Cosmos Policy** — *Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.16163-b31b1b.svg)](https://arxiv.org/abs/2601.16163)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVlabs/cosmos-policy)

- **[arXiv'26.01] TC-IDM** — *TC-IDM: Grounding Video Generation for Executable Zero-shot Robot Motion*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.18323-b31b1b.svg)](https://arxiv.org/abs/2601.18323)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/wsbaiyi/TC-IDM)

- **[arXiv'26.01] LingBot-VA** — *Causal World Modeling for Robot Control (LingBot-VA)*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.21998-b31b1b.svg)](https://arxiv.org/abs/2601.21998)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Robbyant/lingbot-va)

- **[arXiv'26.02] Visuo-Tactile World Models** — *Visuo-Tactile World Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.06001-b31b1b.svg)](https://arxiv.org/abs/2602.06001)

- **[arXiv'26.02] World-VLA-Loop** — *World-VLA-Loop: Closed-Loop Learning of Video World Model and VLA Policy*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.06508-b31b1b.svg)](https://arxiv.org/abs/2602.06508)[![GitHub](https://img.shields.io/badge/GitHub-repo-181717.svg?logo=github)](https://github.com/showlab/World-VLA-Loop)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://showlab.github.io/World-VLA-Loop/)

- **[arXiv'26.02] DreamDojo** — *DreamDojo: A Generalist Robot World Model from Large-Scale Human Videos*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.06949-b31b1b.svg)](https://arxiv.org/abs/2602.06949)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVIDIA/DreamDojo)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dreamdojo-world.github.io/)

- **[arXiv'26.02] BagelVLA** — *BagelVLA: Enhancing Long-Horizon Manipulation via Interleaved Vision-Language-Action Generation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.09849-b31b1b.svg)](https://arxiv.org/abs/2602.09849)

- **[arXiv'26.02] Say, Dream, and Act** — *Say, Dream, and Act: Learning Video World Models for Instruction-Driven Robot Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.10717-b31b1b.svg)](https://arxiv.org/abs/2602.10717)

- **[arXiv'26.02] VISTA** — *Scaling World Model for Hierarchical Manipulation Policies*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.10983-b31b1b.svg)](https://arxiv.org/abs/2602.10983)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://vista-wm.github.io/)

- **[arXiv'26.02] LDA-1B** — *LDA-1B: Scaling Latent Dynamics Action Model via Universal Embodied Data Ingestion*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.12215-b31b1b.svg)](https://arxiv.org/abs/2602.12215)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/jiangranlv/LDA-1B)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://pku-epic.github.io/LDA/)

- **[arXiv'26.02] DreamZero (WAM)** — *World Action Models are Zero-shot Policies (DreamZero)*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.15922-b31b1b.svg)](https://arxiv.org/abs/2602.15922)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/dreamzero0/dreamzero)

- **[arXiv'26.02] FRAPPE** — *FRAPPE: Infusing World Modeling into Generalist Policies via Multiple Future Representation Alignment*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.17259-b31b1b.svg)](https://arxiv.org/abs/2602.17259)

- **[arXiv'26.02] World Guidance (WoG)** — *World Guidance: World Modeling in Condition Space for Action Generation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.22010-b31b1b.svg)](https://arxiv.org/abs/2602.22010)[![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://selen-suyue.github.io/WoGNet/)

- **[ICLR'26] Horizon Imagination** — *Horizon Imagination: Efficient On-Policy Rollout in Diffusion World Models*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=Obefq4k8iG)[![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/leor-c/horizon-imagination)
