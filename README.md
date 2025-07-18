# Awesome Reliable Robotics 🤖
[![Contributions](https://img.shields.io/badge/contributions-welcome-blue)](https://github.com/philfung/awesome-reliable-robotics/graphs/contributors)
[![Contributors](https://img.shields.io/github/contributors/philfung/awesome-reliable-robotics)](https://github.com/philfung/awesome-reliable-robotics/graphs/contributors)
[![Last Commit](https://img.shields.io/github/last-commit/philfung/awesome-reliable-robotics)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A collection of robotics research papers that demonstrate reliability and robustness in the real world. 

Prerequisites:
- must include real-world results
- preference on research accompanied by code

Common themes include:

- Reward learning from human feedback and interventions

- Value and progress estimation

Contributions are welcome!

---

## High Success Rate w/ Fine Tuning


| **Name** | **Date** | **Real World Success Rate** |**Project** | **Paper** | **Code** |  **Organization(s)** | **Notes** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| WSRL: Efficient Online Reinforcement Learning Fine-Tuning Need Not Retain Offline Data | 07/2025 | **100%** success rate on Franka peg insertion task in 18 minutes, SERL fails (0/20) even with 50 minutes.<br><img alt="WSRL" src="https://github.com/user-attachments/assets/22bb0185-84e8-49cf-82d8-a1bdcdbb7dfc" />| <a href="https://zhouzypaul.github.io/wsrl/" target="_blank">Link</a> | <a href="https://arxiv.org/pdf/2412.07762" target="_blank">Link</a> | <a href="https://github.com/zhouzypaul/wsrl" target="_blank">Link</a> | UC Berkeley |  Overall idea: <img src="https://github.com/user-attachments/assets/defd1384-d7ce-4742-b9cc-6bc662d09139" /> No data retention during fine-tuning, warmup phase with small rollouts from pre-trained policy.  Unfortunately, only 1 real world experiment, all others in sim.
| Dyna Robotics (Unknown Model) | 07/2025 | **99.9%** success rate in folding towels for 8 hours/day over 3 days (dropped 1 towel on day 2).  No intervention.  |  <a href="https://x.com/DynaRobotics/status/1940443709621109186" target="_blank">Link</a> | | | Dyna Robotics | |
| Figure (Helix) | 06/2025 | **~95%** accuracy at correctly orienting barcodes. **4.05** seconds per package. |  <a href="https://www.figure.ai/news/scaling-helix-logistics" target="_blank">Link</a> | | | Figure | Adds memory for more robust, long-term tasks and force feedback for improved grip.
| RSS 2025 Workshop: Human-in-the-Loop Robot Learning: Teaching, Correcting, and Adapting | 06/2025 | various results | <a href="https://hitl-robot-learning.github.io/" target="_blank">Link</a> |  |  | various universities | 
| Compliant Residual DAgger: Improving Real-World Contact-Rich Manipulation with Human Corrections | 06/2025 | book-flipping success rate of **100%** (**60%** improvement) and belt assembly success of **70%** (**50%** improvement) <br><img src="https://github.com/user-attachments/assets/c9f31853-a699-4eb9-acd2-78720fe672d8" />| <a href="https://compliant-residual-dagger.github.io/" target="_blank">Link</a> | <a href="https://arxiv.org/abs/2506.16685" target="_blank">Link</a> |  | Stanford | 
| Dyna Robotics DYNA-1 Model | 04/2025 | **99.4%** success rate in folding napkins over 24 hours. No intervention. &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; |  <a href="https://www.dyna.co/research)" target="_blank">Link</a> | | | Dyna Robotics | |
| ConRFT: A Reinforced Fine-tuning Method for VLA Models via Consistency Policy | 02/2025 | **96.3%** avg success rate across tasks, compared to 31.9% w/ HIL-SERL <img alt="ConRFT" src="https://github.com/user-attachments/assets/15ddc8ba-59a6-448b-91db-3fefb212e8f7" /> | | <a href="https://arxiv.org/pdf/2502.05450" target="_blank">Link</a> | <a href="https://github.com/cccedric/conrft" target="_blank">Link</a> | Chinese Academy of Sciences | Online and offline fine-tuning. |
| HIL-SERL: Precise and Dexterous Robotic Manipulation via Human-in-the-Loop Reinforcement Learning | 10/2024 | **100%** success rate on a variety of tasks <img alt="HIL-SERL" src="https://github.com/user-attachments/assets/56f35ef2-e297-4fd7-a4e0-362bf441c670" />  | <a href="https://hil-serl.github.io/" target="_blank">Link</a> | <a href="https://hil-serl.github.io/static/hil-serl-paper.pdf" target="_blank">Link</a> | <a href="https://github.com/rail-berkeley/hil-serl" target="_blank">Link</a> | UC Berkeley | Online fine-tuning, human intervention allowed.  Implementation available in LeRobot. |
| RLIF: INTERACTIVE IMITATION LEARNING AS REINFORCEMENT LEARNING | 03/2024 | * **95%** success rate in cloth unfolding within 7 rounds * **100%** rate success in peg insertion within 6 rounds <img alt="RLIF" src="https://github.com/user-attachments/assets/f101b109-e813-4deb-99b1-99f2e070e007" /> | <a href="https://rlif-page.github.io/" target="_blank">Link</a> | <a href="https://arxiv.org/pdf/2311.12996" target="_blank">Link</a> | <a href="https://github.com/pd-perry/RLIF" target="_blank">Link</a> | UC Berkeley |  |
| SERL: A Software Suite for Sample-Efficient Robotic Reinforcement Learning | 01/2024 | **100%** success on PCB insertion, cable routing, object relocation <img src="https://github.com/user-attachments/assets/ce22ae75-259b-43b6-a000-d6d5f88f3875" />  | <a href="https://serl-robot.github.io/" target="_blank">Link</a> | <a href="https://arxiv.org/abs/2401.16013" target="_blank">Link</a> | <a href="https://github.com/rail-berkeley/serl" target="_blank">Link</a> | UC Berkeley | |

## Unseen Tasks

| **Name** | **Date** | **Real World Success Rate** |**Project** | **Paper** | **Code** |  **Organization(s)** | **Notes** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ReWiND: Language-Guided Rewards Teach Robot Policies without New Demonstrations | 05/2025 | **50% - 100%** success rate on new tasks, **~5x** improvement over baseline &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img alt="ReWIND" src="https://github.com/user-attachments/assets/ff5250b7-cbca-4747-aab2-7dcf257ce08b" />|  <a href="https://rewind-reward.github.io/" target="_blank">Link</a> |  <a href="https://arxiv.org/abs/2505.10911" target="_blank">Link</a> |  | USC, Amazon, KAIST | Focussed on new tasks. |
| Opening Articulated Structures in the Real World | 05/2025 | **61%** success rate across 13 real-world homes and offices on previously unseen cabinets and drawers | [Link](https://arjung128.github.io/opening-articulated-structures/) | [Link](https://arxiv.org/abs/2402.17767) | [Link](https://github.com/arjung128/stretch-open) | UIUC | General mobile manipulation system with no environment-specific tuning. |
| RDT-1B: a Diffusion Foundation Model for Bimanual Manipulation | 03/2025 | **87.5% - 100%** success rate on unseen tasks, **56%** _improvement_ in success rates across tasks over baseline (ACT, VLA, Octo) <img alt="RDT-1B" src="https://github.com/user-attachments/assets/aa8bbc19-f4d1-4006-aea3-65e34b30fd1b" />| <a href="https://rdt-robotics.github.io/rdt-robotics/" target="_blank">Link</a> |  <a href="https://arxiv.org/pdf/2410.07864" target="_blank">Link</a> | <a href="https://github.com/thu-ml/RoboticsDiffusionTransformer" target="_blank">Link</a> | Tsinghua | Focussed on new tasks.  Human-level inference/robot speed. |
| GVL: Vision Language Models are In-Context Value Learner | 11/2024 | **15% - 90%** success rate, **0.46** avg _improvement_ (VOC) on scale -1.0 to 1.0 over DP (diffusion policy)<img alt="GVL" src="https://github.com/user-attachments/assets/21541e78-91fd-478e-9de0-d491d3da8e44" />  | <a href="https://generative-value-learning.github.io/" target="_blank">Link</a> | <a href="https://arxiv.org/pdf/2411.04549" target="_blank">Link</a> |  | Deepmind, UPenn, Stanford | Focussed on new tasks and estimation using VLM.  |

