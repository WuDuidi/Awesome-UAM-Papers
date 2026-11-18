# Awesome UAM Papers

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated reading list for **UAM — Unmanned Aerial Manipulators** (multirotor UAV + robot arm): platform design & morphology, whole-body control, disturbance rejection, contact-rich interaction, learning-based methods, and multi-robot cooperation for aerial manipulation.

🔖 Last updated: Nov 2026 · ✦ renowned teams · 🛸UAV = aerial-robot paper without a manipulator, kept for its role in the UAM stack · Contributions welcome via PR!

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
  - [Low-Level Control & Solvers](#low-level)
- [Learning-Based Methods](#learning)
  - [Simulators & Benchmarks](#simulators)
  - [RL & Learned Policies](#rl)
  - [Language-Grounding & VLA](#vla)
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

*UAV-only (no manipulator):*

- [2026] **UAVs Meet Embodied Intelligence: Bridging Human Intents and Flying Dynamics Via Harnessing Physical-Digital AI Agents** · *arXiv* [paper](https://arxiv.org/abs/2609.18326) (Institute of Automation, Chinese Academy of Sciences) 🛸UAV — *UAV-wide embodied-AI roadmap; the autonomy context above the UAM stack*

### <a id="nature-science"></a>Nature & Science Family

- [2026] **Hand-like Autonomous Flying Robot for Airborne Grasping and Interaction** · *Nature Communications* [paper](https://doi.org/10.1038/s41467-026-68967-3)
- [2026] **Octopus-Inspired Muscle Activation Unlocks High-DOF Motion from a Single Actuator** · *Science Advances* [paper](https://doi.org/10.1126/sciadv.aei4282)
- [2025] ⭐ **Proximal Cooperative Aerial Manipulation with Vertically Stacked Drones** · *Nature* [paper](https://www.nature.com/articles/s41586-025-09575-x) [pdf](https://ndownloader.figshare.com/files/58224982) (Westlake University, Lancaster University) ✦ *Shiyu Zhao*
- [2025] **Agile and Cooperative Aerial Manipulation of a Cable-Suspended Load** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.adu8015) [pdf](https://arxiv.org/pdf/2501.18802) (TU Delft, Sapienza University of Rome, University of Twente) ✦ *Javier Alonso-Mora*
- [2025] **Embodied Aerial Physical Interaction: Combining Body and Brain for Robust Interaction with Unstructured Environments** · *Science Robotics* [paper](https://doi.org/10.1126/scirobotics.ads0200) (EPFL)
- [2025] **A Dexterous and Compliant Aerial Continuum Manipulator for Cluttered and Constrained Environments** · *Nature Communications* [paper](https://doi.org/10.1038/s41467-024-55157-2)
- [2024] **Powerful UAV Manipulation via Bioinspired Self-Adaptive Soft Self-Contained Gripper** · *Science Advances* [paper](https://doi.org/10.1126/sciadv.adn6642)
- [2023] ⭐ **Champion-Level Drone Racing Using Deep Reinforcement Learning (Swift)** · *Nature* [paper](https://www.nature.com/articles/s41586-023-06419-9) (University of Zurich) ✦ *Davide Scaramuzza* 🛸UAV — *sim-to-real RL landmark for the flight stack every UAM builds on*
- [2022] ⭐ **Aerial Additive Manufacturing with Multiple Autonomous Robots** · *Nature* [paper](https://www.nature.com/articles/s41586-022-04988-4) (Imperial College London, Empa) ✦ *Mirko Kovac*
- [2021] **Bird-Inspired Dynamic Grasping and Perching in Arboreal Environments (SNAG)** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.abj7562) [pdf](https://lentinklab.com/wp-content/uploads/2023/12/2021-bird-inspired-perching.pdf) (Stanford University) ✦ *David Lentink*

*UAV-only (no manipulator):*

- [2026] **RAPTOR: A Foundation Policy for Quadrotor Control** · *Science Robotics* [paper](https://doi.org/10.1126/scirobotics.aec1481) (NYU) ✦ *Giuseppe Loianno* 🛸UAV — *flight-level foundation policy; the base controller future UAM policies may inherit*
- [2025] **Learning Vision-Based Agile Flight via Differentiable Physics** · *Nature Machine Intelligence* [paper](https://www.nature.com/articles/s42256-025-01048-0) [pdf](https://arxiv.org/pdf/2407.10648) (Shanghai Jiao Tong University) 🛸UAV — *differentiable-physics flight learning; methodology transferable to UAM sim-to-real*
- [2024] **Scale-Inspired Programmable Robotic Structures with Concurrent Shape Morphing and Stiffness Variation** · *Science Robotics* [paper](https://doi.org/10.1126/scirobotics.adl0307) 🛸UAV — *fish-scale morphing-stiffness structures: airframe/skin mechanism, no end-effector*
- [2022] **Swarm of Micro Flying Robots in the Wild** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.abm5954) [pdf](https://zhepeiwang.github.io/pubs/sr_2022_swarm.pdf) [code](https://github.com/ZJU-FAST-Lab/EGO-Planner-v2) (Zhejiang University) ✦ *Fei Gao, Boyu Zhou* 🛸UAV — *decentralized swarm autonomy: the navigation layer of multi-UAM teams*
- [2021] **Learning High-Speed Flight in the Wild** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.abg5810) [pdf](https://rpg.ifi.uzh.ch/docs/Loquercio21_Science.pdf) (University of Zurich) ✦ *Davide Scaramuzza* 🛸UAV — *high-speed wild navigation: perception-planning backbone for field UAM*
- [2021] **Enhancing Optical-Flow-Based Control by Learning Visual Appearance Cues for Flying Robots** · *Nature Machine Intelligence* [paper](https://doi.org/10.1038/s42256-020-00279-7) (TU Delft) ✦ *Guido de Croon* 🛸UAV — *fly-vision flight control; lightweight sensing principle for UAM state estimation*
- [2021] **Predictive Control of Aerial Swarms in Cluttered Environments** · *Nature Machine Intelligence* [paper](https://www.nature.com/articles/s42256-021-00341-y) (EPFL) ✦ *Dario Floreano* 🛸UAV — *NMPC swarm coordination: the multi-robot layer above multi-UAM*
- [2020] **Soft Biohybrid Morphing Wings with Feathers Underactuated by Wrist and Finger Actuation (PigeonBot)** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.aay1246) [project](https://www.erchang.org/pigeonbot) (Stanford University) ✦ *David Lentink* 🛸UAV — *biohybrid morphing-wing flight platform (no arm)*
- [2019] **Untethered Flight of an Insect-Sized Flapping-Wing Microscale Aerial Vehicle (RoboBee X-Wing)** · *Nature* [paper](https://www.nature.com/articles/s41586-019-1322-0) (Harvard University) ✦ *Robert Wood* 🛸UAV — *insect-scale flapping flight platform (no arm)*
- [2017] **A Biomimetic Robotic Platform to Study Flight Specializations of Bats (Bat Bot B2)** · *Science Robotics* [paper](https://pubmed.ncbi.nlm.nih.gov/33157861) [pdf](https://faculty.cc.gatech.edu/~seth/ResPages/pdfs/ScienceRobotics2017.pdf) (Caltech, UIUC) ✦ *Soon-Jo Chung* 🛸UAV — *bat-inspired flapping platform (no arm)*

### <a id="tro"></a>IEEE T-RO Selection

- [2026] **Effector-Centric NMPC of Tiltable-Multirotors for Offset-Free Omnidirectional Aerial Manipulation** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2026.3731683) (University of Tokyo) ✦ *Moju Zhao*
- [2025] **Optical Tactile Sensing for Aerial Multicontact Interaction: Design, Integration, and Evaluation** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2024.3508140) (ETH Zurich) ✦ *Raffaello D'Andrea*
- [2025] **Whole-Body Integrated Motion Planning for Aerial Manipulators (AM-Planner)** · *IEEE T-RO* [paper](https://arxiv.org/abs/2501.06493) [code](https://github.com/SYSU-HILAB/am-planner) (Sun Yat-sen University) — *first whole-body (base + arm) integrated planner for aerial manipulators*
- [2024] **Perching and Grasping Using a Passive Dynamic Bioinspired Gripper** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2023.3336216)
- [2024] **Design, Control, and Motion Planning for a Root-Perching Rotor-Distributed Manipulator** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2023.3327634) (University of Tokyo)
- [2022] ⭐ **Past, Present, and Future of Aerial Robotic Manipulators** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/9462539) [pdf](https://idus.us.es/bitstreams/954638e3-7b65-4817-889e-a476317572a0/download) (University of Seville, CNRS-LAAS, University of Twente, Seoul National University) ✦ *Aníbal Ollero*
- [2021] ⭐ **Active Interaction Force Control for Contact-Based Inspection with a Fully Actuated Aerial Vehicle** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/9295362) [pdf](https://arxiv.org/pdf/2003.09516v3) (ETH Zurich) ✦ *Roland Siegwart*
- [2018] **A Novel Robotic Platform for Aerial Manipulation Using Quadrotors as Rotating Thrust Generators** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/8294249) (Seoul National University) ✦ *Dongjun Lee* — *quadrotors spin around a jointed arm to generate joint torques*

*UAV-only (no manipulator):*

- [2025] **From Flies to Robots: Inverted Landing in Small Quadcopters With Dynamic Perching** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2025.3543263) (Beihang University) 🛸UAV — *fly-inspired inverted landing: docking maneuver primitive for UAM stations*
- [2024] **Adaptive Tracking and Perching for Quadrotor in Dynamic Scenarios** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2023.3335670) (Zhejiang University) ✦ *Fei Gao* 🛸UAV — *perching on moving targets: docking skill for dynamic grasping*
- [2024] **Impact-Aware Planning and Control for Aerial Robots With Suspended Payloads** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2024.3381555) (Zhejiang University) ✦ *Fei Gao* 🛸UAV — *impact-aware suspended-payload planning: payload dynamics relevant to arm-held loads*
- [2023] **Robust Active Visual Perching With Quadrotors on Inclined Surfaces** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2023.3238911) (NYU) ✦ *Giuseppe Loianno* 🛸UAV — *vision-based perching: precise base positioning before manipulation*
- [2013] ⭐ **Geometric Control of a Quadrotor with a Cable-Suspended Load** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2013.2271569) [pdf](https://hybrid-robotics.berkeley.edu/publications/CDC2013.pdf) (University of Pennsylvania) ✦ *Vijay Kumar* 🛸UAV — *cable-load differential flatness: the transport-dynamics foundation*

### <a id="foundations"></a>Classic Foundations

- [2018] **Design of a Lightweight Dual Arm System for Aerial Manipulation** · *Bioinspiration & Biomimetics* [paper](https://doi.org/10.1088/1748-3190/aa9d51) [pdf](https://idus.us.es/bitstreams/8aa25e92-ae25-4a04-8f29-8735f5232399/download) (University of Seville)
- [2018] **An Anthropomorphic, Compliant, and Lightweight Dual Arm for Aerial Manipulation** · *IEEE Access* [paper](https://ieeexplore.ieee.org/document/8354886) [pdf](https://idus.us.es/bitstream/11441/87747/1/IEEEA_Suarez_2018_Design.pdf) (University of Seville)
- [2014] **Aerial Manipulation Robot Composed of an Autonomous Helicopter and a 7-DOF Industrial Manipulator** · *ICRA* [paper](https://doi.org/10.1109/ICRA.2014.6907148) (DLR — German Aerospace Center)
- [2012] **Cartesian Impedance Control of a UAV with a Robotic Arm** · *SYROCO* [pdf](https://www.fedoa.unina.it/9621/1/SYROCO12_0158_MS.pdf) (University of Naples Federico II)
- [2012] **Impedance Control of an Aerial Manipulator** · *ACC* [paper](https://ieeexplore.ieee.org/document/6425020) (University of Bologna) ✦ *Lorenzo Marconi*
- [2011] ⭐ **Grasping from the Air: Hovering Capture and Load Stability** · *ICRA* [paper](https://www.eng.yale.edu/grablab/pubs/Pounds_ICRA2011.pdf) (Yale University) ✦ *Aaron Dollar*

*UAV-only (no manipulator):*

- [2022] **A Benchmark Comparison of Learned Control Policies for Agile Quadrotor Flight (CTBR)** · *ICRA* [paper](https://arxiv.org/abs/2202.10796) [pdf](https://arxiv.org/pdf/2202.10796) (University of Zurich) ✦ *Davide Scaramuzza* 🛸UAV — *collective-thrust & body-rate (CTBR) command interface transfers sim-to-real better than per-rotor thrusts; the low-level command layer of every UAM*

---

## <a id="platforms"></a>Platforms & Morphology

### <a id="bio-inspired"></a>Bio-Inspired UAM

*Each entry notes the biological model and the borrowed idea.*

- [2026] **Octopus-Inspired Muscle Activation Unlocks High-DOF Motion from a Single Actuator** · *Science Advances* [paper](https://doi.org/10.1126/sciadv.aei4282) — 🐙 *model: octopus arm musculature; idea: stereotyped muscle-activation patterns give high-DOF continuum motion from one actuator*
- [2026] **Hand-like Autonomous Flying Robot for Airborne Grasping and Interaction** · *Nature Communications* [paper](https://doi.org/10.1038/s41467-026-68967-3) — ✋ *model: human/avian hand prehension; idea: a multi-fingered hand-like gripper with autonomous onboard grasping on a flying robot*
- [2026] **Bioinspired Adaptive Leg-Claw Enables Robust Perching and Grasping for UAVs** · *Advanced Science* [paper](https://doi.org/10.1002/advs.202523518) — 🦅 *model: raptor leg-claw; idea: passive-adaptive leg-claw mechanism for perching and grasping on varied surfaces*
- [2025] **A Dexterous and Compliant Aerial Continuum Manipulator for Cluttered and Constrained Environments** · *Nature Communications* [paper](https://doi.org/10.1038/s41467-024-55157-2) — 🐍 *model: continuum limbs (elephant trunk/tentacle); idea: soft continuum arm navigates cluttered spaces rigid arms cannot*
- [2024] **Powerful UAV Manipulation via Bioinspired Self-Adaptive Soft Self-Contained Gripper** · *Science Advances* [paper](https://doi.org/10.1126/sciadv.adn6642) — 🦎 *model: self-adaptive animal grasping (e.g., gecko/fin ray); idea: soft self-contained underactuated gripper with high payload-to-weight ratio*
- [2021] ⭐ **Bird-Inspired Dynamic Grasping and Perching in Arboreal Environments (SNAG)** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.abj7562) [pdf](https://lentinklab.com/wp-content/uploads/2023/12/2021-bird-inspired-perching.pdf) (Stanford University) ✦ *David Lentink* — 🐦 *model: peregrine-falcon / parrotlet legs & tendons; idea: stereotyped 50-ms snatch-and-grasp reflex + tendon lock for a 3D-printed perching gripper*

*UAV-only (no manipulator):*

- [2024] **Scale-Inspired Programmable Robotic Structures with Concurrent Shape Morphing and Stiffness Variation** · *Science Robotics* [paper](https://doi.org/10.1126/scirobotics.adl0307) 🛸UAV — 🐟 *model: fish scales; morphing-stiffness structures — airframe/skin mechanism, no end-effector*
- [2023] **Synergistic Morphology and Feedback Control for Traversal of Unknown Compliant Obstacles with Aerial Robots** · *preprint (Research Square)* [paper](https://doi.org/10.21203/rs.3.rs-3262987/v1) (EPFL, Scuola Superiore Sant'Anna) 🛸UAV — 🌿 *model: insect/vegetation traversal; compliant body-environment synergy — flight platform morphology, no arm*
- [2021] **Enhancing Optical-Flow-Based Control by Learning Visual Appearance Cues for Flying Robots** · *Nature Machine Intelligence* [paper](https://doi.org/10.1038/s42256-020-00279-7) (TU Delft) ✦ *Guido de Croon* 🛸UAV — 🪰 *model: insect vision; flight-control sensing, no manipulation*
- [2020] **PigeonBot — Soft Biohybrid Morphing Wings with Feathers** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.aay1246) [project](https://www.erchang.org/pigeonbot) (Stanford University) ✦ *David Lentink* 🛸UAV — 🕊️ *model: pigeon wing; biohybrid morphing-wing flight platform, no arm*
- [2019] **RoboBee X-Wing — Untethered Insect-Sized Flapping Flight** · *Nature* [paper](https://www.nature.com/articles/s41586-019-1322-0) (Harvard University) ✦ *Robert Wood* 🛸UAV — 🐝 *model: insect flapping flight; micro flight platform, no arm*
- [2017] **Bat Bot B2 — A Biomimetic Robotic Bat** · *Science Robotics* [paper](https://pubmed.ncbi.nlm.nih.gov/33157861) [pdf](https://faculty.cc.gatech.edu/~seth/ResPages/pdfs/ScienceRobotics2017.pdf) (Caltech, UIUC) ✦ *Soon-Jo Chung* 🛸UAV — 🦇 *model: bat wing; articulated membrane flapping platform, no arm*

### <a id="fully-actuated"></a>Fully-Actuated & Omnidirectional Platforms

- [2026] **Effector-Centric NMPC of Tiltable-Multirotors for Offset-Free Omnidirectional Aerial Manipulation** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2026.3731683) (University of Tokyo) ✦ *Moju Zhao* — *effector-centric NMPC keeps the end-effector offset-free while the tiltable platform reorients*
- [2026] **FAM-DQ: A Dual-Quadrotor-Based Fully Actuated Aerial Manipulator for High-Torque Interaction** · *arXiv* [paper](https://arxiv.org/abs/2608.13220) — *two coupled quadrotors form a fully-actuated arm base for high-torque tasks*
- [2021] **Dynamic End Effector Tracking With an Omnidirectional Parallel Aerial Manipulator** · *IEEE RA-L* [paper](https://doi.org/10.1109/LRA.2021.3101864) (ETH Zurich) ✦ *Roland Siegwart*
- [2020] **Fully-Actuated Aerial Manipulator for Infrastructure Contact Inspection: Design, Modeling, Localization, and Control** · *IEEE TASE* [paper](https://ieeexplore.ieee.org/document/9114869) [pdf](https://idus.us.es/items/4338b496-9292-4a71-8462-c0cbfa414528) (University of Seville, University of Luxembourg)
- [2019] ⭐ **An Omnidirectional Aerial Manipulation Platform for Robust Interaction with Unstructured Environments** · *RSS* [paper](https://www.roboticsproceedings.org/rss15/p19.pdf) (ETH Zurich) ✦ *Roland Siegwart*
- [2018] **ODAR: Aerial Manipulation Platform Enabling Omnidirectional Wrench Generation** · *IEEE/ASME Trans. Mechatronics* [paper](https://ieeexplore.ieee.org/document/8401328) (Seoul National University) ✦ *Dongjun Lee (co-author)*
- [2017] **6D Physical Interaction with a Fully Actuated Aerial Robot** · *ICRA* [pdf](https://laas.hal.science/hal-01476814v1/document) (MPI for Biological Cybernetics, University of Cassino, CNRS-LAAS) ✦ *Antonio Franchi*
- [2016] **Modeling and Control of FAST-Hex: A Fully-Actuated and Tiltable Hexarotor** · *IROS* [paper](https://ieeexplore.ieee.org/document/7759271) [pdf](https://hal.science/hal-01348538v1/document) (MPI for Biological Cybernetics, University of Twente, CNRS-LAAS) ✦ *Antonio Franchi*
- [2015] **Modeling, Control and Design Optimization for a Fully-Actuated Hexarotor** · *ICRA* [pdf](https://hal.science/hal-01134829v1/document) (MPI for Biological Cybernetics, University of Twente) ✦ *Antonio Franchi, Heinrich Bülthoff*

*UAV-only (no manipulator):*

- [2025] **Anti-Windup Active Disturbance Rejection Control of Tiltable-Rotors Fully-Actuated Hexarotor** · *Int. J. Advanced Robotic Systems* [paper](https://doi.org/10.1177/17298806251331321) 🛸UAV — *ADRC + anti-windup flight control of the tiltable fully-actuated base (no arm)*

### <a id="morphing"></a>Morphing & Reconfigurable UAV/UAM

*Each entry notes the morphing / reconfiguration mechanism.*

- [2019] **DRAGON — A Dual-Rotor-Embedded Multilink Robot with Multi-DoF Aerial Transformation** · *IEEE RA-L* [paper](https://ieeexplore.ieee.org/document/8258850) [project](https://www.dragon.t.u-tokyo.ac.jp/publications/references/2018-ral-dragon-zhao) (University of Tokyo) ✦ *Moju Zhao (JSK Lab)* — 🐉 *mechanism: snake-like chain of 2-DoF links, each with a vectorable dual-rotor unit; transforms its whole shape mid-flight (line→L→S) to slalom through gaps, later extended into a flying manipulator*
- [2016] **FAST-Hex — A Fully-Actuated and Tiltable Hexarotor** · *IROS* [paper](https://ieeexplore.ieee.org/document/7759271) [pdf](https://hal.science/hal-01348538v1/document) (MPI for Biological Cybernetics, University of Twente, CNRS-LAAS) ✦ *Antonio Franchi* — 🔧 *mechanism: one central servo tilts all six arms together, switching between underactuated and fully-actuated flight in mid-air*

*UAV-only (no manipulator):*

- [2026] **MorphQuad: Morphable Quadrotor for Superhuman Maneuverability, Manipulation, and Resiliency** · *arXiv* [paper](https://arxiv.org/abs/2607.02764) (UC Berkeley) 🛸UAV — 🔧 *mechanism: servo-driven morphing arms shrink/grow the airframe in flight; morphable platform concept for future UAM*
- [2020] **PigeonBot — Biohybrid Feathered Morphing Wing** · *Science Robotics* [paper](https://www.science.org/doi/10.1126/scirobotics.aay1246) [project](https://www.erchang.org/pigeonbot) (Stanford University) ✦ *David Lentink* 🛸UAV — 🪶 *mechanism: passive feather deployment via elastic skin, wing area/shape morphs with only wrist & finger actuation*
- [2019] **A Quadrotor with an Origami-Inspired Protective Mechanism** · *IEEE RA-L* [paper](https://arxiv.org/abs/1907.07056) (City University of Hong Kong) 🛸UAV — 🗂️ *mechanism: passive origami foldable airframe/cage that buckles to absorb collision impact and self-restores in flight*

---

## <a id="control"></a>Control

### <a id="wbc"></a>Whole-Body Control & Loco-Manipulation

- [2026] **QuadHand: A Compact Quadrotor Aerial Manipulator with MRC-SDF-Based Whole-Body Motion Planning** · *arXiv* [paper](https://arxiv.org/abs/2609.35094) (Nanyang Technological University) — *compact 3-DoF-arm quadrotor with MRC-SDF whole-body planning*
- [2026] **Aerial Manipulation in the Wild with Onboard Perception, Policy Learning, and Whole-Body Control** · *arXiv* [paper](https://arxiv.org/abs/2609.30521) (The Chinese University of Hong Kong) — *visuomotor diffusion policy on top of a WBC with onboard LiDAR-inertial state estimation; outdoor, no motion capture*
- [2026] **Global End-Effector Pose Control of an Underactuated Aerial Manipulator via Reinforcement Learning** · *ICRA* [paper](https://arxiv.org/abs/2512.21085) [pdf](https://arxiv.org/pdf/2512.21085) (TU Delft) — *RL whole-body coordination of quadrotor + 2-DoF arm for full 6-DoF end-effector pose, incl. pushing and heavy loads*
- [2025] **Flying Hand: End-Effector-Centric Framework for Versatile Aerial Manipulation** · *RSS* [paper](https://www.roboticsproceedings.org/rss21/p130.pdf) [pdf](https://arxiv.org/abs/2504.10334) (CMU)
- [2025] **Whole-Body Integrated Motion Planning for Aerial Manipulators (AM-Planner)** · *IEEE T-RO* [paper](https://arxiv.org/abs/2501.06493) [code](https://github.com/SYSU-HILAB/am-planner) (Sun Yat-sen University) — *joint base+arm waypoint optimization for versatile aerial tasks*
- [2023] **Hierarchical Whole-Body Control of the Cable-Suspended Aerial Manipulator with Winch-Based Actuation** · *arXiv* [paper](https://arxiv.org/abs/2305.16466) (Korea University, DLR) — *hierarchical WBC for the winch-actuated cable-suspended manipulator (SAM lineage)*
- [2025] **Predictive Kinematic Coordinate Control for Aerial Manipulators Based on Modified Kinematics Learning** · *ICRA* [paper](https://doi.org/10.1109/ICRA55743.2025.11128580) (Westlake University) ✦ *Shiyu Zhao* — *learned modified kinematics improve coordinate control of the arm*
- [2025] **Prespecified-Performance Kinematic Tracking Control for Aerial Manipulation** · *IEEE RA-L* [paper](https://doi.org/10.1109/LRA.2025.3609098) (Westlake University) ✦ *Shiyu Zhao* — *guaranteed prescribed transient accuracy for end-effector tracking*
- [2024] **Avian-Inspired High-Precision Tracking Control for Aerial Manipulators** · *Nonlinear Dynamics* [paper](https://doi.org/10.1007/s11071-024-10584-0) (Westlake University) ✦ *Shiyu Zhao* — *avian-inspired pursuit guidance adapted to arm tracking (simulation)*
- [2020] **Aerial Manipulation Using Hybrid Force and Position NMPC Applied to Aerial Writing** · *RSS* [paper](https://www.roboticsproceedings.org/rss16/p046.pdf) (Imperial College London) — *hybrid force/position NMPC demonstrated on contact writing*
- [2019] **AeroVR: Virtual Reality-Based Teleoperation with Tactile Feedback for Aerial Manipulation** · *ICAR* [paper](https://doi.org/10.1109/ICAR46387.2019.8981574) (Skoltech) — *VR teleoperation with haptic/tactile feedback for a UAM*
- [2012] **Cartesian Impedance Control of a UAV with a Robotic Arm** · *SYROCO* [pdf](https://www.fedoa.unina.it/9621/1/SYROCO12_0158_MS.pdf) (University of Naples Federico II) — *foundational coupled base-arm Cartesian impedance*

### <a id="disturbance"></a>Disturbance Compensation & Estimation

*Wind, downwash, contact interaction, and arm-motion reaction — estimation and rejection.*

- [2025] ⭐ **Proximal Cooperative Aerial Manipulation with Vertically Stacked Drones** · *Nature* [paper](https://www.nature.com/articles/s41586-025-09575-x) [pdf](https://ndownloader.figshare.com/files/58224982) (Westlake University, Lancaster University) ✦ *Shiyu Zhao* — *explicit downwash modeling and compensation between stacked vehicles*
- [2025] **Predictive Admittance Control for Aerial Physical Interaction** · *IEEE RA-L* [paper](https://ieeexplore.ieee.org/document/11155162) [pdf](https://ayhamalharbat.github.io/publication/2025-4-ral/2025-4-RAL.pdf) (University of Twente) ✦ *Antonio Franchi* — *model-based prediction to hold the desired impedance through contact/free-flight transitions*
- [2024] **ESO-Based Robust and High-Precision Tracking Control for Aerial Manipulation** · *IEEE TASE* [paper](https://doi.org/10.1109/TASE.2023.3260874) (Westlake University) ✦ *Shiyu Zhao* — *extended-state-observer estimates and rejects arm-motion/coupling disturbances for mm-level end-effector tracking*
- [2024] **Robust Control of an Aerial Manipulator Based on a Variable Inertia Parameters Model** · *arXiv* [paper](https://arxiv.org/abs/2401.04316) (Shenyang Institute of Automation, CAS; Toronto Metropolitan University) — *arm-induced variable inertia explicitly modeled and compensated*
- [2021] **Active Interaction Force Control for Contact-Based Inspection with a Fully Actuated Aerial Vehicle** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/9295362) [pdf](https://arxiv.org/pdf/2003.09516v3) (ETH Zurich) ✦ *Roland Siegwart* — *maintains desired contact force while rejecting interaction disturbances*

*UAV-only (no manipulator):*

- [2009] **Wind Disturbance Estimation and Rejection for Quadrotor Position Control** · *AIAA Infotech@Aerospace* [paper](https://www.researchgate.net/publication/260122517_Wind_Disturbance_Estimation_and_Rejection_for_Quadrotor_Position_Control) (Stanford University) 🛸UAV — *classic wind-drag modeling + integral sliding-mode rejection on STARMAC: the flying base under every UAM*

### <a id="contact-force"></a>Contact & Force Interaction

- [2025] **Predictive Admittance Control for Aerial Physical Interaction** · *IEEE RA-L* [paper](https://ieeexplore.ieee.org/document/11155162) [pdf](https://ayhamalharbat.github.io/publication/2025-4-ral/2025-4-RAL.pdf) (University of Twente) ✦ *Antonio Franchi*
- [2025] **Optical Tactile Sensing for Aerial Multicontact Interaction: Design, Integration, and Evaluation** · *IEEE T-RO* [paper](https://doi.org/10.1109/TRO.2024.3508140) (ETH Zurich) ✦ *Raffaello D'Andrea* — *vision-based tactile sensors on the airframe enable multicontact interaction*
- [2023] **Aerial Interaction with Tactile Sensing** · *arXiv (IROS'24)* [paper](https://arxiv.org/abs/2310.00142) (The Chinese University of Hong Kong) ✦ *Junyi Geng* — *low-cost tactile-sensing fingertips for aerial contact tasks*
- [2022] **Energy Tank-Based Policies for Robust Aerial Physical Interaction with Moving Objects** · *ICRA* [paper](https://doi.org/10.1109/ICRA46639.2022.9812342) (ETH Zurich) ✦ *Roland Siegwart, Marco Tognon*
- [2022] **Towards 6DoF Bilateral Teleoperation of an Omnidirectional Aerial Vehicle for Aerial Physical Interaction** · *ICRA* [paper](https://doi.org/10.1109/ICRA46639.2022.9812346) (ETH Zurich) ✦ *Roland Siegwart, Marco Tognon*
- [2021] **Active Interaction Force Control for Contact-Based Inspection with a Fully Actuated Aerial Vehicle** · *IEEE T-RO* [paper](https://ieeexplore.ieee.org/document/9295362) [pdf](https://arxiv.org/pdf/2003.09516v3) (ETH Zurich) ✦ *Roland Siegwart*
- [2020] **Aerial Manipulation Using Hybrid Force and Position NMPC Applied to Aerial Writing** · *RSS* [paper](https://www.roboticsproceedings.org/rss16/p046.pdf) (Imperial College London)
- [2017] **6D Physical Interaction with a Fully Actuated Aerial Robot** · *ICRA* [pdf](https://laas.hal.science/hal-01476814v1/document) (MPI for Biological Cybernetics, University of Cassino, CNRS-LAAS) ✦ *Antonio Franchi*
- [2012] **Impedance Control of an Aerial Manipulator** · *ACC* [paper](https://ieeexplore.ieee.org/document/6425020) (University of Bologna) ✦ *Lorenzo Marconi*
- [2012] **Cartesian Impedance Control of a UAV with a Robotic Arm** · *SYROCO* [pdf](https://www.fedoa.unina.it/9621/1/SYROCO12_0158_MS.pdf) (University of Naples Federico II)

### <a id="low-level"></a>Low-Level Control & Solvers

*Tooling that UAM controllers commonly build on — all flight-level (no arm).*

- [2021] **acados — A Modular Open-Source Framework for Fast Embedded Optimal Control** · *Mathematical Programming Computation* [paper](https://doi.org/10.1007/s12532-021-00208-8) [code](https://github.com/acados/acados) (KU Leuven, ETH Zurich, TUM) 🛸UAV — *the de-facto NMPC solver backend for aerial WBC/force-control stacks*
- [2022] **L1 Adaptive Augmentation for Geometric Tracking Control of Quadrotors** · *ICRA* [paper](https://doi.org/10.1109/ICRA46639.2022.9811946) (University of Illinois Urbana-Champaign) 🛸UAV — *L1 adaptive augmentation on SE(3) geometric controllers for fast adaptation*
- [2009] **From PID to Active Disturbance Rejection Control** · *IEEE Trans. Industrial Electronics* [paper](https://doi.org/10.1109/TIE.2008.2011621) (Chinese Academy of Sciences) 🛸UAV — *Jingqing Han's canonical ADRC paper; basis of ESO-based UAM disturbance rejection*

---

## <a id="learning"></a>Learning-Based Methods

### <a id="simulators"></a>Simulators & Benchmarks

- [2026] ⭐ **AM-Bench: A Modular Simulation Suite and Benchmark for Aerial Manipulation Policy Learning** · *arXiv* [paper](https://arxiv.org/abs/2609.00641) [project](https://ambench.github.io) (The Chinese University of Hong Kong, CMU) ✦ *Guanya Shi* — *12 tasks, 3 embodiments; single-UAM only → multi-UAM is the open gap*
- [2026] **Benchmarking Interaction-Oriented Aerial Mobility across Heterogeneous Environments (CrosFly)** · *arXiv* [paper](https://arxiv.org/abs/2610.18381) — *interaction-oriented aerial mobility benchmark across heterogeneous environments*
- [2025] **Aerial Gym Simulator: A Framework for Highly Parallelized Simulation of Aerial Robots (multi-linked embodiments)** · *arXiv* [paper](https://arxiv.org/abs/2503.01471) [pdf](https://arxiv.org/pdf/2503.01471) [code](https://github.com/ntnu-arl/aerial_gym_simulator) (NTNU) ✦ *Kostas Alexis* — *adds drone+arm multi-linked bodies*
- [2024] ⭐ **Aerial Gym: Isaac Gym Simulator for Aerial Robots** · *IEEE RA-L* [paper](https://arxiv.org/abs/2305.16510) [pdf](https://arxiv.org/pdf/2305.16510) [code](https://github.com/ntnu-arl/aerial_gym_simulator) (NTNU) ✦ *Kostas Alexis*
- [2020] **Benchmarks for Aerial Manipulation** · *IEEE RA-L* [paper](https://doi.org/10.1109/LRA.2020.2972870) (University of Seville) — *early quantitative benchmark of aerial manipulation capabilities*

*UAV-only (no manipulator):*

- [2026] **AerialDojo-200K: A Large-Scale Benchmark Suite for Open-World Aerial Object-Goal Search** · *arXiv* [paper](https://arxiv.org/abs/2609.36066) 🛸UAV — *open-world aerial object-goal navigation benchmark: the search layer above UAM tasks*
- [2024] **OmniDrones: An Efficient and Flexible Platform for Reinforcement Learning in Drone Control** · *IEEE RA-L* [paper](https://doi.org/10.1109/LRA.2024.3356168) [code](https://github.com/btx042/OmniDrones) (Peking University) 🛸UAV — *multi-drone RL platform, extendable with manipulator embodiments*
- [2020] **Flightmare: A Flexible Quadrotor Simulator** · *CoRL* [paper](https://arxiv.org/abs/2009.00563) [pdf](https://arxiv.org/pdf/2009.00563) [code](https://github.com/uzh-rpg/flightmare) (University of Zurich) ✦ *Davide Scaramuzza* 🛸UAV — *quadrotor simulator with rendering/physics split: flight-side backend*

### <a id="rl"></a>RL & Learned Policies

- [2026] **Reinforcement Learning with Inner-Loop Dynamics Estimator for Aerial Manipulation Under Uncertainty** · *CASE* [paper](https://doi.org/10.1109/CASE69030.2026.11704236) — *inner-loop dynamics estimator stabilizes RL policies under model uncertainty*
- [2026] **Autonomous Aerial Manipulation via Contextual Contrastive Meta Reinforcement Learning (Aco²)** · *arXiv* [paper](https://arxiv.org/abs/2606.08533) (Nanyang Technological University) — *meta-RL with contextual contrastive pretraining for fast task adaptation*
- [2026] **Whole-Body Aerial Grasping and Lifting via Partial Visual Observations** · *arXiv* [paper](https://arxiv.org/abs/2610.00404) [pdf](https://arxiv.org/pdf/2610.00404) (Nanyang Technological University)
- [2025] **Swooper: Learning High-Speed Aerial Grasping with a Simple Gripper** · *IEEE RA-L* [paper](https://doi.org/10.1109/LRA.2025.3643298) — *high-speed aerial grasping (>50 km/h approach) with a simple gripper*
- [2025] ⭐ **Decentralized Aerial Manipulation of a Cable-Suspended Load Using Multi-Agent Reinforcement Learning** · *arXiv* [paper](https://arxiv.org/abs/2508.01522) [pdf](https://arxiv.org/pdf/2508.01522) (TU Delft, UC Berkeley) ✦ *Javier Alonso-Mora* — *first real-world decentralized MARL multi-lift*
- [2025] **UMI-on-Air: Embodiment-Aware Guidance for Flying Manipulators** · *arXiv* [paper](https://arxiv.org/abs/2510.02614) [code](https://github.com/LeCAR-Lab/umi-on-air_checkpoints) (Shanghai Jiao Tong University)
- [2025] **CognitiveDrone: A VLA Model and Evaluation Benchmark for Real-Time Cognitive Task Solving in UAVs** · *IROS* [paper](https://arxiv.org/abs/2503.01378) [pdf](https://arxiv.org/pdf/2503.01378) (Skoltech)
- [2024] **Osprey: An Open-Source Soft Robotic Platform for Autonomous Aerial Manipulation in the Wild** · *CoRL* [paper](https://arxiv.org/abs/2409.07662) [pdf](https://arxiv.org/pdf/2409.07662) [code](https://github.com/srl-ethz/osprey) (ETH Zurich)
- [2023] **A Deep Multi-Agent Reinforcement Learning Framework for Autonomous Aerial Navigation to Grasping Points on Loads** · *Robotics and Autonomous Systems* [paper](https://www.sciencedirect.com/science/article/pii/S0921889023001288) [pdf](https://eprints.whiterose.ac.uk/id/eprint/232609/1/1-s2.0-S0921889023001288-main.pdf) (Coventry University)

*UAV-only (no manipulator):*

- [2026] **RAPTOR: A Foundation Policy for Quadrotor Control** · *Science Robotics* [paper](https://doi.org/10.1126/scirobotics.aec1481) (NYU) ✦ *Giuseppe Loianno* 🛸UAV — *flight-level foundation policy: the base skill future UAM policies can build on*
- [2026] **AgilePE: Autonomous UAV Pursuit-Evasion via Self-Play Reinforcement Learning** · *arXiv* [paper](https://arxiv.org/abs/2608.14135) (Shanghai Jiao Tong University) 🛸UAV — *self-play pursuit-evasion: adversarial flight skill with sim-to-real transfer*
- [2026] **FLARE: Agile Flights for Quadrotor Cable-Suspended Payload System via Reinforcement Learning** · *IEEE RA-L* [paper](https://doi.org/10.1109/LRA.2026.3662598) 🛸UAV — *RL agility for cable-suspended payload flight: load dynamics without an arm*
- [2023] ⭐ **Champion-Level Drone Racing Using Deep Reinforcement Learning (Swift)** · *Nature* [paper](https://www.nature.com/articles/s41586-023-06419-9) (University of Zurich) ✦ *Davide Scaramuzza* 🛸UAV — *sim-to-real RL landmark for the flight stack every UAM builds on*

### <a id="vla"></a>Language-Grounding & VLA

- [2026] **AIR-VLA: Vision-Language-Action Systems for Aerial Manipulation** · *arXiv* [paper](https://arxiv.org/abs/2601.21602) [code](https://github.com/SpencerSon2001/AIR-VLA) (Institute of Automation, Chinese Academy of Sciences)
- [2026] **AIR-VLA+: Decoupling Movement and Manipulation via Cascaded Dual-Action Decoders with Asymmetric MoE for Aerial Robots** · *arXiv* [paper](https://arxiv.org/abs/2606.12859) (Institute of Automation, Chinese Academy of Sciences)
- [2026] **AeroManip-VLA: Scalable Vision-Language-Action Learning for Aerial Manipulation with RL-Generated Demonstrations** · *arXiv* [paper](https://arxiv.org/abs/2609.36915) — *RL-generated demonstrations scale up VLA training for aerial manipulation*
- [2026] **π, But Make It Fly: Physics-Guided Transfer of VLA Models to Aerial Manipulation** · *arXiv* [paper](https://arxiv.org/abs/2603.25038) ✦ *Allen Z. Ren* — *physics-guided residual transfer of π-family VLAs onto flying arms*
- [2026] **Fly-by-Code: Embodied Coding Agents for Aerial Manipulation with Active Visual and Physical Feedback** · *arXiv* [paper](https://arxiv.org/abs/2610.12549) — *LLM coding agents close the loop with active visual/physical feedback*
- [2026] **From Local Whole-Body VLA Behaviors to Scene-Scale Aerial Manipulation** · *arXiv* [paper](https://arxiv.org/abs/2609.39670) (Nanyang Technological University)
- [2026] **AERMANI-PLACE: Language Guided Object Placement with Aerial Manipulators** · *CASE* [paper](https://doi.org/10.1109/CASE69030.2026.11704177) (University of Manchester) ✦ *Wei Pan*

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
- [2021] **Design, Sensing, and Control of a Novel UAV Platform for Aerial Drilling and Screwing** · *IEEE RA-L* [paper](https://doi.org/10.1109/LRA.2021.3062305) (Sun Yat-sen University) — *integrated aerial drilling & screwing platform*
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

⭐ = must-read · ✦ = paper from a renowned team / with a renowned co-author · 🛸UAV = aerial-robot paper without a manipulator, kept for its role in the UAM stack (placed at the end of each subsection). Papers without an open-access copy link to the publisher page only.

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
