# 星语4.0

[![GitHub Repo stars](https://img.shields.io/github/stars/Yu-Yang-Li/StarWhisper?style=social)](https://github.com/Yu-Yang-Li/StarWhisper/stargazers)
[![GitHub Code License](https://img.shields.io/github/license/Yu-Yang-Li/StarWhisper)](LICENSE)
[![GitHub last commit](https://img.shields.io/github/last-commit/Yu-Yang-Li/StarWhisper)](https://github.com/Yu-Yang-Li/StarWhisper/commits/main)

<br>
        中文&nbsp ｜ &nbsp<a href="README_EN.md">English</a>&nbsp
</p>

在国家天文台-之江实验室的支持下，我们开发了星语4.0天文大模型系列，包括语言模型、时序模型、多模态模型（7B-72B）。 

## 版本更新：

1.通过清洗订正科普、科研数据飞轮得到的数据，改进训练方法，进一步提升了模型的天文物理、代码与Agent能力，开源了星语3训练集于LLM_Data目录，即将开源星语4.0权重于魔搭平台。

2.发布了[StarWhisper Pulsar](https://openreview.net/pdf?id=8SKgWpZiDL)的技术报告，一种SOTA的基于多模态大模型的脉冲星识别方法。

3.发布了[StarWhisper LC](https://spj.science.org/doi/epdf/10.34133/icomputing.0110)的技术报告，基于迁移学习、大模型的光变曲线分类方法，上传了论文相关测试代码。

<div align=center><img src="example/StarWhisper LC.png"/></div>

4.发布了[StarWhisper Telescope](https://arxiv.org/pdf/2412.06412)的技术报告，一种基于大模型智能体的望远镜控制工作流，已应用于近邻星系巡天项目。

## 效果展示

<div align=center><img src="example/图片1.png"/></div>


<div align=center><img src="example/图片2.png"/></div>


## 司天工程

司天工程是我国天文学家面向时域天文学所提出的“十五五”天文重大基础设施，一期计划在国内多个优选观测台址布置54台（18组）口径1米级的大视场望远镜，组成多波段同时监测网络，每30分钟完成1万平方度天区的高精度三色“凝视”巡天。司天的采样频率比全球其它巡天项目高近两个量级，将突破目前探测时标的限制，在新的空域和时域下发现大批新天体、新现象，在宇宙极端高能爆发源、引力波电磁对应体、系外行星和太阳系天体等理论和观测研究中形成新的突破，在“两暗一黑三起源”等重大科学问题研究以及地球文明灾难预警等国家空间安全问题方面发挥重要作用。

<div align=center><img src="example/sitian.png"/></div>

其中司天"大脑"作为数据智能处理中枢，需要适配于天文的AI工具。StarWhisper作为其备选方案，在使用大模型整合天文知识的同时，探索多模态解决具体天文问题的可能性。
## 许可证信息

项目源码遵从Apache-2.0 license，Qwen Chat的模型权重使用需遵从相应许可。

## To do list

<div align=center><img src="example/Starwhisper Telescope.png"/></div>

### 大语言模型（科普方式）

- 调整监督微调中，通用数据和专业数据的比例，缓解灾难性遗忘问题。
- 通过人工反馈的强化学习，进一步提升模型性能。
- 通过特定数据集微调，提升模型总结能力，进一步适配知识库。
- 完成天文知识图谱，与模型链接，进一步降低天文领域的幻觉现象。

### 专业多模态（科研工具）

- 开源在多模态微调权重。
- 进一步探索多模态模型在天文图像生成与识别上应用的可能性。


### 观测Agent（司天大脑）

- 提升模型在天文领域的编程能力。
- 在MiniSiTian/司天样机上，进行与天文环境交互的Agent探索工作。
- 考虑通过工具学习，链接天文专业工具。
- 尝试Agent相关工作，验证作为司天大脑备选方案的可行性。

## 引用
如果这篇工作对你有帮助，请引用：

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
## Star History

![Star History Chart](https://api.star-history.com/svg?repos=Yu-Yang-Li/StarWhisper&type=Date)
