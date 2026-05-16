<div align="center">

# Awesome World Models for Robotic Policy Learning

[![arXiv](https://img.shields.io/badge/arXiv-2605.00080-b31b1b.svg)](https://arxiv.org/abs/2605.00080) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Paper-FFD21E)](https://huggingface.co/papers/2605.00080) [![Website](https://img.shields.io/badge/Website-Link-blue)](https://ntumars.github.io/wm-robot-survey/) [![GitHub](https://img.shields.io/badge/GitHub-Repo-181717.svg?logo=github)](https://github.com/NTUMARS/Awesome-World-Model-for-Robotics-Policy)

<p align="center">
  Bohan Hou<sup>1,*,†</sup>,
  Gen Li<sup>1,*</sup>,
  Jindou Jia<sup>1,*</sup>,
  Tuo An<sup>1,*</sup>,
  Xinying Guo<sup>1,*</sup>,
  Sicong Leng<sup>1</sup>,<br>
  Haoran Geng<sup>2</sup>,
  Yanjie Ze<sup>3</sup>,
  Tatsuya Harada<sup>4</sup>,
  Philip Torr<sup>5</sup>,
  Oier Mees<sup>6</sup>,
  Marc Pollefeys<sup>7</sup>,<br>
  Zhuang Liu<sup>8</sup>,
  Jiajun Wu<sup>3</sup>,
  Pieter Abbeel<sup>2</sup>,
  Jitendra Malik<sup>2</sup>,
  Yilun Du<sup>9</sup>,
  Jianfei Yang<sup>1,†</sup>
</p>

<p align="center">
  <sup>1</sup>Nanyang Technological University,
  <sup>2</sup>University of California, Berkeley,
  <sup>3</sup>Stanford University,<br>
  <sup>4</sup>The University of Tokyo,
  <sup>5</sup>University of Oxford,
  <sup>6</sup>Microsoft,
  <sup>7</sup>ETH Zurich,<br>
  <sup>8</sup>Princeton University,
  <sup>9</sup>Harvard University<br>
  <sup>*</sup>Equal Contribution (alphabetical order),
  <sup>†</sup>Corresponding Author
</p>

</div>

This repository accompanies our survey **World Model for Robot Learning: A Comprehensive Survey** — a policy-centric survey of predictive world models for robot policy learning, planning, simulation, evaluation, data generation, and robotic video generation.

- 📄 We maintain a curated list of papers, code, websites, models, benchmarks, and datasets on world models for robotic policy learning.
- 🤖 The list is organized around world models as policies, simulators, video-generation backbones, benchmarks, and datasets.
- 🤝 If you find missing papers, outdated links, or incorrect metadata, please feel free to open an issue or submit a pull request!

## Table of Contents

- [World Model as Policy](#world-models-as-policy)
  - [IDM-style Policies](#idm-style)
  - [Single-backbone Policies](#single-backbone)
  - [MoE/MoT-style Policies](#moe-mot-style)
  - [Unified VLA Models](#unified-vla)
  - [Latent-space World Modeling](#latent-space-wm)
- [World Model as Simulator](#world-models-as-simulator)
  - [World Model for Reinforcement Learning](#wm-for-rl)
  - [World Model for Evaluation](#wm-for-eval)
- [World Model for Video Generation](#world-models-for-gen)
- [Benchmarks for Evaluation World-Model](#benchmarks-for-evaluation-world-model)
- [Datasets](#datasets)

---

<a id="world-models-as-policy"></a>

## World Model as Policy

> World models（video generation models, unified models) used as backbone or components for improving Vision-Language-Action (VLA) policies. Organized by architectural paradigm following the taxonomy in our survey.

<a id="idm-style"></a>

### IDM-style Policies

> Inverse Dynamics Policies: first predict future visual trajectories, then use an inverse dynamics model to recover actions. Decoupled predict-then-act pipeline.

#### Early Subgoal-Image Instantiations

> Earlier instantiations leveraged image-editing diffusion models to predict subgoals for a goal-conditioned policy to follow.

- **[arXiv'23.10] SuSIE** — *Zero-Shot Robotic Manipulation with Pretrained Image-Editing Diffusion Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2310.10639-b31b1b.svg)](https://arxiv.org/abs/2310.10639) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://rail-berkeley.github.io/susie/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/kvablack/susie)

- **[ICRA'25] GHIL-Glue** — *GHIL-Glue: Hierarchical Control with Filtered Subgoal Images*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://ieeexplore.ieee.org/document/11128025) [![arXiv](https://img.shields.io/badge/arXiv-2410.20018-b31b1b.svg)](https://arxiv.org/abs/2410.20018) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/kyle-hatch-tri/ghil-glue) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://ghil-glue.github.io/)
  
#### Video-IDM Policies

- **[NeurIPS'23] UniPi** — *Learning Universal Policies via Text-Guided Video Generation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=bo8q5MRcwy) [![arXiv](https://img.shields.io/badge/arXiv-2302.00111-b31b1b.svg)](https://arxiv.org/abs/2302.00111) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://universal-policy.github.io/)

- **[ICLR'24] GR-1** — *Unleashing Large-Scale Video Generative Pre-training for Visual Robot Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=NxoFmGgWC9) [![arXiv](https://img.shields.io/badge/arXiv-2312.13139-b31b1b.svg)](https://arxiv.org/abs/2312.13139) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/bytedance/GR-1) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gr1-manipulation.github.io/)

- **[NeurIPS'24] VidMan** — *VidMan: Exploiting Implicit Dynamics from Video Diffusion Model for Effective Robot Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=YbhHz0X2j5) [![arXiv](https://img.shields.io/badge/arXiv-2411.09153-b31b1b.svg)](https://arxiv.org/abs/2411.09153) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/jirufengyu/VidMan) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://jirufengyu.github.io/VidMan/)

- **[ICML'25] VPP** — *Video Prediction Policy: A Generalist Robot Policy with Predictive Visual Representations*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=c0dhw1du33) [![arXiv](https://img.shields.io/badge/arXiv-2412.14803-b31b1b.svg)](https://arxiv.org/abs/2412.14803) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/roboterax/video-prediction-policy) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://video-prediction-policy.github.io/)

- **[CoRL'25] Gen2Act** — *Human Video Generation in Novel Scenarios Enables Generalizable Robot Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2409.16283-b31b1b.svg)](https://arxiv.org/abs/2409.16283) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://homangab.github.io/gen2act/)

- **[ICLR'25] V2A** — *Grounding Video Models to Actions through Goal Conditioned Exploration*  
  [![arXiv](https://img.shields.io/badge/arXiv-2411.07223-b31b1b.svg)](https://arxiv.org/abs/2411.07223) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/video-to-action/video-to-action-release)

- **[arXiv'25.12] Video2Act** — *Video2Act: A Dual-System Video Diffusion Policy with Robotic Spatio-Motional Modeling*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.03044-b31b1b.svg)](https://arxiv.org/abs/2512.03044) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/jiayueru/Video2Act) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://video2act.github.io/)

- **[arXiv'25.12] mimic-video** — *mimic-video: Video-Action Models for Generalizable Robot Control Beyond VLAs*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.15692-b31b1b.svg)](https://arxiv.org/abs/2512.15692) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://mimic-video.github.io/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/mimic-video/mimic-video) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/jonpai/mimic-video)

- **[arXiv'25.12] LVP** — *Large Video Planner Enables Generalizable Robot Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.15840-b31b1b.svg)](https://arxiv.org/abs/2512.15840) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/buoyancy99/large-video-planner) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.boyuan.space/large-video-planner/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/KempnerInstituteAI/LVP)

- **[arXiv'25.12] Vidarc** — *Vidarc: Embodied Video Diffusion Model for Closed-loop Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.17661-b31b1b.svg)](https://arxiv.org/abs/2512.17661) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/thu-ml/vidar) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://embodiedfoundation.github.io/vidar_anypos)

- **[arXiv'26.01] TC-IDM** — *TC-IDM: Grounding Video Generation for Executable Zero-shot Robot Motion*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.18323-b31b1b.svg)](https://arxiv.org/abs/2601.18323) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/wsbaiyi/TC-IDM) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://wsbaiyi.github.io/TC-IDM-Page/)

- **[arXiv'26.02] Say, Dream, and Act** — *Say, Dream, and Act: Learning Video World Models for Instruction-Driven Robot Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.10717-b31b1b.svg)](https://arxiv.org/abs/2602.10717)

#### Structured 3D-aware IDM Extensions

> A complementary line within the IDM family extracts 3D-aware motion structure (dense correspondences, hand trajectories, motion fields, 3D flow) from generated/demonstrated videos and uses it as a more action-relevant predictive prior.

- **[IROS'20] Hind4sight-Net** — *Hindsight for Foresight: Unsupervised Structured Dynamics Models from Physical Interaction*  
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)](https://ieeexplore.ieee.org/document/9341491) [![arXiv](https://img.shields.io/badge/arXiv-2008.00456-b31b1b.svg)](https://arxiv.org/abs/2008.00456) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/nematoli/hind4sight) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://hind4sight.cs.uni-freiburg.de/)

- **[ICLR'24] AVDC** — *Learning to Act from Actionless Videos through Dense Correspondences*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=Mhb5fpA1T0) [![arXiv](https://img.shields.io/badge/arXiv-2310.08576-b31b1b.svg)](https://arxiv.org/abs/2310.08576) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/flow-diffusion/AVDC) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://flow-diffusion.github.io/)

- **[CVPR'25] VidBot** — *VidBot: Learning Generalizable 3D Actions from In-the-Wild 2D Human Videos for Zero-Shot Robotic Manipulation*

- **[NeurIPS'25] Object-centric 3D Motion Field** — *Object-centric 3D Motion Field for Robot Learning from Human Videos*

- **[arXiv'26] NovaFlow** — *NovaFlow: Zero-shot Manipulation via Actionable Flow from Generated Videos*  
  [![arXiv](https://img.shields.io/badge/arXiv-2510.08568-b31b1b.svg)](https://arxiv.org/abs/2510.08568) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/rai-opensource/NovaFlow) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://novaflow.lhy.xyz/)

- **[arXiv'26.04] VAG** — *VAG: Dual-Stream Video-Action Generation for Embodied Data Synthesis*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.09330-b31b1b.svg)](https://arxiv.org/abs/2604.09330)

<a id="single-backbone"></a>

### Single-backbone Policies

> Unified Policies with Single World Model Backbone: a single shared backbone jointly models video and action through joint diffusion/prediction.

- **[RSS'25] UVA** — *Unified Video Action Model*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://www.roboticsproceedings.org/rss21/p074.pdf) [![arXiv](https://img.shields.io/badge/arXiv-2503.00200-b31b1b.svg)](https://arxiv.org/abs/2503.00200) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/ShuangLI59/unified_video_action) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://unified-video-action-model.github.io/)

- **[RSS'25] UWM** — *Unified World Models: Coupling Video and Action Diffusion for Pretraining on Large Robotic Datasets*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://roboticsconference.org/program/papers/15/) [![arXiv](https://img.shields.io/badge/arXiv-2504.02792-b31b1b.svg)](https://arxiv.org/abs/2504.02792) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/WEIRDLabUW/unified-world-model) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://weirdlabuw.github.io/uwm/)

- **[NeurIPS'25] VideoVLA** — *VideoVLA: Video Generators Can Be Generalizable Robot Manipulators*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=UPHlqbZFZB) [![arXiv](https://img.shields.io/badge/arXiv-2512.06963-b31b1b.svg)](https://arxiv.org/abs/2512.06963) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://videovla-nips2025.github.io/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/VideoVLA-Project/VideoVLA) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/VideoVLA/VideoVLA_Cogvideobase_Pretrained)

- **[ICLR'26] UD-VLA** — *Unified Diffusion VLA: Vision-Language-Action Model via Joint Discrete Denoising Diffusion Process*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=UvQOcw2oCD) [![arXiv](https://img.shields.io/badge/arXiv-2511.01718-b31b1b.svg)](https://arxiv.org/abs/2511.01718) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/OpenHelix-Team/Unified-Diffusion-VLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://irpn-eai.github.io/UD-VLA.github.io/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/chenpyyy/UD-VLA_CALVIN_ABCD_D)

- **[arXiv'25.08] VideoPolicy** — *Video Generators are Robot Policies*  
  [![arXiv](https://img.shields.io/badge/arXiv-2508.00795-b31b1b.svg)](https://arxiv.org/abs/2508.00795) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/cvlab-columbia/videopolicy) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://videopolicy.cs.columbia.edu)

- **[arXiv'26.01] Cosmos Policy** — *Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.16163-b31b1b.svg)](https://arxiv.org/abs/2601.16163) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVlabs/cosmos-policy) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://research.nvidia.com/labs/dir/cosmos-policy/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/collections/nvidia/cosmos-policy)

- **[arXiv'26.02] DreamZero (WAM)** — *World Action Models are Zero-shot Policies*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.15922-b31b1b.svg)](https://arxiv.org/abs/2602.15922) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/dreamzero0/dreamzero) [![Website](https://img.shields.io/badge/Website-NVIDIA-76B900.svg)](https://dreamzero0.github.io/)

- **[arXiv'26.03] GigaWorld-Policy** — *An Efficient Action-Centered World-Action Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.17240-b31b1b.svg)](https://arxiv.org/abs/2603.17240) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/open-gigaai/giga-world-policy) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gigaai-research.github.io/GigaWorld-Policy/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/open-gigaai)

- **[arXiv'26.04] MV-VDP** — *Multi-View Video Diffusion Policy: A 3D Spatio-Temporal-Aware Video Action Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.03181-b31b1b.svg)](https://arxiv.org/abs/2604.03181) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://lpy1219.github.io/MV-VDP-Web/)

- **[arXiv'26.04] Action Images** — *Action Images: End-to-End Policy Learning via Multiview Video Generation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.06168-b31b1b.svg)](https://arxiv.org/abs/2604.06168) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/UMass-Embodied-AGI/ActionImages)

<a id="moe-mot-style"></a>

### MoE/MoT-style Policies

> Expert World-Model Backbones: video and action experts remain separated, interacting through shared attention / cross-attention / MoT fusion.



#### Expert-Coupled / MoT Designs

- **[ICLR'26] GE-Act** — *Genie Envisioner's parallel flow-matching action expert with cross-attention to a video-diffusion world model*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=fHLtSxDFKC) [![arXiv](https://img.shields.io/badge/arXiv-2508.05635-b31b1b.svg)](https://arxiv.org/abs/2508.05635) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/Genie-Envisioner) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://genie-envisioner.github.io/)

- **[arXiv'25.12] Motus** — *Motus: A Unified Latent Action World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.13030-b31b1b.svg)](https://arxiv.org/abs/2512.13030) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/thu-ml/Motus) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://motus-robotics.github.io/motus) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/motus-robotics/Motus)

- **[arXiv'26.01] LingBot-VA** — *Causal World Modeling for Robot Control (LingBot-VA)*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.21998-b31b1b.svg)](https://arxiv.org/abs/2601.21998) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Robbyant/lingbot-va)

- **[arXiv'26.02] BagelVLA** — *BagelVLA: Enhancing Long-Horizon Manipulation via Interleaved Vision-Language-Action Generation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.09849-b31b1b.svg)](https://arxiv.org/abs/2602.09849) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://cladernyjorn.github.io/BagelVLA.github.io/)

- **[arXiv'26.02] LDA-1B** — *LDA-1B: Scaling Latent Dynamics Action Model via Universal Embodied Data Ingestion*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.12215-b31b1b.svg)](https://arxiv.org/abs/2602.12215) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/jiangranlv/LDA-1B) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://pku-epic.github.io/LDA/)

- **[arXiv'26.02] FRAPPE** — *FRAPPE: Infusing World Modeling into Generalist Policies via Multiple Future Representation Alignment*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.17259-b31b1b.svg)](https://arxiv.org/abs/2602.17259) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/OpenHelix-Team/frappe) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://h-zhao1997.github.io/frappe/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/collections/hhhJB/frappe)

- **[arXiv'26.02] World Guidance (WoG)** — *World Guidance: World Modeling in Condition Space for Action Generation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.22010-b31b1b.svg)](https://arxiv.org/abs/2602.22010) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Selen-Suyue/WoG) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://selen-suyue.github.io/WoGNet/)

- **[arXiv'26.03] DiT4DiT** — *Jointly Modeling Video Dynamics and Actions for Generalizable Robot Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.10448-b31b1b.svg)](https://arxiv.org/abs/2603.10448) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Mondo-Robotics/DiT4DiT) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dit4dit.github.io/)

- **[arXiv'26.03] Fast-WAM** — *Do World Action Models Need Test-Time Future Imagination?*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.16666-b31b1b.svg)](https://arxiv.org/abs/2603.16666) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/yuantianyuan01/FastWAM) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://yuantianyuan01.github.io/FastWAM/)

- **[arXiv'26.04] STARRY** — *STARRY: Spatial-Temporal Action-Centric World Modeling for Robotic Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.26848-b31b1b.svg)](https://arxiv.org/abs/2604.26848)

- **[arXiv'26.04] MotuBrain** — *MotuBrain: An Advanced World Action Model for Robot Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.27792-b31b1b.svg)](https://arxiv.org/abs/2604.27792) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.shengshu.com/en/motubrain)

- **[arXiv'26.04] WAV** — *World-Value-Action Model: Implicit Planning for Vision-Language-Action Systems*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.14732-b31b1b.svg)](https://arxiv.org/abs/2604.14732) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Win-commit/WAV) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://win-commit.github.io/wavpage/)

- **[arXiv'26.05] CKT-WAM** — *CKT-WAM: Parameter-Efficient Context Knowledge Transfer Between World Action Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2605.06247-b31b1b.svg)](https://arxiv.org/abs/2605.06247) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/YuhuaJiang2002/CKT-WAM)

<a id="unified-vla"></a>

### Unified VLA Models

> Unified Vision-Language-Action architectures that internalize world modeling as a training objective within a single multimodal backbone.

- **[ICLR'24] GR-1** — *Unleashing Large-Scale Video Generative Pre-training for Visual Robot Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=NxoFmGgWC9) [![arXiv](https://img.shields.io/badge/arXiv-2312.13139-b31b1b.svg)](https://arxiv.org/abs/2312.13139) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/bytedance/GR-1) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gr1-manipulation.github.io/)

- **[arXiv'24.10] GR-2** — *GR-2: A Generative Video-Language-Action Model with Web-Scale Knowledge for Robot Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2410.06158-b31b1b.svg)](https://arxiv.org/abs/2410.06158) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gr2-manipulation.github.io/)

- **[ICML'25] UP-VLA** — *A Unified Understanding and Prediction Model for Embodied Agent*  
  [![arXiv](https://img.shields.io/badge/arXiv-2501.18867-b31b1b.svg)](https://arxiv.org/abs/2501.18867) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/CladernyJorn/UP-VLA)

- **[NeurIPS'25] DreamVLA** — *DreamVLA: A Vision-Language-Action Model Dreamed with Comprehensive World Knowledge*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=PK07eretkF) [![arXiv](https://img.shields.io/badge/arXiv-2507.04447-b31b1b.svg)](https://arxiv.org/abs/2507.04447) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Zhangwenyao1/DreamVLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://zhangwenyao1.github.io/DreamVLA/)

- **[arXiv'25.05] UniVLA (task-centric latent actions)** — *UniVLA: Learning to Act Anywhere with Task-Centric Latent Actions*  
  [![arXiv](https://img.shields.io/badge/arXiv-2505.06111-b31b1b.svg)](https://arxiv.org/abs/2505.06111) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/OpenDriveLab/UniVLA)

- **[ICLR'26] Unified VLA (UniVLA)** — *Unified Vision-Language-Action Model*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=PklMD8PwUy) [![arXiv](https://img.shields.io/badge/arXiv-2506.19850-b31b1b.svg)](https://arxiv.org/abs/2506.19850) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/baaivision/UniVLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robertwyq.github.io/univla.github.io/)

- **[ICLR'26] Genie Envisioner** — *Genie Envisioner: A Unified World Foundation Platform for Robotic Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=fHLtSxDFKC) [![arXiv](https://img.shields.io/badge/arXiv-2508.05635-b31b1b.svg)](https://arxiv.org/abs/2508.05635) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/Genie-Envisioner) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://genie-envisioner.github.io/)

- **[CVPR'26] CoWVLA** — *Chain of World: World Model Thinking in Latent Motion*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.03195-b31b1b.svg)](https://arxiv.org/abs/2603.03195) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://fx-hit.github.io/cowvla-io/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/fx-hit/CoWVLA) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/hitfx/CoWVLA)

- **[arXiv'25.09] F1** — *A Vision-Language-Action Model Bridging Understanding and Generation to Actions*  
  [![arXiv](https://img.shields.io/badge/arXiv-2509.06951-b31b1b.svg)](https://arxiv.org/abs/2509.06951) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/InternRobotics/F1-VLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://aopolin-lv.github.io/F1-VLA/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/InternRobotics/F1-VLA)

- **[arXiv'25.11] RynnVLA-002** — *RynnVLA-002: A Unified Vision-Language-Action and World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.17502-b31b1b.svg)](https://arxiv.org/abs/2511.17502) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/alibaba-damo-academy/RynnVLA-002) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/Alibaba-DAMO-Academy/RynnVLA-002)

- **[arXiv'25.07] TriVLA** — *TriVLA: A Triple-System-Based Unified Vision-Language-Action Model for General Robot Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-2507.01424-b31b1b.svg)](https://arxiv.org/abs/2507.01424) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://zhenyangliu.github.io/TriVLA/)

- **[arXiv'26.01] InternVLA-A1** — *InternVLA-A1: Unifying Understanding, Generation and Action for Robotic Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.02456-b31b1b.svg)](https://arxiv.org/abs/2601.02456) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/InternRobotics/InternVLA-A1) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://internrobotics.github.io/internvla-a1.github.io/)

- **[arXiv'26.02] HALO** — *A Unified VLA Model for Embodied Multimodal Chain-of-Thought Reasoning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.21157-b31b1b.svg)](https://arxiv.org/abs/2602.21157)


- **[arXiv'26.05] OA-WAM** — *OA-WAM: Object-Addressable World Action Model for Robust Robot Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2605.06481-b31b1b.svg)](https://arxiv.org/abs/2605.06481)

<a id="latent-space-wm"></a>

### Latent-space World Modeling

> Policies with Latent-Space World Modeling: internalize future prediction in representation space without explicit video generation. JEPA-style approaches.

- **[CoRL'25] FLARE** — *Robot Learning with Implicit World Modeling*  
  [![arXiv](https://img.shields.io/badge/arXiv-2505.15659-b31b1b.svg)](https://arxiv.org/abs/2505.15659) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://research.nvidia.com/labs/gear/flare/)

- **[arXiv'26.02] VLA-JEPA** — *Enhancing Vision-Language-Action Model with Latent World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.10098-b31b1b.svg)](https://arxiv.org/abs/2602.10098) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/ginwind/VLA-JEPA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://ginwind.github.io/VLA-JEPA/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/ginwind/VLA-JEPA)

- **[arXiv'26.02] VISTA** — *Scaling World Model for Hierarchical Manipulation Policies*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.10983-b31b1b.svg)](https://arxiv.org/abs/2602.10983) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/vista-wm/Vista-WM) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://vista-wm.github.io/)

- **[arXiv'26.02] JEPA-VLA** — *Video Predictive Embedding is Needed for VLA Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.11832-b31b1b.svg)](https://arxiv.org/abs/2602.11832)

- **[arXiv'26.02] World Guidance (WoG)** — *World Guidance: World Modeling in Condition Space for Action Generation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.22010-b31b1b.svg)](https://arxiv.org/abs/2602.22010) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Selen-Suyue/WoG) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://selen-suyue.github.io/WoGNet/)

- **[arXiv'26.03] DIAL** — *Decoupling Intent and Action via Latent World Modeling for End-to-End VLA*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.29844-b31b1b.svg)](https://arxiv.org/abs/2603.29844) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://xpeng-robotics.github.io/dial) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/xpeng-robotics/DIAL) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/xpeng-robotics/DIAL_checkpoints)

- **[arXiv'26.04] AIM** — *Intent-Aware Unified World Action Modeling with Spatial Value Maps*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.11135-b31b1b.svg)](https://arxiv.org/abs/2604.11135) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Agentic-Intelligence-Lab/AIM)

- **[arXiv'26.04] DexWorldModel** — *DexWorldModel: Causal Latent World Modeling towards Automated Learning of Embodied Tasks*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.16484-b31b1b.svg)](https://arxiv.org/abs/2604.16484) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/DexForce/EmbodiChain)


---
<a id="world-models-as-simulator"></a>

## World Model as Simulator

> Beyond predictive conditioning, world models can serve as **interactive simulators**: given observations, instructions, and candidate actions, they roll out future states, provide feedback signals, and support downstream decision-making through imagined interaction. This section covers two complementary uses: reinforcement learning in learned simulators, and evaluation/planning through imagined rollouts.

<a id="wm-for-rl"></a>

### World Model for Reinforcement Learning

> World models as learned environments for policy improvement through imagined rollouts, replacing costly physical interaction.

- **[CoRL'23] DayDreamer** — *DayDreamer: World Models for Physical Robot Learning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2206.14176-b31b1b.svg)](https://arxiv.org/abs/2206.14176) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/danijar/daydreamer) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://danijar.com/project/daydreamer/)

- **[ICLR'24] UniSim** — *Learning Interactive Real-World Simulators*  
  [![arXiv](https://img.shields.io/badge/arXiv-2310.06114-b31b1b.svg)](https://arxiv.org/abs/2310.06114) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://universal-simulator.github.io/)

- **[CoRL'25] DiWA** — *DiWA: Diffusion Policy Adaptation with World Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2508.03645-b31b1b.svg)](https://arxiv.org/abs/2508.03645) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/acl21/diwa) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://diwa.cs.uni-freiburg.de/)

- **[arXiv'25.09] World-Env** — *World-Env: Leveraging World Model as a Virtual Environment for VLA Post-Training*  
  [![arXiv](https://img.shields.io/badge/arXiv-2509.24948-b31b1b.svg)](https://arxiv.org/abs/2509.24948) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/amap-cvlab/world-env)

- **[arXiv'25.09] World4RL** — *Diffusion World Models for Policy Refinement with Reinforcement Learning for Robotic Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2509.19080-b31b1b.svg)](https://arxiv.org/abs/2509.19080) [![Code](https://img.shields.io/badge/Code-repo-181717.svg)](https://anonymous.4open.science/r/World4RL-0410) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://world4rl.github.io/)

- **[arXiv'25.10] VLA-RFT** — *Vision-Language-Action Reinforcement Fine-tuning with Verified Rewards in World Simulators*  
  [![arXiv](https://img.shields.io/badge/arXiv-2510.00406-b31b1b.svg)](https://arxiv.org/abs/2510.00406) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/OpenHelix-Team/VLA-RFT) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://vla-rft.github.io/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/VLA-RFT)

- **[arXiv'25.11] ProphRL** — *Reinforcing Action Policies by Prophesying*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.20633-b31b1b.svg)](https://arxiv.org/abs/2511.20633) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://logosroboticsgroup.github.io/ProphRL)

- **[ICLR'26] WMPO** — *World Model-based Policy Optimization for Vision-Language-Action Models*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=qE2FyvRvuF) [![arXiv](https://img.shields.io/badge/arXiv-2511.09515-b31b1b.svg)](https://arxiv.org/abs/2511.09515) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/WM-PO/WMPO) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://wm-po.github.io/)

- **[CVPR'26] RehearseVLA** — *Simulated Post-Training for VLAs with Physically-Consistent World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2509.24948-b31b1b.svg)](https://arxiv.org/abs/2509.24948) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/amap-cvlab/world-env)

- **[arXiv'26.02] World-Gymnast** — *World-Gymnast: Training Robots with Reinforcement Learning in a World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.02454-b31b1b.svg)](https://arxiv.org/abs/2602.02454) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/world-gymnast/world-gymnast) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://world-gymnast.github.io/)

- **[arXiv'26.02] RISE** — *RISE: Self-Improving Robot Policy with Compositional World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.11075-b31b1b.svg)](https://arxiv.org/abs/2602.11075) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://opendrivelab.com/kai0-rl/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/OpenDriveLab/RISE)

- **[arXiv'26.02] VLAW** — *VLAW: Iterative Co-Improvement of Vision-Language-Action Policy and World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.12063-b31b1b.svg)](https://arxiv.org/abs/2602.12063) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sites.google.com/view/vlaw-arxiv)

- **[arXiv'26.02] GigaBrain-0.5M\*** — *a VLA That Learns From World Model-Based Reinforcement Learning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.12099-b31b1b.svg)](https://arxiv.org/abs/2602.12099) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/open-gigaai/giga-brain-0) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gigabrain05m.github.io/)

- **[arXiv'26.02] WoVR** — *WoVR: World Models as Reliable Simulators for Post-Training VLA Policies with RL*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.13977-b31b1b.svg)](https://arxiv.org/abs/2602.13977) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/RLinf/RLinf) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/collections/RLinf/wovr)

- **[arXiv'26.02] World-VLA-Loop** — *World-VLA-Loop: Closed-Loop Learning of Video World Model and VLA Policy*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.06508-b31b1b.svg)](https://arxiv.org/abs/2602.06508) [![GitHub](https://img.shields.io/badge/GitHub-repo-181717.svg?logo=github)](https://github.com/showlab/World-VLA-Loop) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://showlab.github.io/World-VLA-Loop/)

- **[arXiv'26.03] PlayWorld** — *Learning Robot World Models from Autonomous Play*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.09030-b31b1b.svg)](https://arxiv.org/abs/2603.09030) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robot-playworld.github.io/)

- **[arXiv'26.03] VLA-MBPO** — *Towards Practical World Model-based Reinforcement Learning for Vision-Language-Action Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.20607-b31b1b.svg)](https://arxiv.org/abs/2603.20607)

- **[arXiv'26.04] ViVa** — *ViVa: A Video-Generative Value Model for Robot Reinforcement Learning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.08168-b31b1b.svg)](https://arxiv.org/abs/2604.08168) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://viva-value-model.github.io/)

<a id="wm-for-eval"></a>

### World Model for Evaluation

> World models as evaluators: scoring candidate behaviors, ranking policies, supporting MPC planning, and enabling decision-time action selection through predictive rollout.

- **[ICLR'24] TD-MPC2** — *Scalable, Robust World Models for Continuous Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-2310.16828-b31b1b.svg)](https://arxiv.org/abs/2310.16828) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.tdmpc2.com/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/nicklashansen/tdmpc2)

- **[ICLR'26] WorldGym** — *WorldGym: World Model as An Environment for Policy Evaluation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=hidBHy1CAw) [![arXiv](https://img.shields.io/badge/arXiv-2506.00613-b31b1b.svg)](https://arxiv.org/abs/2506.00613) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/world-model-eval/world-model-eval) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://world-model-eval.github.io/abstract)


- **[ICLR'26] Horizon Imagination** — *Horizon Imagination: Efficient On-Policy Rollout in Diffusion World Models*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=Obefq4k8iG) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/leor-c/horizon-imagination)

- **[arXiv'25.05] WorldEval** — *WorldEval: World Model as Real-World Robot Policies Evaluator*  
  [![arXiv](https://img.shields.io/badge/arXiv-2505.19017-b31b1b.svg)](https://arxiv.org/abs/2505.19017) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/liyaxuanliyaxuan/Worldeval) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://worldeval.github.io/)

- **[arXiv'25.11] Scalable Policy Evaluation with Video World Models**  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.11520-b31b1b.svg)](https://arxiv.org/abs/2511.11520) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://miscsubmission.github.io/world_model_policy_eval/)

- **[arXiv'25.12] Evaluating Gemini Robotics Policies in a Veo World Simulator**  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.10675-b31b1b.svg)](https://arxiv.org/abs/2512.10675)

- **[RA-L'26] GPC** — *Inference-Time Enhancement of Generative Robot Policies via Predictive World Modeling*  
  [![arXiv](https://img.shields.io/badge/arXiv-2502.00622-b31b1b.svg)](https://arxiv.org/abs/2502.00622) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/han20192019/gpc_code)

- **[arXiv'26.03] DreamPlan** — *Efficient Reinforcement Fine-Tuning of Vision-Language Planners via Video World Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.16860-b31b1b.svg)](https://arxiv.org/abs/2603.16860) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://psi-lab.ai/DreamPlan/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/physical-superintelligence-lab/DreamPlan)

- **[arXiv'26.03] LeWorldModel** — *Stable End-to-End Joint-Embedding Predictive Architecture from Pixels*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.19312-b31b1b.svg)](https://arxiv.org/abs/2603.19312) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://le-wm.github.io/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/lucas-maes/le-wm)

- **[arXiv'25.06] V-JEPA 2** — *V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2506.09985-b31b1b.svg)](https://arxiv.org/abs/2506.09985) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/vjepa2)

- **[arXiv'26.03] V-JEPA 2.1** — *Unlocking Dense Features in Video Self-Supervised Learning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.14482-b31b1b.svg)](https://arxiv.org/abs/2603.14482) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://ai.meta.com/research/vjepa/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/vjepa2)

- **[arXiv'26.04] dWorldEval** — *dWorldEval: Scalable Robotic Policy Evaluation via Discrete Diffusion World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.22152-b31b1b.svg)](https://arxiv.org/abs/2604.22152) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dworldeval.github.io/)

- **[arXiv'26.05] FFDC-WAM** — *When to Trust Imagination: Adaptive Action Execution for World Action Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2605.06222-b31b1b.svg)](https://arxiv.org/abs/2605.06222)

---

<a id="world-models-for-gen"></a>

## World Model for Video Generation

> Video generation / video world models for robotics, including interactive simulators, imagination-based policy learning, and foundation video-world backbones that support robot learning.

- **[ICLR'24] Video Language Planning (VLP)** — *Video Language Planning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2310.10625-b31b1b.svg)](https://arxiv.org/abs/2310.10625) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/video-language-planning/vlp_code) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://video-language-planning.github.io/)

- **[CoRL'24] Dreamitate** — *Dreamitate: Real-World Visuomotor Policy Learning via Video Generation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=InT87E5sr4) [![arXiv](https://img.shields.io/badge/arXiv-2406.16862-b31b1b.svg)](https://arxiv.org/abs/2406.16862) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/cvlab-columbia/dreamitate) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dreamitate.cs.columbia.edu/)

- **[ICML'24] RoboDreamer** — *RoboDreamer: Learning Compositional World Models for Robot Imagination*  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v235/zhou24f.html) [![arXiv](https://img.shields.io/badge/arXiv-2404.12377-b31b1b.svg)](https://arxiv.org/abs/2404.12377) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/UMass-Embodied-AGI/robodreamer) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robovideo.github.io/)

- **[ICLR'25] DreMa** — *Dream to Manipulate: Compositional World Models Empowering Robot Imitation Learning with Imagination*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=3RSLW9YSgk) [![arXiv](https://img.shields.io/badge/arXiv-2410.04587-b31b1b.svg)](https://arxiv.org/abs/2410.04587) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/leobarcellona/drema_code) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dreamtomanipulate.github.io/)

- **[ICLR'25] CogVideoX** — *CogVideoX: Text-to-Video Diffusion Models with An Expert Transformer*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=LQzN6TRFg9) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/THUDM/CogVideo)

- **[CoRL'25] DreamGen** — *DreamGen: Unlocking Generalization in Robot Learning through Video World Models*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=3CnxNqmklv) [![arXiv](https://img.shields.io/badge/arXiv-2505.12705-b31b1b.svg)](https://arxiv.org/abs/2505.12705) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dreamgen-robot.github.io/)

- **[ICCV'25] PhysWorld** — *PhysWorld: Robot Learning from a Physical World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.07416-b31b1b.svg)](https://arxiv.org/abs/2511.07416) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://pointscoder.github.io/PhysWorld_Web/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/PointsCoder/OpenReal2Sim)

- **[ICCV'25] IRASim** — *IRASim: A Fine-Grained World Model for Robot Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-CVF-4B5D67.svg)](https://openaccess.thecvf.com/content/ICCV2025/html/Zhu_IRASim_A_Fine-Grained_World_Model_for_Robot_Manipulation_ICCV_2025_paper.html) [![arXiv](https://img.shields.io/badge/arXiv-2506.05034-b31b1b.svg)](https://arxiv.org/abs/2506.05034) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/bytedance/IRASim) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gen-irasim.github.io/)

- **[IROS'25] RoboEnvision** — *RoboEnvision: A Long-Horizon Video Generation Model for Multi-Task Robot Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2506.22007-b31b1b.svg)](https://arxiv.org/abs/2506.22007)

- **[ICLR'26] RoboMaster** — *Learning Video Generation for Robotic Manipulation with Collaborative Trajectory Control*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=OeDwYtp8n1) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/KlingAIResearch/RoboMaster) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](http://fuxiao0719.github.io/projects/robomaster)

- **[ICLR'26] Vid2World** — *Vid2World: Crafting Video Diffusion Models to Interactive World Models*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=pFyzqbUiF9) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/thuml/Vid2World) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://knightnemo.github.io/vid2world/)

- **[ICLR'26] Genie Envisioner** — *Genie Envisioner: A Unified World Foundation Platform for Robotic Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=fHLtSxDFKC) [![arXiv](https://img.shields.io/badge/arXiv-2508.05635-b31b1b.svg)](https://arxiv.org/abs/2508.05635) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/Genie-Envisioner) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://genie-envisioner.github.io/)

- **[ICLR'26] Ctrl-World** — *Ctrl-World: A Controllable Generative World Model for Robot Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=748bHL2BAv) [![arXiv](https://img.shields.io/badge/arXiv-2510.10125-b31b1b.svg)](https://arxiv.org/abs/2510.10125) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Robert-gyj/Ctrl-World) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://ctrl-world.github.io/)

- **[AAAI'26] Mask2IV** — *Mask2IV: Interaction-Centric Video Generation via Mask Trajectories*  
  [![arXiv](https://img.shields.io/badge/arXiv-2510.03135-b31b1b.svg)](https://arxiv.org/abs/2510.03135) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Reagan1311/Mask2IV) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://reagan1311.github.io/mask2iv/)

- **[arXiv'25.04] ManipDreamer** — *ManipDreamer: Boosting Robotic Manipulation World Model with Action Tree and Visual Guidance*  
  [![arXiv](https://img.shields.io/badge/arXiv-2504.16464-b31b1b.svg)](https://arxiv.org/abs/2504.16464) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://myendless1.github.io/ManipDreamer/)

- **[arXiv'25.04] TesserAct** — *TesserAct*  
  [![arXiv](https://img.shields.io/badge/arXiv-2504.20995-b31b1b.svg)](https://arxiv.org/abs/2504.20995) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/UMass-Embodied-AGI/TesserAct) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://tesseractworld.github.io/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/anyeZHY/tesseract)

- **[arXiv'25.05] EnerVerse-AC** — *EnerVerse-AC*  
  [![arXiv](https://img.shields.io/badge/arXiv-2505.09723-b31b1b.svg)](https://arxiv.org/abs/2505.09723) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/EnerVerse-AC) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://tesseractworld.github.io/)

- **[arXiv'25.09] WoW** — *WoW: Towards a World-omniscient World-model Through Embodied Interaction*  
  [![arXiv](https://img.shields.io/badge/arXiv-2509.22642-b31b1b.svg)](https://arxiv.org/abs/2509.22642) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/wow-world-model/wow-world-model)

- **[Tech Release'25.09] UnifoLM-WMA-0** — *UnifoLM-WMA-0: A World-Model-Action Framework for General-Purpose Robot Learning*  
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/unitreerobotics/unifolm-world-model-action) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://unigen-x.github.io/unifolm-world-model-action.github.io/)

- **[Tech Report'25.10] Cosmos Predict 2.5** — *Cosmos-Predict2.5: A Suite of Diffusion-based World Foundation Models*  
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/nvidia-cosmos/cosmos-predict2.5) [![Website](https://img.shields.io/badge/Website-NVIDIA-76B900.svg)](https://research.nvidia.com/labs/dir/cosmos-predict2.5/)

- **[arXiv'25.11] GigaWorld-0** — *GigaWorld-0*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.19861-b31b1b.svg)](https://arxiv.org/abs/2511.19861) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/EnerVerse-AC) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://giga-world-0.github.io/)

- **[arXiv'26.01] RoboVIP** — *RoboVIP: Multi-View Video Generation with Visual Identity Prompting Augments Robot Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.05241-b31b1b.svg)](https://arxiv.org/abs/2601.05241) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/RoboVIP/RoboVIP_VDM) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robovip.github.io/RoboVIP/)

- **[arXiv'26.02] DreamDojo** — *DreamDojo: A Generalist Robot World Model from Large-Scale Human Videos*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.06949-b31b1b.svg)](https://arxiv.org/abs/2602.06949) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVIDIA/DreamDojo) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dreamdojo-world.github.io/)

- **[arXiv'26.03] Interactive World Simulator** — *Interactive World Simulator for Robot Policy Training and Evaluation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.08546-b31b1b.svg)](https://arxiv.org/abs/2603.08546) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/WangYixuan12/interactive_world_sim) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.yixuanwang.me/interactive_world_sim/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/yixuan1999/interactive-world-sim-checkpoints)

- **[arXiv'26.03] ABot-PhysWorld** — *Interactive World Foundation Model for Robotic Manipulation with Physics Alignment*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.23376-b31b1b.svg)](https://arxiv.org/abs/2603.23376) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/amap-cvlab/ABot-PhysWorld)

- **[arXiv'26.03] EVA (model)** — *EVA: Aligning Video World Models with Executable Robot Actions via Inverse Dynamics Rewards*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.17808-b31b1b.svg)](https://arxiv.org/abs/2603.17808) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://eva-project-page.github.io/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/RobbinW/EVA) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/RobbinWang123/EVA)

> Note: this EVA is the action-controllable video world **model** (Wang et al., 2026); not to be confused with **EVA-Bench** (Chi et al., ICML'25) listed under Benchmarks.
- **[arXiv'26.03] Kinema4D** — *Kinema4D: Kinematic 4D World Modeling for Spatiotemporal Embodied Simulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.16669-b31b1b.svg)](https://arxiv.org/abs/2603.16669) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/mutianxu/Kinema4D)

- **[arXiv'26.03] Persistent Robot World Models** — *Persistent Robot World Models: Stabilizing Multi-Step Rollouts via Reinforcement Learning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.25685-b31b1b.svg)](https://arxiv.org/abs/2603.25685) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Jai2500/PersistWorld)

- **[arXiv'26.04] Cortex 2.0** — *Cortex 2.0: Grounding World Models in Real-World Industrial Deployment*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.20246-b31b1b.svg)](https://arxiv.org/abs/2604.20246)

- **[arXiv'26.04] X-WAM** — *Unified 4D World Action Modeling from Video Priors with Asynchronous Denoising*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.26694-b31b1b.svg)](https://arxiv.org/abs/2604.26694) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sharinka0715.github.io/X-WAM/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/sharinka0715/X-WAM)

- **[arXiv'26.05] EA-WM** — *EA-WM: Event-Aware Generative World Model with Structured Kinematic-to-Visual Action Fields*  
  [![arXiv](https://img.shields.io/badge/arXiv-2605.06192-b31b1b.svg)](https://arxiv.org/abs/2605.06192)

---

<a id="benchmarks-for-evaluation-world-model"></a>

## Benchmarks for Evaluation World-Model

> Benchmarks / evaluation suites for embodied world models, video world models, and world simulators.  
> **Cross-listing is intentional**: if a work releases both a benchmark and a dataset, it can appear here **and** in [Datasets](#datasets).

- **[ICML'25] EVA-Bench** — *benchmark introduced in **Empowering World Models with Reflection for Embodied Video Prediction** (EVA)*  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v267/chi25b.html) [![arXiv](https://img.shields.io/badge/arXiv-2410.15461-b31b1b.svg)](https://arxiv.org/abs/2410.15461) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/litwellchi/EmbodiedVideoAnticipator) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sites.google.com/view/eva-public)

- **[ICML'25] WorldSimBench** — *WorldSimBench: Towards Video Generation Models as World Simulators*  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v267/qin25f.html) [![arXiv](https://img.shields.io/badge/arXiv-2410.18072-b31b1b.svg)](https://arxiv.org/abs/2410.18072) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://iranqin.github.io/WorldSimBench.github.io/)

- **[BMVC'25] EWMBench** — *EWMBench: Evaluating Scene, Motion, and Semantic Quality in Embodied World Models*  
  [![Paper](https://img.shields.io/badge/Paper-BMVC-4B5D67.svg)](https://bmva-archive.org.uk/bmvc/2025/assets/papers/Paper_736/paper.pdf) [![arXiv](https://img.shields.io/badge/arXiv-2505.09694-b31b1b.svg)](https://arxiv.org/abs/2505.09694) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/EWMBench)

- **[CoRL'25] DreamGen Bench** — *benchmark introduced in **DreamGen: Unlocking Generalization in Robot Learning through Video World Models***  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v305/jang25a.html) [![arXiv](https://img.shields.io/badge/arXiv-2505.12705-b31b1b.svg)](https://arxiv.org/abs/2505.12705) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVIDIA/GR00T-Dreams) [![Website](https://img.shields.io/badge/Website-NVIDIA-76B900.svg)](https://research.nvidia.com/labs/gear/dreamgen)

- **[ICLR'26] World-in-World (WoW!)** — *World-in-World: World Models in a Closed-Loop World*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=yDmb7xAfeb) [![arXiv](https://img.shields.io/badge/arXiv-2510.18135-b31b1b.svg)](https://arxiv.org/abs/2510.18135) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/World-In-World/world-in-world) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://world-in-world.github.io/)

- **[arXiv'26.01] WoW-World-Eval** — *Wow, wo, val! A Comprehensive Embodied World Model Evaluation Turing Test*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.04137-b31b1b.svg)](https://arxiv.org/abs/2601.04137)

- **[arXiv'26.01] RBench** — *Rethinking Video Generation Model for the Embodied World*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.15282-b31b1b.svg)](https://arxiv.org/abs/2601.15282) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/DAGroup-PKU/ReVidgen) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dagroup-pku.github.io/ReVidgen.github.io/)

- **[arXiv'26.02] WorldArena** — *WorldArena: A Unified Benchmark for Evaluating Perception and Functional Utility of Embodied World Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.08971-b31b1b.svg)](https://arxiv.org/abs/2602.08971) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/tsinghua-fib-lab/WorldArena) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://world-arena.ai)

- **[ACL Findings'25] WM-ABench** — *Do Vision-Language Models Have Internal World Models? Towards an Atomic Evaluation*  
  [![Paper](https://img.shields.io/badge/Paper-ACL-4B5D67.svg)](https://aclanthology.org/2025.findings-acl.1342/) [![arXiv](https://img.shields.io/badge/arXiv-2506.21876-b31b1b.svg)](https://arxiv.org/abs/2506.21876) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://wm-abench.maitrix.org/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Dataset-FFD21E)](https://huggingface.co/datasets/maitrix-org/WM-ABench)

- **[arXiv'26.04] RoboWM-Bench** — *RoboWM-Bench: A Benchmark for Evaluating World Models in Robotic Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.19092-b31b1b.svg)](https://arxiv.org/abs/2604.19092) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/fffstrong/RoboWM-Bench)

- **[arXiv'26.01] DrivingGen** — *DrivingGen: A Comprehensive Benchmark for Generative Video World Models in Autonomous Driving*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.01528-b31b1b.svg)](https://arxiv.org/abs/2601.01528) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://drivinggen-bench.github.io/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/youngzhou1999/DrivingGen)

---

<a id="datasets"></a>

## Datasets

> Training datasets, preference datasets, and instruction-tuning datasets.  
> **Cross-listing is intentional**: if a work releases both datasets and benchmarks, it may appear here **and** in [Benchmarks for Evaluation World-Model](#benchmarks-for-evaluation-world-model).

### General-Purpose Trajectory Corpora & Cross-Embodiment

- **[CoRL'23] BridgeData V2** — *BridgeData V2: A Dataset for Robot Learning at Scale*  
  [![arXiv](https://img.shields.io/badge/arXiv-2308.12952-b31b1b.svg)](https://arxiv.org/abs/2308.12952) [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/rail-berkeley/bridge_data_v2) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://rail-berkeley.github.io/bridgedata/)

- **[ICRA'24] Open X-Embodiment (OXE)** — *Open X-Embodiment: Robotic Learning Datasets and RT-X Models*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://asu.elsevierpure.com/en/publications/open-x-embodiment-robotic-learning-datasets-and-rt-x-models-open-/) [![arXiv](https://img.shields.io/badge/arXiv-2310.08864-b31b1b.svg)](https://arxiv.org/abs/2310.08864) [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/google-deepmind/open_x_embodiment) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robotics-transformer-x.github.io/)

- **[RSS'24] DROID** — *DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://roboticsconference.org/2024/program/papers/120/) [![arXiv](https://img.shields.io/badge/arXiv-2403.12945-b31b1b.svg)](https://arxiv.org/abs/2403.12945) [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/droid-dataset/droid) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://droid-dataset.github.io/)

- **[IROS'25] AgiBot-World (Alpha/Beta)** — *AgiBot World Colosseo: A Large-scale Manipulation Platform for Scalable and Intelligent Embodied Systems*  
  [![arXiv](https://img.shields.io/badge/arXiv-2503.06669-b31b1b.svg)](https://arxiv.org/abs/2503.06669) [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/OpenDriveLab/AgiBot-World) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://agibot-world.com/)

- **[arXiv'25.09] Galaxea Open-World Dataset** — *Galaxea Open-World Dataset and G0 Dual-System VLA Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2509.00576-b31b1b.svg)](https://arxiv.org/abs/2509.00576) [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/OpenGalaxea/GalaxeaVLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://opengalaxea.github.io/G0/)

- **[arXiv'25.10] Humanoid Everyday** — *Humanoid Everyday: A Comprehensive Robotic Dataset for Open-World Humanoid Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2510.08807-b31b1b.svg)](https://arxiv.org/abs/2510.08807) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://humanoideveryday.github.io/) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Dataset-FFD21E)](https://huggingface.co/datasets/USC-PSI-Lab/humanoid-everyday)

- **[arXiv'25.12] RoboMIND 2.0** — *RoboMIND 2.0: A Multimodal, Bimanual Mobile Manipulation Dataset for Generalizable Embodied Intelligence*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.24653-b31b1b.svg)](https://arxiv.org/abs/2512.24653) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Open-X-Humanoid/RoboMIND-Sim) [![ModelScope](https://img.shields.io/badge/ModelScope-Dataset-624AFF.svg)](https://modelscope.cn/datasets/X-Humanoid/RoboMIND2.0)

- **[arXiv'24.05] BRMData** — *Empowering Embodied Manipulation: A Bimanual-Mobile Robot Manipulation Dataset for Household Tasks*  
  [![arXiv](https://img.shields.io/badge/arXiv-2405.18860-b31b1b.svg)](https://arxiv.org/abs/2405.18860) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Louis-ZhangLe/BRMData)

- **[RSS Workshop'23] RH20T** — *RH20T: A Robotic Dataset for Learning Diverse Skills in One-Shot*  
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://rh20t.github.io/)

- **[IROS'25] RH20T-P** — *RH20T-P: A Primitive-Level Robotic Manipulation Dataset Towards Composable Generalization Agents in Real-World Scenarios*  
  [![arXiv](https://img.shields.io/badge/arXiv-2403.19622-b31b1b.svg)](https://arxiv.org/abs/2403.19622) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sites.google.com/view/rh20t-primitive/main)

### UMI / Hand-Held Interface Family

- **[RSS'24] UMI** — *Universal Manipulation Interface: In-the-Wild Robot Teaching without In-the-Wild Robots*  
  [![arXiv](https://img.shields.io/badge/arXiv-2402.10329-b31b1b.svg)](https://arxiv.org/abs/2402.10329) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/real-stanford/universal_manipulation_interface) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://umi-gripper.github.io/)

- **[arXiv'25.09] MV-UMI** — *MV-UMI: A Scalable Multi-View Interface for Cross-Embodiment Learning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2509.18757-b31b1b.svg)](https://arxiv.org/abs/2509.18757) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://mv-umi.github.io/)

- **[arXiv'25.10] ActiveUMI** — *ActiveUMI: Robotic Manipulation with Active Perception from Robot-Free Human Demonstrations*  
  [![arXiv](https://img.shields.io/badge/arXiv-2510.01607-b31b1b.svg)](https://arxiv.org/abs/2510.01607) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://activeumi.github.io/)

- **[arXiv'25.10] FastUMI-100K** — *FastUMI-100K: Advancing Data-Driven Robotic Manipulation with a Large-scale UMI-style Dataset*  
  [![arXiv](https://img.shields.io/badge/arXiv-2510.08022-b31b1b.svg)](https://arxiv.org/abs/2510.08022) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/MrKeee/FastUMI-100K)

- **[arXiv'25.11] TWIST2** — *TWIST2: Scalable, Portable, and Holistic Humanoid Data Collection System*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.02832-b31b1b.svg)](https://arxiv.org/abs/2511.02832) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://yanjieze.com/TWIST2/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/amazon-far/TWIST2)

### Human-Video / Egocentric Priors

- **[ICRA'25] EgoMimic** — *EgoMimic: Scaling Imitation Learning via Egocentric Video*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://ieeexplore.ieee.org/document/11127989) [![arXiv](https://img.shields.io/badge/arXiv-2410.24221-b31b1b.svg)](https://arxiv.org/abs/2410.24221) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://egomimic.github.io/)

- **[RSS'25] DexWild** — *DexWild: Dexterous Human Interactions for In-the-Wild Robot Policies*  
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dexwild.github.io/)

- **[arXiv'25.07] Being-h0 (UniHand)** — *Being-h0: Vision-Language-Action Pretraining from Large-scale Human Videos*  
  [![arXiv](https://img.shields.io/badge/arXiv-2507.15597-b31b1b.svg)](https://arxiv.org/abs/2507.15597) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://beingbeyond.github.io/Being-H0/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/BeingBeyond/Being-H0) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/collections/BeingBeyond/being-h0)

- **[arXiv'26.01] Being-H0.5 (UniHand 2.0)** — *Being-H0.5: Scaling Human-Centric Robot Learning for Cross-Embodiment Generalization*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.12993-b31b1b.svg)](https://arxiv.org/abs/2601.12993) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://research.beingbeyond.com/being-h05) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/BeingBeyond/Being-H) [![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Model-FFD21E)](https://huggingface.co/collections/BeingBeyond/being-h05)

- **[arXiv'25.11] PHSD / In-N-On** — *In-N-On: Scaling Egocentric Manipulation with In-the-Wild and On-Task Data*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.15704-b31b1b.svg)](https://arxiv.org/abs/2511.15704) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://xiongyicai.github.io/In-N-On/)

### Tactile / Force / Contact-Rich Datasets

- **[arXiv'25.06] FreeTacMan** — *FreeTacMan: Robot-Free Visuo-Tactile Data Collection System for Contact-Rich Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2506.01941-b31b1b.svg)](https://arxiv.org/abs/2506.01941) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://opendrivelab.com/FreeTacMan) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/OpenDriveLab/FreeTacMan)

- **[arXiv'25.10] Humanoid Visual-Tactile-Action** — *A Humanoid Visual-Tactile-Action Dataset for Contact-Rich Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2510.25725-b31b1b.svg)](https://arxiv.org/abs/2510.25725)

- **[ICLR'25] VTDexManip** — *VTDexManip: A Dataset and Benchmark for Visual-Tactile Pretraining and Dexterous Manipulation with Reinforcement Learning*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=jf7C7EGw21)

- **[arXiv'25.12] Hoi!** — *Hoi!: A Multimodal Dataset for Force-Grounded, Cross-View Articulated Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.04884-b31b1b.svg)](https://arxiv.org/abs/2512.04884) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://timengelbracht.github.io/Hoi-Dataset-Website/)

### Synthetic / Recipe-Driven Datasets & Preference / Instruction-Tuning Sets

- **[arXiv'25.06] RoboTwin 2.0** — *RoboTwin 2.0: A Scalable Data Generator and Benchmark with Strong Domain Randomization for Robust Bimanual Robotic Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2506.18088-b31b1b.svg)](https://arxiv.org/abs/2506.18088) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robotwin-platform.github.io/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/robotwin-Platform/RoboTwin)

- **[ICML'25] EVA-Instruct** — *instruction-tuning dataset released with **Empowering World Models with Reflection for Embodied Video Prediction** (EVA)*  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v267/chi25b.html) [![arXiv](https://img.shields.io/badge/arXiv-2410.15461-b31b1b.svg)](https://arxiv.org/abs/2410.15461) [![GitHub](https://img.shields.io/badge/GitHub-code/data-181717.svg?logo=github)](https://github.com/litwellchi/EmbodiedVideoAnticipator) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sites.google.com/view/eva-public)

- **[ICML'25] HF-Embodied** — *human-preference dataset introduced in **WorldSimBench***  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v267/qin25f.html) [![arXiv](https://img.shields.io/badge/arXiv-2410.18072-b31b1b.svg)](https://arxiv.org/abs/2410.18072) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://iranqin.github.io/WorldSimBench.github.io/)

- **[arXiv'26.01] Action100M** — *Action100M: A Large-scale Video Action Dataset*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.10592-b31b1b.svg)](https://arxiv.org/abs/2601.10592) [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/facebookresearch/Action100M)

- **[arXiv'26.01] RoVid-X** — *training dataset released with **Rethinking Video Generation Model for the Embodied World***  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.15282-b31b1b.svg)](https://arxiv.org/abs/2601.15282) [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/DAGroup-PKU/ReVidgen) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dagroup-pku.github.io/ReVidgen.github.io/)

## Citations

If you find this repository useful, please consider citing the **original papers** listed above and/or citing this collection:

```bibtex
@misc{hou2026worldmodelrobotlearning,
  title         = {World Model for Robot Learning: A Comprehensive Survey},
  author        = {Bohan Hou and Gen Li and Jindou Jia and Tuo An and Xinying Guo and Sicong Leng and Haoran Geng and Yanjie Ze and Tatsuya Harada and Philip Torr and Oier Mees and Marc Pollefeys and Zhuang Liu and Jiajun Wu and Pieter Abbeel and Jitendra Malik and Yilun Du and Jianfei Yang},
  year          = {2026},
  eprint        = {2605.00080},
  archivePrefix = {arXiv},
  primaryClass  = {cs.RO},
  url           = {https://arxiv.org/abs/2605.00080}
}
```
