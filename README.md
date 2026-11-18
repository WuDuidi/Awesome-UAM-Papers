# Awesome UAM Papers

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated reading list for **UAM — Unmanned Aerial Manipulators** (multirotor UAV + robot arm): platform design & morphology, whole-body control, disturbance rejection, contact-rich interaction, learning-based methods, and multi-robot cooperation for aerial manipulation.

🔖 Last updated: Nov 2026 · ✦ marks papers from renowned teams · Contributions welcome via PR!

---

## 📑 Contents

- [Getting Started](#getting-started)
  - [Surveys & Reviews](#surveys)
  - [Nature & Science Family](#nature-science)
  - [IEEE T-RO Selection](#tro)
  - [Classic Foundations](#foundations)
- [Platforms & Morphology](#platforms)
  - [Bio-Inspired UAM](#bio-inspired)
  - [Fully-Actuated & Omnidirectional Platforms](#fully-actuated)
  - [Morphing & Reconfigurable UAV/UAM](#morphing)
- [Control](#control)
  - [Whole-Body Control & Loco-Manipulation](#wbc)
  - [Disturbance Compensation & Estimation](#disturbance)
  - [Contact & Force Interaction](#contact-force)
- [Learning-Based Methods](#learning)
  - [Simulators & Benchmarks](#simulators)
  - [RL & Learned Policies](#rl)
- [Multi-Robot Cooperation](#multi-robot)
  - [Multi-UAM Cooperative Manipulation](#multi-uam)
  - [Multi-UAV Cooperative Transport](#transport)
- [Applications](#applications)
  - [Tool Use & Field Operations](#tools)
  - [Aerial Construction & Heterogeneous Teams](#construction)

---

## <a id="getting-started"></a>Getting Started

### <a id="surveys"></a>Surveys & Reviews

- [2026] **From Aerial Transportation to Aerial Interaction: A Review** · *Chinese Journal of Aeronautics* [paper](https://www.sciencedirect.com/science/article/pii/S1000936126003808) (Nanjing University of Aeronautics and Astronautics)
- [2024] ⭐ **A Review of Real-Time Implementable Cooperative Aerial Manipulation** · *Drones (MDPI)* [paper](https://www.mdpi.com/2504-446x/8/5/196) [pdf](https://arxiv.org/pdf/2403.14347) (National Technical University of Athens, University of Denver)
- [2022] ⭐ **Past, Present, and Future of Aerial Robotic Manipulators** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/9462539) [pdf](https://idus.us.es/bitstreams/954638e3-7b65-4817-889e-a476317572a0/download) (University of Seville, CNRS-LAAS, University of Twente, Seoul National University) ✦ *Aníbal Ollero*
- [2018] **Aerial Manipulation: A Literature Review** · *IEEE RA-L* [paper](https://ieeexplore.ieee.org/document/8506571) (University of Naples Federico II, University of Seville)
- [2018] **Aerial Manipulation — A Literature Survey** · *Journal of Intelligent & Robotic Systems* [paper](https://link.springer.com/article/10.1007/s10846-018-0875-3) (Toronto Metropolitan University)

### <a id="nature-science"></a>Nature & Science Family

- [2025] ⭐ **Proximal Cooperative Aerial Manipulation with Vertically Stacked Drones** · *Nature* [paper](https://www.nature.com/articles/s41586-025-09575-x) [pdf](https://ndownloader.figshare.com/files/58224982) (Westlake University, Lancaster University) ✦ *Shiyu Zhao*
- [2025] **Agile and Cooperative Aerial Manipulation of a Cable-Suspended Load** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.adu8015) [pdf](https://arxiv.org/pdf/2501.18802) (TU Delft, Sapienza University of Rome, University of Twente) ✦ *Javier Alonso-Mora*
- [2025] **Learning Vision-Based Agile Flight via Differentiable Physics** · *Nature Machine Intelligence* [paper](https://www.nature.com/articles/s42256-025-01048-0) [pdf](https://arxiv.org/pdf/2407.10648) (Shanghai Jiao Tong University)
- [2023] ⭐ **Champion-Level Drone Racing Using Deep Reinforcement Learning (Swift)** · *Nature* [paper](https://www.nature.com/articles/s41586-023-06419-9) (University of Zurich) ✦ *Davide Scaramuzza*
- [2022] ⭐ **Aerial Additive Manufacturing with Multiple Autonomous Robots** · *Nature* [paper](https://www.nature.com/articles/s41586-022-04988-4) (Imperial College London, Empa) ✦ *Mirko Kovac*
- [2022] **Swarm of Micro Flying Robots in the Wild** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.abm5954) [pdf](https://zhepeiwang.github.io/pubs/sr_2022_swarm.pdf) [code](https://github.com/ZJU-FAST-Lab/EGO-Planner-v2) (Zhejiang University) ✦ *Fei Gao, Boyu Zhou*
- [2021] **Learning High-Speed Flight in the Wild** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.abg5810) [pdf](https://rpg.ifi.uzh.ch/docs/Loquercio21_Science.pdf) (University of Zurich) ✦ *Davide Scaramuzza*
- [2021] **Bird-Inspired Dynamic Grasping and Perching in Arboreal Environments (SNAG)** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.abj7562) [pdf](https://lentinklab.com/wp-content/uploads/2023/12/2021-bird-inspired-perching.pdf) (Stanford University) ✦ *David Lentink*
- [2021] **Predictive Control of Aerial Swarms in Cluttered Environments** · *Nature Machine Intelligence* [paper](https://www.nature.com/articles/s42256-021-00341-y) (EPFL) ✦ *Dario Floreano*
- [2020] **Soft Biohybrid Morphing Wings with Feathers Underactuated by Wrist and Finger Actuation (PigeonBot)** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.aay1246) [project](https://www.erchang.org/pigeonbot) (Stanford University) ✦ *David Lentink*
- [2019] **Untethered Flight of an Insect-Sized Flapping-Wing Microscale Aerial Vehicle (RoboBee X-Wing)** · *Nature* [paper](https://www.nature.com/articles/s41586-019-1322-0) (Harvard University) ✦ *Robert Wood*
- [2017] **A Biomimetic Robotic Platform to Study Flight Specializations of Bats (Bat Bot B2)** · *Science Robotics* [paper](https://pubmed.ncbi.nlm.nih.gov/33157861) [pdf](https://faculty.cc.gatech.edu/~seth/ResPages/pdfs/ScienceRobotics2017.pdf) (Caltech, UIUC) ✦ *Soon-Jo Chung*

### <a id="tro"></a>IEEE T-RO Selection

- [2025] **Whole-Body Integrated Motion Planning for Aerial Manipulators (AM-Planner)** · *IEEE T-RO* [paper](https://arxiv.org/abs/2501.06493) [code](https://github.com/SYSU-HILAB/am-planner) (Sun Yat-sen University) — *first whole-body (base + arm) integrated planner for aerial manipulators*
- [2022] ⭐ **Past, Present, and Future of Aerial Robotic Manipulators** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/9462539) [pdf](https://idus.us.es/bitstreams/954638e3-7b65-4817-889e-a476317572a0/download) (University of Seville, CNRS-LAAS, University of Twente, Seoul National University) ✦ *Aníbal Ollero*
- [2021] ⭐ **Active Interaction Force Control for Contact-Based Inspection with a Fully Actuated Aerial Vehicle** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/9295362) [pdf](https://arxiv.org/pdf/2003.09516v3) (ETH Zurich) ✦ *Roland Siegwart*
- [2018] **A Novel Robotic Platform for Aerial Manipulation Using Quadrotors as Rotating Thrust Generators** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/8294249) (Seoul National University) ✦ *Dongjun Lee* — *quadrotors spin around a jointed arm to generate joint torques*
- [2013] ⭐ **Geometric Control of a Quadrotor with a Cable-Suspended Load** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2013.2271569) [pdf](https://hybrid-robotics.berkeley.edu/publications/CDC2013.pdf) (University of Pennsylvania) ✦ *Vijay Kumar*

### <a id="foundations"></a>Classic Foundations

- [2022] **A Benchmark Comparison of Learned Control Policies for Agile Quadrotor Flight (CTBR)** · *ICRA* [paper](https://arxiv.org/abs/2202.10796) [pdf](https://arxiv.org/pdf/2202.10796) (University of Zurich) ✦ *Davide Scaramuzza* — *collective-thrust & body-rate (CTBR) 
- [2018] **Design of a Lightweight Dual Arm System for Aerial Manipulation** · *Bioinspiration & Biomimetics* [paper](https://doi.org/10.1088/1748-3190/aa9d51) [pdf](https://idus.us.es/bitstreams/8aa25e92-ae25-4a04-8f29-8735f5232399/download) (University of Seville)
- [2018] **An Anthropomorphic, Compliant, and Lightweight Dual Arm for Aerial Manipulation** · *IEEE Access* [paper](https://ieeexplore.ieee.org/document/8354886) [pdf](https://idus.us.es/bitstream/11441/87747/1/IEEEA_Suarez_2018_Design.pdf) (University of Seville)
- [2014] **Aerial Manipulation Robot Composed of an Autonomous Helicopter and a 7-DOF Industrial Manipulator** · *ICRA* [paper](https://doi.org/10.1109/ICRA.2014.6907148) (DLR — German Aerospace Center)
- [2012] **Cartesian Impedance Control of a UAV with a Robotic Arm** · *SYROCO* [pdf](https://www.fedoa.unina.it/9621/1/SYROCO12_0158_MS.pdf) (University of Naples Federico II)
- [2012] **Impedance Control of an Aerial Manipulator** · *ACC* [paper](https://ieeexplore.ieee.org/document/6425020) (University of Bologna) ✦ *Lorenzo Marconi*
- [2011] ⭐ **Grasping from the Air: Hovering Capture and Load Stability** · *ICRA* [paper](https://www.eng.yale.edu/grablab/pubs/Pounds_ICRA2011.pdf) (Yale University) ✦ *Aaron Dollar*

---

## <a id="platforms"></a>Platforms & Morphology

### <a id="bio-inspired"></a>Bio-Inspired UAM

*Each entry notes the biological model and the borrowed idea.*

- [2021] ⭐ **Bird-Inspired Dynamic Grasping and Perching in Arboreal Environments (SNAG)** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.abj7562) [pdf](https://lentinklab.com/wp-content/uploads/2023/12/2021-bird-inspired-perching.pdf) (Stanford University) ✦ *David Lentink* — 🐦 *model: peregrine-falcon / parrotlet legs & tendons; idea: stereotyped 50-ms snatch-and-grasp reflex + tendon lock for a 3D-printed perching gripper*
- [2020] **PigeonBot — Soft Biohybrid Morphing Wings with Feathers** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.aay1246) [project](https://www.erchang.org/pigeonbot) (Stanford University) ✦ *David Lentink* — 🕊️ *model: pigeon wing; idea: 40 real feathers passively deployed by elastic skin driven by only 4 wrist/finger servos → underactuated biohybrid morphing wing*
- [2019] **RoboBee X-Wing — Untethered Insect-Sized Flapping Flight** · *Nature* [paper](https://www.nature.com/articles/s41586-019-1322-0) (Harvard University) ✦ *Robert Wood* — 🐝 *model: insect (bee-scale) flapping flight; idea: two piezo-actuated drivers flapping four wings at 200 Hz, solar-powered untethered 259-mg flight*
- [2017] **Bat Bot B2 — A Biomimetic Robotic Bat** · *Science Robotics* [paper](https://pubmed.ncbi.nlm.nih.gov/33157861) [pdf](https://faculty.cc.gatech.edu/~seth/ResPages/pdfs/ScienceRobotics2017.pdf) (Caltech, UIUC) ✦ *Soon-Jo Chung* — 🦇 *model: bat wing; idea: 5 actuated joints per wing with stretchable silicone membrane replicating asymmetric fold-flap upstroke*

### <a id="fully-actuated"></a>Fully-Actuated & Omnidirectional Platforms

- [2020] **Fully-Actuated Aerial Manipulator for Infrastructure Contact Inspection: Design, Modeling, Localization, and Control** · *IEEE TASE* [paper](https://ieeexplore.ieee.org/document/9114869) [pdf](https://idus.us.es/items/4338b496-9292-4a71-8462-c0cbfa414528) (University of Seville, University of Luxembourg)
- [2019] ⭐ **An Omnidirectional Aerial Manipulation Platform for Robust Interaction with Unstructured Environments** · *RSS* [paper](https://www.roboticsproceedings.org/rss15/p19.pdf) (ETH Zurich) ✦ *Roland Siegwart*
- [2018] **ODAR: Aerial Manipulation Platform Enabling Omnidirectional Wrench Generation** · *IEEE/ASME Trans. Mechatronics* [paper](https://ieeexplore.ieee.org/document/8401328) (Seoul National University) ✦ *Dongjun Lee (co-author)*
- [2017] **6D Physical Interaction with a Fully Actuated Aerial Robot** · *ICRA* [pdf](https://laas.hal.science/hal-01476814v1/document) (MPI for Biological Cybernetics, University of Cassino, CNRS-LAAS) ✦ *Antonio Franchi*
- [2016] **Modeling and Control of FAST-Hex: A Fully-Actuated and Tiltable Hexarotor** · *IROS* [paper](https://ieeexplore.ieee.org/document/7759271) [pdf](https://hal.science/hal-01348538v1/document) (MPI for Biological Cybernetics, University of Twente, CNRS-LAAS) ✦ *Antonio Franchi*
- [2015] **Modeling, Control and Design Optimization for a Fully-Actuated Hexarotor** · *ICRA* [pdf](https://hal.science/hal-01134829v1/document) (MPI for Biological Cybernetics, University of Twente) ✦ *Antonio Franchi, Heinrich Bülthoff*

### <a id="morphing"></a>Morphing & Reconfigurable UAV/UAM

*Each entry notes the morphing / reconfiguration mechanism.*

- [2020] **PigeonBot — Biohybrid Feathered Morphing Wing** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.aay1246) [project](https://www.erchang.org/pigeonbot) (Stanford University) ✦ *David Lentink* — 🪶 *mechanism: passive feather deployment via elastic skin, wing area/shape morphs with only wrist & finger actuation*
- [2019] **DRAGON — A Dual-Rotor-Embedded Multilink Robot with Multi-DoF Aerial Transformation** · *IEEE RA-L* [paper](https://ieeexplore.ieee.org/document/8258850) [project](https://www.dragon.t.u-tokyo.ac.jp/publications/references/2018-ral-dragon-zhao) (University of Tokyo) ✦ *Moju Zhao (JSK Lab)* — 🐉 *mechanism: snake-like chain of 2-DoF links, each with a vectorable dual-rotor unit; transforms its whole shape mid-flight (line→L→S) to slalom through gaps, later extended into a flying manipulator*
- [2019] **A Quadrotor with an Origami-Inspired Protective Mechanism** · *IEEE RA-L* [paper](https://arxiv.org/abs/1907.07056) (City University of Hong Kong) — 🗂️ *mechanism: passive origami foldable airframe/cage that buckles to absorb collision impact and self-restores in flight*
- [2016] **FAST-Hex — A Fully-Actuated and Tiltable Hexarotor** · *IROS* [paper](https://ieeexplore.ieee.org/document/7759271) [pdf](https://hal.science/hal-01348538v1/document) (MPI for Biological Cybernetics, University of Twente, CNRS-LAAS) ✦ *Antonio Franchi* — 🔧 *mechanism: one central servo tilts all six arms together, switching between underactuated and fully-actuated flight in mid-air*

---

## <a id="control"></a>Control

### <a id="wbc"></a>Whole-Body Control & Loco-Manipulation

- [2026] **Aerial Manipulation in the Wild with Onboard Perception, Policy Learning, and Whole-Body Control** · *arXiv* [paper](https://arxiv.org/abs/2609.30521) (The Chinese University of Hong Kong) — *visuomotor diffusion policy on top of a WBC with onboard LiDAR-inertial state estimation; outdoor, no motion capture*
- [2026] **Global End-Effector Pose Control of an Underactuated Aerial Manipulator via Reinforcement Learning** · *ICRA* [paper](https://arxiv.org/abs/2512.21085) [pdf](https://arxiv.org/pdf/2512.21085) (TU Delft) — *RL whole-body coordination of quadrotor + 2-DoF arm for full 6-DoF end-effector pose, incl. pushing and heavy loads*
- [2025] **Flying Hand: End-Effector-Centric Framework for Versatile Aerial Manipulation** · *RSS* [paper](https://www.roboticsproceedings.org/rss21/p130.pdf) [pdf](https://arxiv.org/abs/2504.10334) (CMU)
- [2025] **Whole-Body Integrated Motion Planning for Aerial Manipulators (AM-Planner)** · *IEEE T-RO* [paper](https://arxiv.org/abs/2501.06493) [code](https://github.com/SYSU-HILAB/am-planner) (Sun Yat-sen University) — *joint base+arm waypoint optimization for versatile aerial tasks*
- [2023] **Hierarchical Whole-Body Control of the Cable-Suspended Aerial Manipulator with Winch-Based Actuation** · *arXiv* [paper](https://arxiv.org/abs/2305.16466) (Korea University, DLR) — *hierarchical WBC for the winch-actuated cable-suspended manipulator (SAM lineage)*
- [2012] **Cartesian Impedance Control of a UAV with a Robotic Arm** · *SYROCO* [pdf](https://www.fedoa.unina.it/9621/1/SYROCO12_0158_MS.pdf) (University of Naples Federico II) — *foundational coupled base-arm Cartesian impedance*

### <a id="disturbance"></a>Disturbance Compensation & Estimation

*Wind, downwash, contact interaction, and arm-motion reaction — estimation and rejection.*

- [2025] ⭐ **Proximal Cooperative Aerial Manipulation with Vertically Stacked Drones** · *Nature* [paper](https://www.nature.com/articles/s41586-025-09575-x) [pdf](https://ndownloader.figshare.com/files/58224982) (Westlake University, Lancaster University) ✦ *Shiyu Zhao* — *explicit downwash modeling and compensation between stacked vehicles*
- [2025] **Predictive Admittance Control for Aerial Physical Interaction** · *IEEE RA-L* [paper](https://ieeexplore.ieee.org/document/11155162) [pdf](https://ayhamalharbat.github.io/publication/2025-4-ral/2025-4-RAL.pdf) (University of Twente) ✦ *Antonio Franchi* — *model-based prediction to hold the desired impedance through contact/free-flight transitions*
- [2024] **Robust Control of an Aerial Manipulator Based on a Variable Inertia Parameters Model** · *arXiv* [paper](https://arxiv.org/abs/2401.04316) (Shenyang Institute of Automation, CAS; Toronto Metropolitan University) — *arm-induced variable inertia explicitly modeled and compensated*
- [2021] **Active Interaction Force Control for Contact-Based Inspection with a Fully Actuated Aerial Vehicle** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/9295362) [pdf](https://arxiv.org/pdf/2003.09516v3) (ETH Zurich) ✦ *Roland Siegwart* — *maintains desired contact force while rejecting interaction disturbances*
- [2009] **Wind Disturbance Estimation and Rejection for Quadrotor Position Control** · *AIAA Infotech@Aerospace* [paper](https://www.researchgate.net/publication/260122517_Wind_Disturbance_Estimation_and_Rejection_for_Quadrotor_Position_Control) (Stanford University) — *classic: wind-drag modeling + integral sliding-mode rejection on STARMAC*

### <a id="contact-force"></a>Contact & Force Interaction

- [2025] **Predictive Admittance Control for Aerial Physical Interaction** · *IEEE RA-L* [paper](https://ieeexplore.ieee.org/document/11155162) [pdf](https://ayhamalharbat.github.io/publication/2025-4-ral/2025-4-RAL.pdf) (University of Twente) ✦ *Antonio Franchi*
- [2021] **Active Interaction Force Control for Contact-Based Inspection with a Fully Actuated Aerial Vehicle** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/9295362) [pdf](https://arxiv.org/pdf/2003.09516v3) (ETH Zurich) ✦ *Roland Siegwart*
- [2020] **Aerial Manipulation Using Hybrid Force and Position NMPC Applied to Multirotor UAVs** · *RSS* [paper](https://www.roboticsproceedings.org/rss16/p046.pdf) (Imperial College London)
- [2017] **6D Physical Interaction with a Fully Actuated Aerial Robot** · *ICRA* [pdf](https://laas.hal.science/hal-01476814v1/document) (MPI for Biological Cybernetics, University of Cassino, CNRS-LAAS) ✦ *Antonio Franchi*
- [2012] **Impedance Control of an Aerial Manipulator** · *ACC* [paper](https://ieeexplore.ieee.org/document/6425020) (University of Bologna) ✦ *Lorenzo Marconi*
- [2012] **Cartesian Impedance Control of a UAV with a Robotic Arm** · *SYROCO* [pdf](https://www.fedoa.unina.it/9621/1/SYROCO12_0158_MS.pdf) (University of Naples Federico II)

---

## <a id="learning"></a>Learning-Based Methods

### <a id="simulators"></a>Simulators & Benchmarks

- [2026] ⭐ **AM-Bench: A Modular Simulation Suite and Benchmark for Aerial Manipulation Policy Learning** · *arXiv* [paper](https://arxiv.org/abs/2609.00641) [project](https://ambench.github.io) (The Chinese University of Hong Kong, CMU) ✦ *Guanya Shi* — *12 tasks, 3 embodiments; single-UAM only → multi-UAM is the open gap*
- [2025] **Aerial Gym Simulator: A Framework for Highly Parallelized Simulation of Aerial Robots (multi-linked embodiments)** · *arXiv* [paper](https://arxiv.org/abs/2503.01471) [pdf](https://arxiv.org/pdf/2503.01471) [code](https://github.com/ntnu-arl/aerial_gym_simulator) (NTNU) ✦ *Kostas Alexis* — *adds drone+arm multi-linked bodies*
- [2024] ⭐ **Aerial Gym: Isaac Gym Simulator for Aerial Robots** · *IEEE RA-L* [paper](https://arxiv.org/abs/2305.16510) [pdf](https://arxiv.org/pdf/2305.16510) [code](https://github.com/ntnu-arl/aerial_gym_simulator) (NTNU) ✦ *Kostas Alexis*
- [2020] **Flightmare: A Flexible Quadrotor Simulator** · *CoRL* [paper](https://arxiv.org/abs/2009.00563) [pdf](https://arxiv.org/pdf/2009.00563) [code](https://github.com/uzh-rpg/flightmare) (University of Zurich) ✦ *Davide Scaramuzza*

### <a id="rl"></a>RL & Learned Policies

- [2026] **AIR-VLA: Vision-Language-Action Systems for Aerial Manipulation** · *arXiv* [paper](https://arxiv.org/abs/2601.21602) [code](https://github.com/SpencerSon2001/AIR-VLA) (Institute of Automation, Chinese Academy of Sciences)
- [2026] **Whole-Body Aerial Grasping and Lifting via Partial Visual Observations** · *arXiv* [paper](https://arxiv.org/abs/2610.00404) [pdf](https://arxiv.org/pdf/2610.00404) (Nanyang Technological University)
- [2025] ⭐ **Decentralized Aerial Manipulation of a Cable-Suspended Load Using Multi-Agent Reinforcement Learning** · *arXiv* [paper](https://arxiv.org/abs/2508.01522) [pdf](https://arxiv.org/pdf/2508.01522) (TU Delft, UC Berkeley) ✦ *Javier Alonso-Mora* — *first real-world decentralized MARL multi-lift*
- [2025] **UMI-on-Air: Embodiment-Aware Guidance for Flying Manipulators** · *arXiv* [paper](https://arxiv.org/abs/2510.02614) [code](https://github.com/LeCAR-Lab/umi-on-air_checkpoints) (Shanghai Jiao Tong University)
- [2025] **CognitiveDrone: A VLA Model and Evaluation Benchmark for Real-Time Cognitive Task Solving in UAVs** · *IROS* [paper](https://arxiv.org/abs/2503.01378) [pdf](https://arxiv.org/pdf/2503.01378) (Skoltech)
- [2024] **Osprey: An Open-Source Soft Robotic Platform for Autonomous Aerial Manipulation in the Wild** · *CoRL* [paper](https://arxiv.org/abs/2409.07662) [pdf](https://arxiv.org/pdf/2409.07662) [code](https://github.com/srl-ethz/osprey) (ETH Zurich)
- [2023] ⭐ **Champion-Level Drone Racing Using Deep Reinforcement Learning (Swift)** · *Nature* [paper](https://www.nature.com/articles/s41586-023-06419-9) (University of Zurich) ✦ *Davide Scaramuzza*
- [2023] **A Deep Multi-Agent Reinforcement Learning Framework for Autonomous Aerial Navigation to Grasping Points on Loads** · *Robotics and Autonomous Systems* [paper](https://www.sciencedirect.com/science/article/pii/S0921889023001288) [pdf](https://eprints.whiterose.ac.uk/id/eprint/232609/1/1-s2.0-S0921889023001288-main.pdf) (Coventry University)

---

## <a id="multi-robot"></a>Multi-Robot Cooperation

### <a id="multi-uam"></a>Multi-UAM Cooperative Manipulation

- [2025] ⭐⭐ **Proximal Cooperative Aerial Manipulation with Vertically Stacked Drones** · *Nature* [paper](https://www.nature.com/articles/s41586-025-09575-x) [pdf](https://ndownloader.figshare.com/files/58224982) (Westlake University, Lancaster University) ✦ *Shiyu Zhao* — *tool handover between stacked drones under downwash*
- [2021] **Estimation and Control of Cooperative Aerial Manipulators for a Payload with an Arbitrary Center of Mass** · *Sensors* [paper](https://www.mdpi.com/1424-8220/21/19/6452) [pdf](https://pmc-oa-opendata.s3.amazonaws.com/PMC8512681.1/PMC8512681.1.pdf) (Korea Institute of Science and Technology)
- [2018] ⭐ **Cooperative Aerial Manipulation Using Multirotors with Multi-DOF Robotic Arms** · *IEEE/ASME Trans. Mechatronics* [paper](https://ieeexplore.ieee.org/document/8253830) (Seoul National University) ✦ *H. Jin Kim* — *flagship two-hexarotor+arm rod transport*
- [2018] **First Experimental Results on Motion Planning for Transportation in Aerial Long-Reach Manipulator with Two Arms** · *IROS* [paper](https://ieeexplore.ieee.org/document/8594123) [pdf](https://zenodo.org/records/2621105/files/A.Caballero_IROS_2018.pdf) (University of Seville)
- [2015] ⭐ **Hierarchical Cooperative Control Framework of Multiple Quadrotor-Manipulator Systems** · *ICRA* [paper](https://ieeexplore.ieee.org/document/7139844) (Seoul National University) ✦ *Dongjun Lee* — *first general multi-QMS framework*
- [2015] **Cooperative Impedance Control for Multiple UAVs with a Robotic Arm** · *IROS* [paper](https://ieeexplore.ieee.org/document/7353697) (University of Salerno)

### <a id="transport"></a>Multi-UAV Cooperative Transport

- [2025] ⭐ **Agile and Cooperative Aerial Manipulation of a Cable-Suspended Load** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.adu8015) [pdf](https://arxiv.org/pdf/2501.18802) (TU Delft, Sapienza University of Rome, University of Twente) ✦ *Javier Alonso-Mora*
- [2025] **Distributed NMPC for Cooperative Aerial Manipulation of Cable-Suspended Loads** · *IEEE RA-L* [paper](https://ieeexplore.ieee.org/document/11145772) [pdf](https://hal.science/hal-05239115v1/file/p2024b_distributed_MPC_.pdf) (University of Bologna, CNRS-LAAS)
- [2020] **Scalable Cooperative Transport of Cable-Suspended Loads with UAVs Using Distributed Trajectory Optimization (Team-Lift)** · *IEEE RA-L* [paper](https://ieeexplore.ieee.org/document/9073952) [pdf](https://thowell.github.io/documents/team_lift_ral.pdf) (Stanford University, CMU, UIUC) ✦ *Mac Schwager, Zachary Manchester*
- [2018] **Cooperative Object Transport in 3D with Multiple Quadrotors Using No Peer Communication** · *ICRA* [pdf](https://stanfordasl.github.io/wp-content/papercite-data/pdf/Wang.Singh.Pavone.ea.ICRA18.pdf) (Stanford University) ✦ *Marco Pavone*
- [2014] **Geometric Control of a Quadrotor with a Cable-Suspended Rigid Body** · *arXiv* [paper](https://arxiv.org/abs/1403.3684) (University of Pennsylvania) ✦ *Vijay Kumar*
- [2013] ⭐ **Geometric Control of a Quadrotor with a Cable-Suspended Load** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2013.2271569) [pdf](https://hybrid-robotics.berkeley.edu/publications/CDC2013.pdf) (University of Pennsylvania) ✦ *Vijay Kumar*
- [2013] **Geometric Control of Cooperating Multiple Quadrotor UAVs with a Suspended Payload** · *CDC* [pdf](https://hybrid-robotics.berkeley.edu/publications/CDC2013a.pdf) (University of Pennsylvania) ✦ *Vijay Kumar*
- [2013] **Cooperative Grasping and Transport Using Multiple Quadrotors** · *DARS* [paper](https://link.springer.com/chapter/10.1007/978-3-642-32723-0_39) [pdf](https://web.archive.org/web/20120526220045id_/http://www.seas.upenn.edu/~dmel/mellingerDARS10.pdf) (University of Pennsylvania) ✦ *Vijay Kumar*
- [2011] **Cooperative Manipulation and Transportation with Aerial Robots** · *Autonomous Robots* [paper](https://link.springer.com/article/10.1007/s10514-010-9205-0) [pdf](https://www.roboticsproceedings.org/rss05/p1.pdf) (University of Pennsylvania) ✦ *Vijay Kumar*

---

## <a id="applications"></a>Applications

### <a id="tools"></a>Tool Use & Field Operations

- [2025] **Pointillism Wall Painting Drone Using Bouncing Frequency Control** · *IEEE RA-L* [paper](https://ieeexplore.ieee.org/document/9830012) [pdf](https://hal.science/hal-05096557v1/file/STRAD_Format_IEEE_RA_L_Final_Version.pdf) (University Grenoble Alpes, GIPSA-lab)
- [2023] ⭐ **A Perching and Tilting Aerial Robot for Precise and Versatile Power Tool Work on Vertical Walls** · *IROS* [paper](https://arxiv.org/abs/2310.10548) [pdf](https://arxiv.org/pdf/2310.10548) (ETH Zurich) — *150 N concrete drilling*
- [2023] **Learning to Open Doors with an Aerial Manipulator** · *IROS* [paper](https://arxiv.org/abs/2307.15581) [pdf](https://arxiv.org/pdf/2307.15581) (ETH Zurich)
- [2022] ⭐ **Automated Aerial Screwing with a Fully Actuated Aerial Manipulator** · *IROS* [paper](https://ieeexplore.ieee.org/document/9981979) [pdf](https://fis.tu-dresden.de/portal/files/18179291/IROS22_submittedVersion_prePrint.pdf) (TU Dresden)
- [2020] **Aerial Manipulator with Rolling Base for Inspection of Pipe Arrays** · *IEEE Access* [paper](https://ieeexplore.ieee.org/document/9023885) [pdf](https://aerial-core.eu/wp-content/uploads/2021/01/Aerial-Manipulator-with-Rolling-Base-for-Inspection-of-Pipe-Arrays.pdf) (University of Seville)
- [2020] **Fully-Actuated Aerial Manipulator for Infrastructure Contact Inspection** · *IEEE TASE* [paper](https://ieeexplore.ieee.org/document/9114869) [pdf](https://idus.us.es/items/4338b496-9292-4a71-8462-c0cbfa414528) (University of Seville, University of Luxembourg)
- [2019] **Novel Aerial Manipulator for Accurate and Robust Industrial NDT Contact Inspection (AeroX)** · *Sensors* [paper](https://www.mdpi.com/1424-8220/19/6/1305) [pdf](https://idus.us.es/items/2f17021a-e2c3-4230-a5f1-74d1601d4351) (University of Seville)
- [2019] **Robotic System for Inspection by Contact of Bridge Beams Using UAVs** · *Sensors* [paper](https://www.mdpi.com/1424-8220/19/2/305) [pdf](https://idus.us.es/items/ec99ccc4-c208-4771-88b6-d655396aa4c8) (University of Seville)
- [2018] **PaintCopter: An Autonomous UAV for Spray Painting on 3D Surfaces** · *IEEE RA-L + IROS* [paper](https://ieeexplore.ieee.org/document/8432222) [pdf](http://disneyresearch.s3.amazonaws.com/wp-content/uploads/20181001120656/PaintCopter-An-Autonomous-UAV-for-Spray-Painting-on-3D-Surfaces-Paper.pdf) (Disney Research Zurich, ETH Zurich)
- [2014] ⭐ **Towards Valve Turning Using a Dual-Arm Aerial Manipulator** · *IROS* [paper](https://www.semanticscholar.org/paper/8f0aeb1a4216df9fa9a8def78c106c432c837bb1) (Worcester Polytechnic Institute, University of Zagreb)

### <a id="construction"></a>Aerial Construction & Heterogeneous Teams

- [2022] ⭐ **Aerial Additive Manufacturing with Multiple Autonomous Robots** · *Nature* [paper](https://www.nature.com/articles/s41586-022-04988-4) (Imperial College London, Empa) ✦ *Mirko Kovac*
- [2018] **Tele-MAGMaS: An Aerial–Ground Comanipulator System** · *IEEE RAM* [paper](https://ieeexplore.ieee.org/document/8644023) [pdf](https://inria.hal.science/hal-01935127v1/file/2018_ieeeram_staub.pdf) (CNRS-LAAS, University of Twente, University of Siena) ✦ *Paolo Robuffo Giordano*
- [2018] ⭐ **Modeling and Control of Multiple Aerial-Ground Manipulator System (MAGMaS) with Load Flexibility** · *IROS* [paper](https://ieeexplore.ieee.org/document/8593834) [pdf](https://laas.hal.science/hal-01964779v1/file/2018s-YanStaFraLee-preprint.pdf) (CNRS-LAAS, University of Seville, Seoul National University) ✦ *Antonio Franchi, Dongjun Lee*
- [2013] **Building Tensile Structures with Flying Machines** · *IROS* [paper](https://ieeexplore.ieee.org/document/6696853) [pdf](https://www.researchgate.net/publication/261353259_Building_tensile_structures_with_flying_machines) (ETH Zurich) ✦ *Raffaello D'Andrea*

---

## 🤝 Contributing

Pull requests are welcome! Suggested format:

```
- [Year] **Paper Title** · *Venue* [paper](link) [pdf](open-access-link) [code](repo) (Affiliation) ✦ *Renowned co-author*
```

⭐ = must-read · ✦ = paper from a renowned team / with a renowned co-author. Papers without an open-access copy link to the publisher page only.

## 📖 Citation

If you find this repository useful, please consider citing this list:

```bibtex
@misc{wuduidi2026awesomeuampapers,
    title = {Awesome-UAM-Papers},
    author = {WuDuidi},
    journal = {GitHub repository},
    url = {https://github.com/WuDuidi/Awesome-UAM-Papers},
    year = {2026},
}
```

## 📄 License

[MIT](https://opensource.org/licenses/MIT)
