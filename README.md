# Awesome World Models for Robotic Policy Learning

A curated list of papers, code, and resources on world models for robotic policy learning.

The repo is collected by [NTU MARS Lab](https://github.com/NTUMARS)

## Table of Contents
- [World Model for Policy ](#world-models-as-policy)
- [World Model for RL and Simulation ](#world-models-as-simulator)
- [World Model for Video Generation](#world-models-for-gen)
- [Benchmarks for Evaluation World-Model](#benchmarks-for-evaluation-world-model)
- [Datasets](#datasets)

---

<a id="world-models-as-policy"></a>
## World Model as Policy

> World models（video generation models, unified models) used as backbone or components for improving Vision-Language-Action (VLA) policies.


- **[NeurIPS'23] UniPi** — *Learning Universal Policies via Text-Guided Video Generation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=bo8q5MRcwy) [![arXiv](https://img.shields.io/badge/arXiv-2302.00111-b31b1b.svg)](https://arxiv.org/abs/2302.00111) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://universal-policy.github.io/)

- **[ICLR'24] GR-1** — *Unleashing Large-Scale Video Generative Pre-training for Visual Robot Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=NxoFmGgWC9) [![arXiv](https://img.shields.io/badge/arXiv-2312.13139-b31b1b.svg)](https://arxiv.org/abs/2312.13139) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/bytedance/GR-1) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gr1-manipulation.github.io/)

- **[NeurIPS'24] VidMan** — *VidMan: Exploiting Implicit Dynamics from Video Diffusion Model for Effective Robot Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=YbhHz0X2j5) [![arXiv](https://img.shields.io/badge/arXiv-2411.09153-b31b1b.svg)](https://arxiv.org/abs/2411.09153) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/jirufengyu/VidMan) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://jirufengyu.github.io/VidMan/)

- **[ICML'25] VPP** — *Video Prediction Policy: A Generalist Robot Policy with Predictive Visual Representations*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=c0dhw1du33) [![arXiv](https://img.shields.io/badge/arXiv-2412.14803-b31b1b.svg)](https://arxiv.org/abs/2412.14803) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/roboterax/video-prediction-policy) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://video-prediction-policy.github.io/)

- **[RSS'25] UVA** — *Unified Video Action Model*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://www.roboticsproceedings.org/rss21/p074.pdf) [![arXiv](https://img.shields.io/badge/arXiv-2503.00200-b31b1b.svg)](https://arxiv.org/abs/2503.00200) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/ShuangLI59/unified_video_action) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://unified-video-action-model.github.io/) 

- **[RSS'25] UWM** — *Unified World Models: Coupling Video and Action Diffusion for Pretraining on Large Robotic Datasets*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://roboticsconference.org/program/papers/15/) [![arXiv](https://img.shields.io/badge/arXiv-2504.02792-b31b1b.svg)](https://arxiv.org/abs/2504.02792) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/WEIRDLabUW/unified-world-model)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://weirdlabuw.github.io/uwm/)

- **[NeurIPS'25] DreamVLA** — *DreamVLA: A Vision-Language-Action Model Dreamed with Comprehensive World Knowledge*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=PK07eretkF) [![arXiv](https://img.shields.io/badge/arXiv-2507.04447-b31b1b.svg)](https://arxiv.org/abs/2507.04447) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Zhangwenyao1/DreamVLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://zhangwenyao1.github.io/DreamVLA/)

- **[NeurIPS'25] VideoVLA** — *VideoVLA: Video Generators Can Be Generalizable Robot Manipulators*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=UPHlqbZFZB) [![arXiv](https://img.shields.io/badge/arXiv-2512.06963-b31b1b.svg)](https://arxiv.org/abs/2512.06963) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://videovla-nips2025.github.io/)

- **[ICLR'26] Unified VLA (UniVLA)** — *Unified Vision-Language-Action Model*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=PklMD8PwUy) [![arXiv](https://img.shields.io/badge/arXiv-2506.19850-b31b1b.svg)](https://arxiv.org/abs/2506.19850) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/baaivision/UniVLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robertwyq.github.io/univla.github.io/)

- **[ICLR'26] UD-VLA** — *Unified Diffusion VLA: Vision-Language-Action Model via Joint Discrete Denoising Diffusion Process*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=UvQOcw2oCD) [![arXiv](https://img.shields.io/badge/arXiv-2511.01718-b31b1b.svg)](https://arxiv.org/abs/2511.01718) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/OpenHelix-Team/Unified-Diffusion-VLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://irpn-eai.github.io/UD-VLA.github.io/)

- **[ICLR'26] Genie Envisioner** — *Genie Envisioner: A Unified World Foundation Platform for Robotic Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=fHLtSxDFKC) [![arXiv](https://img.shields.io/badge/arXiv-2508.05635-b31b1b.svg)](https://arxiv.org/abs/2508.05635) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/Genie-Envisioner) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://genie-envisioner.github.io/)

- **[ICLR'26] Horizon Imagination** — *Horizon Imagination: Efficient On-Policy Rollout in Diffusion World Models*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=Obefq4k8iG) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/leor-c/horizon-imagination)


- **[arXiv'24.10] GR-2** — *GR-2: A Generative Video-Language-Action Model with Web-Scale Knowledge for Robot Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2410.06158-b31b1b.svg)](https://arxiv.org/abs/2410.06158) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gr2-manipulation.github.io/)

- **[arXiv'25.08] VideoPolicy** — *Video Generators are Robot Policies*  
  [![arXiv](https://img.shields.io/badge/arXiv-2508.00795-b31b1b.svg)](https://arxiv.org/abs/2508.00795) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/cvlab-columbia/videopolicy) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://videopolicy.cs.columbia.edu/)

- **[arXiv'25.11] RynnVLA-002** — *RynnVLA-002: A Unified Vision-Language-Action and World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.17502-b31b1b.svg)](https://arxiv.org/abs/2511.17502) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/alibaba-damo-academy/RynnVLA-002)

- **[arXiv'25.12] Video2Act** — *Video2Act: A Dual-System Video Diffusion Policy with Robotic Spatio-Motional Modeling*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.03044-b31b1b.svg)](https://arxiv.org/abs/2512.03044) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/jiayueru/Video2Act) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://video2act.github.io/)

- **[arXiv'25.12] Motus** — *Motus: A Unified Latent Action World Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.13030-b31b1b.svg)](https://arxiv.org/abs/2512.13030) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/thu-ml/Motus) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://motus-robotics.github.io/motus)

- **[arXiv'25.12] mimic-video** — *mimic-video: Video-Action Models for Generalizable Robot Control Beyond VLAs*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.15692-b31b1b.svg)](https://arxiv.org/abs/2512.15692) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://mimic-video.github.io/)

- **[arXiv'25.12] LVP** — *Large Video Planner Enables Generalizable Robot Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.15840-b31b1b.svg)](https://arxiv.org/abs/2512.15840) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/buoyancy99/large-video-planner) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.boyuan.space/large-video-planner/)

- **[arXiv'25.12] Vidarc** — *Vidarc: Embodied Video Diffusion Model for Closed-loop Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-2512.17661-b31b1b.svg)](https://arxiv.org/abs/2512.17661) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/thu-ml/vidar) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://embodiedfoundation.github.io/vidar_anypos)

- **[arXiv'26.01] InternVLA-A1** — *InternVLA-A1: Unifying Understanding, Generation and Action for Robotic Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.02456-b31b1b.svg)](https://arxiv.org/abs/2601.02456) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/InternRobotics/InternVLA-A1) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://internrobotics.github.io/internvla-a1.github.io/)

- **[arXiv'26.01] Cosmos Policy** — *Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.16163-b31b1b.svg)](https://arxiv.org/abs/2601.16163) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVlabs/cosmos-policy) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://research.nvidia.com/labs/dir/cosmos-policy/)

- **[arXiv'26.01] TC-IDM** — *TC-IDM: Grounding Video Generation for Executable Zero-shot Robot Motion*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.18323-b31b1b.svg)](https://arxiv.org/abs/2601.18323) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/wsbaiyi/TC-IDM) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://wsbaiyi.github.io/TC-IDM-Page/)

- **[arXiv'26.01] LingBot-VA** — *Causal World Modeling for Robot Control (LingBot-VA)*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.21998-b31b1b.svg)](https://arxiv.org/abs/2601.21998) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Robbyant/lingbot-va)

- **[arXiv'26.02] World-VLA-Loop** — *World-VLA-Loop: Closed-Loop Learning of Video World Model and VLA Policy*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.06508-b31b1b.svg)](https://arxiv.org/abs/2602.06508) [![GitHub](https://img.shields.io/badge/GitHub-repo-181717.svg?logo=github)](https://github.com/showlab/World-VLA-Loop) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://showlab.github.io/World-VLA-Loop/)

- **[arXiv'26.02] BagelVLA** — *BagelVLA: Enhancing Long-Horizon Manipulation via Interleaved Vision-Language-Action Generation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.09849-b31b1b.svg)](https://arxiv.org/abs/2602.09849)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://cladernyjorn.github.io/BagelVLA.github.io/) 

- **[arXiv'26.02] Say, Dream, and Act** — *Say, Dream, and Act: Learning Video World Models for Instruction-Driven Robot Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.10717-b31b1b.svg)](https://arxiv.org/abs/2602.10717) 

- **[arXiv'26.02] VISTA** — *Scaling World Model for Hierarchical Manipulation Policies*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.10983-b31b1b.svg)](https://arxiv.org/abs/2602.10983) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/vista-wm/Vista-WM) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://vista-wm.github.io/)

- **[arXiv'26.02] LDA-1B** — *LDA-1B: Scaling Latent Dynamics Action Model via Universal Embodied Data Ingestion*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.12215-b31b1b.svg)](https://arxiv.org/abs/2602.12215) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/jiangranlv/LDA-1B) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://pku-epic.github.io/LDA/)

- **[arXiv'26.02] DreamZero (WAM)** — *World Action Models are Zero-shot Policies*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.15922-b31b1b.svg)](https://arxiv.org/abs/2602.15922) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/dreamzero0/dreamzero) [![Website](https://img.shields.io/badge/Website-NVIDIA-76B900.svg)](https://dreamzero0.github.io/)

- **[arXiv'26.02] FRAPPE** — *FRAPPE: Infusing World Modeling into Generalist Policies via Multiple Future Representation Alignment*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.17259-b31b1b.svg)](https://arxiv.org/abs/2602.17259) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/OpenHelix-Team/frappe)

- **[arXiv'26.02] World Guidance (WoG)** — *World Guidance: World Modeling in Condition Space for Action Generation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.22010-b31b1b.svg)](https://arxiv.org/abs/2602.22010) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Selen-Suyue/WoG) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://selen-suyue.github.io/WoGNet/)

<a id="world-models-as-simulator"></a>
## World Model for RL and Simulation 
> World models used as **learned simulators**, **reward providers**, or **imagination environments** for improving Vision-Language-Action (VLA) policies.

---


- **[ICLR'26] WMPO** — *World Model-based Policy Optimization for Vision-Language-Action Models*  
   [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=qE2FyvRvuF) [![arXiv](https://img.shields.io/badge/arXiv-2511.09515-b31b1b.svg)](https://arxiv.org/abs/2511.09515) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/WM-PO/WMPO) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://wm-po.github.io/)

- **[arXiv'25.09] World-Env** — *World-Env: Leveraging World Model as a Virtual Environment for VLA Post-Training*  
   [![arXiv](https://img.shields.io/badge/arXiv-2509.24948-b31b1b.svg)](https://arxiv.org/abs/2509.24948) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/amap-cvlab/world-env)

- **[arXiv'25.10] VLA-RFT** — *Vision-Language-Action Reinforcement Fine-tuning with Verified Rewards in World Simulators*  
   [![arXiv](https://img.shields.io/badge/arXiv-2510.00406-b31b1b.svg)](https://arxiv.org/abs/2510.00406) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/OpenHelix-Team/VLA-RFT) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://vla-rft.github.io/)

- **[arXiv'26.02] World-Gymnast** — *World-Gymnast: Training Robots with Reinforcement Learning in a World Model*  
   [![arXiv](https://img.shields.io/badge/arXiv-2602.02454-b31b1b.svg)](https://arxiv.org/abs/2602.02454) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/world-gymnast/world-gymnast) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://world-gymnast.github.io/)

- **[arXiv'26.02] RISE** — *RISE: Self-Improving Robot Policy with Compositional World Model*  
   [![arXiv](https://img.shields.io/badge/arXiv-2602.11075-b31b1b.svg)](https://arxiv.org/abs/2602.11075) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://opendrivelab.com/kai0-rl/)

- **[arXiv'26.02] GigaBrain-0.5M\*** — *a VLA That Learns From World Model-Based Reinforcement Learning*  
   [![arXiv](https://img.shields.io/badge/arXiv-2602.12099-b31b1b.svg)](https://arxiv.org/abs/2602.12099) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/open-gigaai/giga-brain-0) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gigabrain05m.github.io/)

- **[arXiv'26.02] WoVR** — *WoVR: World Models as Reliable Simulators for Post-Training VLA Policies with RL*  
   [![arXiv](https://img.shields.io/badge/arXiv-2602.13977-b31b1b.svg)](https://arxiv.org/abs/2602.13977) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/RLinf/RLinf)

- **[arXiv'26.02] VLAW** — *VLAW: Iterative Co-Improvement of Vision-Language-Action Policy and World Model*  
   [![arXiv](https://img.shields.io/badge/arXiv-2602.12063-b31b1b.svg)](https://arxiv.org/abs/2602.12063) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sites.google.com/view/vlaw-arxiv)

- **[arXiv'26.02] World-VLA-Loop** — *World-VLA-Loop: Closed-Loop Learning of Video World Model and VLA Policy*  
   [![arXiv](https://img.shields.io/badge/arXiv-2602.06508-b31b1b.svg)](https://arxiv.org/abs/2602.06508) [![GitHub](https://img.shields.io/badge/GitHub-repo-181717.svg?logo=github)](https://github.com/showlab/World-VLA-Loop) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://showlab.github.io/World-VLA-Loop/)

---

### World Model for Policy Evaluation

- **[ICLR'26] WorldGym** — *WorldGym: World Model as An Environment for Policy Evaluation*  
   [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=hidBHy1CAw) [![arXiv](https://img.shields.io/badge/arXiv-2506.00613-b31b1b.svg)](https://arxiv.org/abs/2506.00613) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/world-model-eval/world-model-eval) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://world-model-eval.github.io/abstract)

- **[arXiv'25.05] WorldEval** — *WorldEval: World Model as Real-World Robot Policies Evaluator*  
   [![arXiv](https://img.shields.io/badge/arXiv-2505.19017-b31b1b.svg)](https://arxiv.org/abs/2505.19017) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/liyaxuanliyaxuan/Worldeval) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://worldeval.github.io/)

- **[arXiv'25.11] Scalable Policy Evaluation with Video World Models**  
   [![arXiv](https://img.shields.io/badge/arXiv-2511.11520-b31b1b.svg)](https://arxiv.org/abs/2511.11520) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://miscsubmission.github.io/world_model_policy_eval/)
---

<a id="world-models-for-gen"></a>
## World Model for Video Generation

> Video generation / video world models for robotics, including interactive simulators, imagination-based policy learning, and foundation video-world backbones that support robot learning.

- **[CoRL'24] Dreamitate** — *Dreamitate: Real-World Visuomotor Policy Learning via Video Generation*  
   [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=InT87E5sr4)

- **[ICML'24] RoboDreamer** — *RoboDreamer: Learning Compositional World Models for Robot Imagination*  
   [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v235/zhou24f.html)  [![arXiv](https://img.shields.io/badge/arXiv-2404.12377-b31b1b.svg)](https://arxiv.org/abs/2404.12377)    [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/UMass-Embodied-AGI/robodreamer)    [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robovideo.github.io/)

- **[ICLR'25] DreMa** — *Dream to Manipulate: Compositional World Models Empowering Robot Imitation Learning with Imagination*  
   [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=3RSLW9YSgk)    [![arXiv](https://img.shields.io/badge/arXiv-2410.04587-b31b1b.svg)](https://arxiv.org/abs/2410.04587)

- **[ICLR'25] CogVideoX** — *CogVideoX: Text-to-Video Diffusion Models with An Expert Transformer*  
   [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=LQzN6TRFg9)     [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/THUDM/CogVideo)

- **[CoRL'25] DreamGen** — *DreamGen: Unlocking Generalization in Robot Learning through Video World Models*  
   [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=3CnxNqmklv)  [![arXiv](https://img.shields.io/badge/arXiv-2505.12705-b31b1b.svg)](https://arxiv.org/abs/2505.12705)     [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dreamgen-robot.github.io/)

- **[ICCV'25] PhysWorld** — *PhysWorld: Robot Learning from a Physical World Model*  
   [![arXiv](https://img.shields.io/badge/arXiv-2505.09171-b31b1b.svg)](https://arxiv.org/abs/2505.09171)

- **[ICCV'25] IRASim** — *IRASim: A Fine-Grained World Model for Robot Manipulation*  
   [![Paper](https://img.shields.io/badge/Paper-CVF-4B5D67.svg)](https://openaccess.thecvf.com/content/ICCV2025/html/Zhu_IRASim_A_Fine-Grained_World_Model_for_Robot_Manipulation_ICCV_2025_paper.html)     [![arXiv](https://img.shields.io/badge/arXiv-2506.05034-b31b1b.svg)](https://arxiv.org/abs/2506.05034)    [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/bytedance/IRASim)    [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gen-irasim.github.io/)

- **[IROS'25] RoboEnvision** — *RoboEnvision: A Long-Horizon Video Generation Model for Multi-Task Robot Manipulation*  
   [![arXiv](https://img.shields.io/badge/arXiv-2507.18867-b31b1b.svg)](https://arxiv.org/abs/2507.18867)


- **[ICLR'26] RoboMaster** — *Learning Video Generation for Robotic Manipulation with Collaborative Trajectory Control*  
   [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=OeDwYtp8n1) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/KlingAIResearch/RoboMaster) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](http://fuxiao0719.github.io/projects/robomaster)


- **[ICLR'26] Vid2World** — *Vid2World: Crafting Video Diffusion Models to Interactive World Models*  
   [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=pFyzqbUiF9) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/thuml/Vid2World) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://knightnemo.github.io/vid2world/)

- **[ICLR'26] Genie Envisioner** — *Genie Envisioner: A Unified World Foundation Platform for Robotic Manipulation*  
   [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=fHLtSxDFKC)     [![arXiv](https://img.shields.io/badge/arXiv-2508.05635-b31b1b.svg)](https://arxiv.org/abs/2508.05635)  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/Genie-Envisioner)   [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://genie-envisioner.github.io/)

- **[ICLR'26] Ctrl-World** — *Ctrl-World: A Controllable Generative World Model for Robot Manipulation*  
   [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=748bHL2BAv)     [![arXiv](https://img.shields.io/badge/arXiv-2510.10125-b31b1b.svg)](https://arxiv.org/abs/2510.10125)     [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Robert-gyj/Ctrl-World)   [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://ctrl-world.github.io/)

- **[AAAI'26] Mask2IV** — *Mask2IV: Interaction-Centric Video Generation via Mask Trajectories*  
   [![arXiv](https://img.shields.io/badge/arXiv-2510.03135-b31b1b.svg)](https://arxiv.org/abs/2510.03135) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Reagan1311/Mask2IV)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://reagan1311.github.io/mask2iv/)


- **[arXiv'25.04] TesserAct** — *TesserAct*  
   [![arXiv](https://img.shields.io/badge/arXiv-2504.20995-b31b1b.svg)](https://arxiv.org/abs/2504.20995) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)]() [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://tesseractworld.github.io/) 

- **[arXiv'25.04] ManipDreamer** — *ManipDreamer: Boosting Robotic Manipulation World Model with Action Tree and Visual Guidance*  
   [![arXiv](https://img.shields.io/badge/arXiv-2504.10406-b31b1b.svg)](https://arxiv.org/abs/2504.10406) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)]()  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://myendless1.github.io/ManipDreamer/) 

- **[arXiv'25.05] EnerVerse-AC** — *EnerVerse-AC*  
   [![arXiv](https://img.shields.io/badge/arXiv-2505.09723-b31b1b.svg)](https://arxiv.org/abs/2505.09723) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/EnerVerse-AC) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://tesseractworld.github.io/) 

- **[arXiv'25.09] WoW** — *WoW: Towards a World-omniscient World-model Through Embodied Interaction*  
   [![arXiv](https://img.shields.io/badge/arXiv-2509.22642-b31b1b.svg)](https://arxiv.org/abs/2509.22642) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/wow-world-model/wow-world-model)

- **[Tech Release'25.09] UnifoLM-WMA-0** — *UnifoLM-WMA-0: A World-Model-Action Framework for General-Purpose Robot Learning*  
   [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/unitreerobotics/unifolm-world-model-action)     [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://unigen-x.github.io/unifolm-world-model-action.github.io/)

- **[Tech Report'25.10] Cosmos Predict 2.5** — *Cosmos-Predict2.5: A Suite of Diffusion-based World Foundation Models*  
   [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/nvidia-cosmos/cosmos-predict2.5)     [![Website](https://img.shields.io/badge/Website-NVIDIA-76B900.svg)](https://research.nvidia.com/labs/dir/cosmos-predict2.5/)


- **[arXiv'25.11] GigaWorld-0** — *GigaWorld-0*  
   [![arXiv](https://img.shields.io/badge/arXiv-2511.19861-b31b1b.svg)](https://arxiv.org/abs/2511.19861) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/EnerVerse-AC) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://giga-world-0.github.io/) 
  
- **[arXiv'26.01] RoboVIP** — *RoboVIP: Multi-View Video Generation with Visual Identity Prompting Augments Robot Manipulation*  
   [![arXiv](https://img.shields.io/badge/arXiv-2601.05241-b31b1b.svg)](https://arxiv.org/abs/2601.05241) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/RoboVIP/RoboVIP_VDM)   [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robovip.github.io/RoboVIP/) 

- **[arXiv'26.02] DreamDojo** — *DreamDojo: A Generalist Robot World Model from Large-Scale Human Videos*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.06949-b31b1b.svg)](https://arxiv.org/abs/2602.06949) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVIDIA/DreamDojo) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dreamdojo-world.github.io/)

<a id="benchmarks-for-evaluation-world-model"></a>
## Benchmarks for Evaluation World-Model

> Benchmarks / evaluation suites for embodied world models, video world models, and world simulators.  
> **Cross-listing is intentional**: if a work releases both a benchmark and a dataset, it can appear here **and** in [Datasets](#datasets).

- **[ICML'25] EVA-Bench** — *benchmark introduced in **Empowering World Models with Reflection for Embodied Video Prediction** (EVA)*  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v267/chi25b.html)  [![arXiv](https://img.shields.io/badge/arXiv-2410.15461-b31b1b.svg)](https://arxiv.org/abs/2410.15461)  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/litwellchi/EmbodiedVideoAnticipator)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sites.google.com/view/eva-public)

- **[ICML'25] WorldSimBench** — *WorldSimBench: Towards Video Generation Models as World Simulators*  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v267/qin25f.html)  [![arXiv](https://img.shields.io/badge/arXiv-2410.18072-b31b1b.svg)](https://arxiv.org/abs/2410.18072)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://iranqin.github.io/WorldSimBench.github.io/)

- **[BMVC'25] EWMBench** — *EWMBench: Evaluating Scene, Motion, and Semantic Quality in Embodied World Models*  
  [![Paper](https://img.shields.io/badge/Paper-BMVC-4B5D67.svg)](https://bmva-archive.org.uk/bmvc/2025/assets/papers/Paper_736/paper.pdf)  [![arXiv](https://img.shields.io/badge/arXiv-2505.09694-b31b1b.svg)](https://arxiv.org/abs/2505.09694)  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AgibotTech/EWMBench)

- **[CoRL'25] DreamGen Bench** — *benchmark introduced in **DreamGen: Unlocking Generalization in Robot Learning through Video World Models***  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v305/jang25a.html)  [![arXiv](https://img.shields.io/badge/arXiv-2505.12705-b31b1b.svg)](https://arxiv.org/abs/2505.12705)  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVIDIA/GR00T-Dreams)  [![Website](https://img.shields.io/badge/Website-NVIDIA-76B900.svg)](https://research.nvidia.com/labs/gear/dreamgen)

- **[ICLR'26] World-in-World (WoW!)** — *World-in-World: World Models in a Closed-Loop World*  
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=yDmb7xAfeb)  [![arXiv](https://img.shields.io/badge/arXiv-2510.18135-b31b1b.svg)](https://arxiv.org/abs/2510.18135)  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/World-In-World/world-in-world)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://world-in-world.github.io/)

- **[arXiv'26.01] WoW-World-Eval** — *Wow, wo, val! A Comprehensive Embodied World Model Evaluation Turing Test*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.04137-b31b1b.svg)](https://arxiv.org/abs/2601.04137)

- **[arXiv'26.01] RBench** — *Rethinking Video Generation Model for the Embodied World*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.15282-b31b1b.svg)](https://arxiv.org/abs/2601.15282)  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/DAGroup-PKU/ReVidgen)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dagroup-pku.github.io/ReVidgen.github.io/)

- **[arXiv'26.02] WorldArena** — *WorldArena: A Unified Benchmark for Evaluating Perception and Functional Utility of Embodied World Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.08971-b31b1b.svg)](https://arxiv.org/abs/2602.08971)  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/tsinghua-fib-lab/WorldArena)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://world-arena.ai)

---

<a id="datasets"></a>
## Datasets

> Training datasets, preference datasets, and instruction-tuning datasets.  
> **Cross-listing is intentional**: if a work releases both datasets and benchmarks, it may appear here **and** in [Benchmarks for Evaluation World-Model](#benchmarks-for-evaluation-world-model).

- **[ICRA'24] Open X-Embodiment (OXE)** — *Open X-Embodiment: Robotic Learning Datasets and RT-X Models*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://asu.elsevierpure.com/en/publications/open-x-embodiment-robotic-learning-datasets-and-rt-x-models-open-/)  [![arXiv](https://img.shields.io/badge/arXiv-2310.08864-b31b1b.svg)](https://arxiv.org/abs/2310.08864)  [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/google-deepmind/open_x_embodiment)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robotics-transformer-x.github.io/)

- **[RSS'24] DROID** — *DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://roboticsconference.org/2024/program/papers/120/)  [![arXiv](https://img.shields.io/badge/arXiv-2403.12945-b31b1b.svg)](https://arxiv.org/abs/2403.12945)  [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/droid-dataset/droid)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://droid-dataset.github.io/)

- **[ICML'25] EVA-Instruct** — *instruction-tuning dataset released with **Empowering World Models with Reflection for Embodied Video Prediction** (EVA)*  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v267/chi25b.html)  [![arXiv](https://img.shields.io/badge/arXiv-2410.15461-b31b1b.svg)](https://arxiv.org/abs/2410.15461)  [![GitHub](https://img.shields.io/badge/GitHub-code/data-181717.svg?logo=github)](https://github.com/litwellchi/EmbodiedVideoAnticipator)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sites.google.com/view/eva-public)

- **[ICML'25] HF-Embodied** — *human-preference dataset introduced in **WorldSimBench***  
  [![Paper](https://img.shields.io/badge/Paper-PMLR-4B5D67.svg)](https://proceedings.mlr.press/v267/qin25f.html)  [![arXiv](https://img.shields.io/badge/arXiv-2410.18072-b31b1b.svg)](https://arxiv.org/abs/2410.18072)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://iranqin.github.io/WorldSimBench.github.io/)

- **[IROS'25] AgiBot-World (Alpha/Beta)** — *AgiBot World Colosseo: A Large-scale Manipulation Platform for Scalable and Intelligent Embodied Systems*  
  [![arXiv](https://img.shields.io/badge/arXiv-2503.06669-b31b1b.svg)](https://arxiv.org/abs/2503.06669)  [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/OpenDriveLab/AgiBot-World)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://agibot-world.com/)

- **[arXiv'25.09] Galaxea Open-World Dataset** — *Galaxea Open-World Dataset and G0 Dual-System VLA Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2509.00576-b31b1b.svg)](https://arxiv.org/abs/2509.00576)  [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/OpenGalaxea/GalaxeaVLA)  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://opengalaxea.github.io/G0/)

- **[arXiv'26.01] Action100M** — *Action100M: A Large-scale Video Action Dataset*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.10592-b31b1b.svg)](https://arxiv.org/abs/2601.10592)  [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/facebookresearch/Action100M)  
- **[arXiv'26.01] RoVid-X** — *training dataset released with **Rethinking Video Generation Model for the Embodied World***  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.15282-b31b1b.svg)](https://arxiv.org/abs/2601.15282)  [![GitHub](https://img.shields.io/badge/GitHub-data-181717.svg?logo=github)](https://github.com/DAGroup-PKU/ReVidgen)   [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dagroup-pku.github.io/ReVidgen.github.io/)


  
