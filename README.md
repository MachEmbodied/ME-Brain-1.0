<p>
  <img src="assets/machembodied.svg" alt="MachEmbodied" width="360">
</p>

<h3 align="center">ME-Brain-1.0: Memory, Cognition, and Action for Self-Evolving Embodied Intelligence</h3>

<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/arXiv-Tech_Report-B31B1B?style=flat-square&amp;logo=arxiv&amp;logoColor=white" alt="Tech Report" height="16"></a>
  &nbsp;
  <a href="https://machembodied.com/ME-Brain/ME-Brain-1.0.html"><img src="https://img.shields.io/badge/Project-Page-057568?style=flat-square&amp;logo=googlechrome&amp;logoColor=white" alt="Project Page" height="16"></a>
</p>

<!-- Tech Report: replace href="#" once the public URL is finalized. -->

## About

**ME-Brain-1.0** is a self-evolving embodied intelligence framework. It brings together Evolvable Memory, Cognition Core, and Action Model in a closed loop action execution → experience acquisition → experience evolution → action execution, enabling robots to autonomously improve through physical interaction without model retraining.

![ME-Brain overview: Evolvable Memory, Cognitive Core, and Action Model](assets/ME-Brain-overview.png)

Long-horizon tasks require robots to understand the current scene, remember previous interactions, and revise their plans when conditions change or execution stalls. ME-Brain addresses these needs through three cooperating modules:

- **Evolvable Memory** organizes visual observations, actions, and task states into structured, hierarchical memories, distilling execution records into reusable knowledge across tasks.
- **Cognition Core** combines physical understanding with multimodal agent reasoning to decompose tasks, invoke tools and skills, verify outcomes, and replan after failures. It also draws on human demonstrations and accumulated experience to develop reusable skills.
- **Action Model** focuses on key interaction events, using relevant history and local future predictions to generate actions. Execution trajectories feed back into memory, connecting physical interaction with subsequent decisions and skill updates.

## Videos
For more videos, visit our [Project Page](https://machembodied.com/ME-Brain/ME-Brain-1.0.html#demos).

### Grasp Anything

[![Grasp Anything animated preview](assets/videos/grasp-anything.webp)](https://machembodied.com/ME-Brain/assets/%E6%8A%93%E4%B8%87%E7%89%A9%E5%8D%81%E5%80%8D%E9%80%9F_web720p.mp4)

### Long-Horizon Task — Pour-Over Coffee


[![Real-robot coffee animated preview](assets/videos/pour-over-coffee.webp)](https://machembodied.com/ME-Brain/assets/%E6%89%8B%E5%86%B2%E5%92%96%E5%95%A1%E4%B8%9A%E5%8A%A1%E5%9C%BA%E6%99%AF%E7%9A%84%E9%95%BF%E7%A8%8B%E4%BB%BB%E5%8A%A1_web720p.mp4)



## Repository Structure

```text
ME-Brain-1.0/
├── me_brain/           # ME-Brain Core
├── robot/              # Real-robot Support
├── simulation/         # Simulation Support
├── submodule/
│   ├── Focus-VLWA/     # Action Model
│   └── ME-VLM/         # Cognition Core
├── LICENSE             # Apache 2.0 license
└── README.md
```

## News

- **2026-09-22:** Released the training and inference code for our **Action Model — [Focus-VLWA](https://github.com/MachEmbodied/Focus-VLWA)**.
- **2026-09-22:** Released our technical report.

## Todo

- [x] **Action Model — [Focus-VLWA](https://github.com/MachEmbodied/Focus-VLWA):** Training and inference code.
- [ ] **Action Model — [Focus-VLWA](https://github.com/MachEmbodied/Focus-VLWA):** Pretrained model weights.
- [ ] **Cognition Core — [MachEmbodied-VLM](https://github.com/MachEmbodied/ME-VLM).**
- [ ] ME-Brain Framework.
- [ ] ME-Brain & Simulation integration.
- [ ] ME-Brain & Real Robot integration.

## Citation
```bibtex
```

## License

ME-Brain is licensed under the [Apache License 2.0](LICENSE).
Third-party dependencies, submodules, model weights, and datasets remain subject
to their respective licenses.
