# StarWhisper 4.0

[![GitHub Repo stars](https://img.shields.io/github/stars/Yu-Yang-Li/StarWhisper?style=social)](https://github.com/Yu-Yang-Li/StarWhisper/stargazers)  
[![GitHub Code License](https://img.shields.io/github/license/Yu-Yang-Li/StarWhisper)](LICENSE)  
[![GitHub last commit](https://img.shields.io/github/last-commit/Yu-Yang-Li/StarWhisper)](https://github.com/Yu-Yang-Li/StarWhisper/commits/main)  

<br>
        <a href="README.md">中文</a> &nbsp ｜ &nbsp English &nbsp
</p>

Under the support of the NAOC and ZheJiang Lab, we developed **StarWhisper 4.0**, a series of astronomical models including language models, time-series models, and multi-modal models (7B-72B).  

---

## Version Updates  

1. **Data & Training Enhancements**  
   - Improved astronomical physics, coding, and agent capabilities through refined training methods and cleaned scientific/popular science datasets.  
   - Open-sourced the **StarWhisper 3 training dataset** in the `LLM_Data` directory.  
   - StarWhisper 4.0 weights will be released on [ModelScope](https://www.modelscope.cn).  

2. **[StarWhisper Pulsar](https://openreview.net/pdf?id=8SKgWpZiDL)**  
   - Technical report on a SOTA multimodal large model for pulsar identification.  

3. **[StarWhisper LC](https://spj.science.org/doi/epdf/10.34133/icomputing.0110)**  
   - Light curve classification method based on transfer learning and large models.  
   - Test code related to the paper is uploaded.  
   <div align=center><img src="example/StarWhisper LC.png" width="600"/></div>  

4. **[StarWhisper Telescope](https://arxiv.org/pdf/2412.06412)**  
   - Agent-based telescope control workflow for the Near-Neighbor Galaxy Survey System (NGSS).  
   - Code is open-sourced in the `NGSS` directory.  
   <div align=center><img src="example/Starwhisper Telescope.png" width="600"/></div>  

5. **Virtual-GOTTA / StarWhisper 5.0+**  
   - Based on the presentation *Virtual-GOTTA: An AI-driven Virtual Sitian Project*, StarWhisper 5.0+ targets embodied intelligence for scientific telescopes.  
   - The system uses StarWhisper as an agent interface to connect alert release, station information, telescope status, and real-time response, supporting a global transient-source telescope data network and early supernova-clock candidate alerts within one day of explosion.  

---

## Demonstration  
<div align=center><img src="example/图片1.png" width="600"/></div>  
<div align=center><img src="example/图片2.png" width="600"/></div>  

---

## Sitian Project  
**Sitian** is a major astronomical infrastructure proposed by Chinese astronomers for time-domain astronomy. Phase I involves deploying **54 wide-field telescopes** (1-meter aperture, 18 groups) across multiple observation sites in China. These telescopes will form a multi-band monitoring network, enabling high-precision three-color "gaze" surveys of **10,000 square degrees** every 30 minutes. With a sampling frequency **two orders of magnitude higher** than global peers, Sitian will:  
- Discover new celestial objects/phenomena in extreme energy bursts, gravitational wave counterparts, exoplanets, and solar system bodies.  
- Address key scientific questions (e.g., dark matter, black holes, cosmic origins) and national space security (e.g., planetary defense).  

<div align=center><img src="example/sitian.png" width="600"/></div>  

As the **AI core** of Sitian's "brain," StarWhisper integrates astronomical knowledge via large models and explores multimodal solutions for domain-specific challenges.  

---

## License  
- Source code: **Apache-2.0 License**  
- Qwen Chat model weights: Subject to their respective licenses.  

---

## To-Do List  

### Large Language Model (Science Communication)  
- Optimize the ratio of general vs. domain-specific data during SFT to mitigate catastrophic forgetting.  
- Improve performance via reinforcement learning with human feedback (RLHF).  
- Enhance summarization capabilities through domain-adaptive fine-tuning.  
- Build an astronomical knowledge graph to reduce hallucinations.  

### Multi-Modal Models (Research Tools)  
- Release multimodal fine-tuning weights.  
- Explore applications in astronomical image generation and recognition.  

### Observation Agents (Sitian Brain)  
- Boost coding proficiency in astronomy.  
- Develop agents for interaction with MiniSiTian/Sitian prototypes.  
- Integrate astronomical tools (e.g., ASTROLABE, CASA) via tool learning.  
- Validate feasibility as a Sitian brain candidate.  

---

## Citation  
```BibTeX
@misc{wang2024starwhispertelescopeagentbasedobservation,
      title={StarWhisper Telescope: Agent-Based Observation Assistant System to Approach AI Astrophysicist}, 
      author={Cunshi Wang and Xinjie Hu and Yu Zhang and Xunhao Chen and Pengliang Du and Yiming Mao and Rui Wang and Yuyang Li and Ying Wu and Hang Yang and Yansong Li and Beichuan Wang and Haiyang Mu and Zheng Wang and Jianfeng Tian and Liang Ge and Yongna Mao and Shengming Li and Xiaomeng Lu and Jinhang Zou and Yang Huang and Ningchen Sun and Jie Zheng and Min He and Yu Bai and Junjie Jin and Hong Wu and Chaohui Shang and Jifeng Liu},
      year={2024},
      eprint={2412.06412},
      archivePrefix={arXiv},
      primaryClass={astro-ph.IM},
      url={https://arxiv.org/abs/2412.06412}, 
}
```

---

## Star History  
![Star History Chart](https://api.star-history.com/svg?repos=Yu-Yang-Li/StarWhisper&type=Date)
