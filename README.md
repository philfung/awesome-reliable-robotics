# Awesome Reliable Robotics 🤖
[![Contributions](https://img.shields.io/badge/contributions-welcome-blue)](https://github.com/philfung/awesome-reliable-robotics/graphs/contributors)
[![Contributors](https://img.shields.io/github/contributors/philfung/awesome-reliable-robotics)](https://github.com/philfung/awesome-reliable-robotics/graphs/contributors)
[![Last Commit](https://img.shields.io/github/last-commit/philfung/awesome-reliable-robotics)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A collection of robotics research papers that demonstrate reliability and robustness in the real world. 

Prerequisites:
- must include real-world results

Common themes include:

- Reward learning from human feedback and interventions

- Value and progress estimation

Contributions are welcome!

---

## High Success Rate w/ Online Fine Tuning

| **Name** | **Date** | **Real World Success Rate** |**Project** | **Paper** | **Code** |  **Organization(s)** | **Notes** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Dual-Actor Fine-Tuning of VLA Models: A Talk-and-Tweak Human-in-the-Loop Approach | 09/2025 | **100%**  success across three tasks within 101 minutes of online fine-tuning. For long-horizon tasks, it sustains a **50%** success rate over 12 consecutive operations.<br><img alt="WSRL" src="https://github.com/user-attachments/assets/2229db75-8bb7-47b4-b761-7c508cd7cd25" />| <a href="https://sites.google.com/view/hil-daft/" target="_blank">Link</a> | <a href="https://arxiv.org/pdf/2509.13774" target="_blank">Link</a> | | Zhejiang & others |  no code : (
| WSRL: Efficient Online Reinforcement Learning Fine-Tuning Need Not Retain Offline Data | 07/2025 | **100%** success rate on Franka peg insertion task in 18 minutes, SERL fails (0/20) even with 50 minutes.<br><img alt="WSRL" src="https://github.com/user-attachments/assets/22bb0185-84e8-49cf-82d8-a1bdcdbb7dfc" />| <a href="https://zhouzypaul.github.io/wsrl/" target="_blank">Link</a> | <a href="https://arxiv.org/pdf/2412.07762" target="_blank">Link</a> | <a href="https://github.com/zhouzypaul/wsrl" target="_blank">Link</a> | UC Berkeley |  Overall idea: <img src="https://github.com/user-attachments/assets/defd1384-d7ce-4742-b9cc-6bc662d09139" /> No data retention during fine-tuning, warmup phase with small rollouts from pre-trained policy.  Unfortunately, only 1 real world experiment, all others in sim.
| Dyna Robotics (Unknown Model) | 07/2025 | **99.9%** success rate in folding towels for 8 hours/day over 3 days (dropped 1 towel on day 2).  No intervention.  |  <a href="https://x.com/DynaRobotics/status/1940443709621109186" target="_blank">Link</a> | | | Dyna Robotics | |
| Figure (Helix) | 06/2025 | **~95%** accuracy at correctly orienting barcodes. **4.05** seconds per package. |  <a href="https://www.figure.ai/news/scaling-helix-logistics" target="_blank">Link</a> | | | Figure | Adds memory for more robust, long-term tasks and force feedback for improved grip.
| RSS 2025 Workshop: Human-in-the-Loop Robot Learning: Teaching, Correcting, and Adapting | 06/2025 | various results | <a href="https://hitl-robot-learning.github.io/" target="_blank">Link</a> |  |  | various universities | 
| Compliant Residual DAgger: Improving Real-World Contact-Rich Manipulation with Human Corrections | 06/2025 | book-flipping success rate of **100%** (**60%** improvement) and belt assembly success of **70%** (**50%** improvement) <br><img src="https://github.com/user-attachments/assets/c9f31853-a699-4eb9-acd2-78720fe672d8" />| <a href="https://compliant-residual-dagger.github.io/" target="_blank">Link</a> | <a href="https://arxiv.org/abs/2506.16685" target="_blank">Link</a> |  | Stanford | 
| ReWiND: Language-Guided Rewards Teach Robot Policies without New Demonstrations | 05/2025 | an hour of real-world RL improves success rate from 12% to 68%, vs 8% to 10% with VLC <br><img alt="WSRL" src="https://github.com/user-attachments/assets/0e762d11-0546-4844-8928-bb607bd49683" /> | <a href="https://rewind-reward.github.io/" target="_blank">Link</a> | <a href="https://arxiv.org/abs/2505.10911" target="_blank">Link</a> | <a href="https://github.com/rewind-reward/ReWiND" target="_blank">Link</a> | U Wash | 
| Dyna Robotics DYNA-1 Model | 04/2025 | **99.4%** success rate in folding napkins over 24 hours. No intervention. &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; |  <a href="https://www.dyna.co/research)" target="_blank">Link</a> | | | Dyna Robotics | |
| ConRFT: A Reinforced Fine-tuning Method for VLA Models via Consistency Policy | 02/2025 | **96.3%** avg success rate across tasks, compared to 31.9% w/ HIL-SERL <img alt="ConRFT" src="https://github.com/user-attachments/assets/15ddc8ba-59a6-448b-91db-3fefb212e8f7" /> | | <a href="https://arxiv.org/pdf/2502.05450" target="_blank">Link</a> | <a href="https://github.com/cccedric/conrft" target="_blank">Link</a> | Chinese Academy of Sciences | Online and offline fine-tuning. |
| HIL-SERL: Precise and Dexterous Robotic Manipulation via Human-in-the-Loop Reinforcement Learning | 10/2024 | **100%** success rate on a variety of tasks <img alt="HIL-SERL" src="https://github.com/user-attachments/assets/56f35ef2-e297-4fd7-a4e0-362bf441c670" />  | <a href="https://hil-serl.github.io/" target="_blank">Link</a> | <a href="https://hil-serl.github.io/static/hil-serl-paper.pdf" target="_blank">Link</a> | <a href="https://github.com/rail-berkeley/hil-serl" target="_blank">Link</a> | UC Berkeley | Online fine-tuning, human intervention allowed.  Implementation available in LeRobot. |
| RLIF: INTERACTIVE IMITATION LEARNING AS REINFORCEMENT LEARNING | 03/2024 | * **95%** success rate in cloth unfolding within 7 rounds * **100%** rate success in peg insertion within 6 rounds <img alt="RLIF" src="https://github.com/user-attachments/assets/f101b109-e813-4deb-99b1-99f2e070e007" /> | <a href="https://rlif-page.github.io/" target="_blank">Link</a> | <a href="https://arxiv.org/pdf/2311.12996" target="_blank">Link</a> | <a href="https://github.com/pd-perry/RLIF" target="_blank">Link</a> | UC Berkeley |  |
| SERL: A Software Suite for Sample-Efficient Robotic Reinforcement Learning | 01/2024 | **100%** success on PCB insertion, cable routing, object relocation <img src="https://github.com/user-attachments/assets/ce22ae75-259b-43b6-a000-d6d5f88f3875" />  | <a href="https://serl-robot.github.io/" target="_blank">Link</a> | <a href="https://arxiv.org/abs/2401.16013" target="_blank">Link</a> | <a href="https://github.com/rail-berkeley/serl" target="_blank">Link</a> | UC Berkeley | |

