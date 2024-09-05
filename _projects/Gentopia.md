---
title: "Gentopia.AI"
collection: projects
permalink: /projects/gentopia
excerpt: 'Gentopia is a lightweight and extensible framework for LLM-driven Agents and ALM research. It provides essential components to build, test and evaluate agents. At its core, Gentopia aims to assemble an agent with a single config, thus minimizing your effort in building, tuning, and sharing agents.'
date: 2024-6-27
img: '/images/gentopia.png'
tags: ['Large Language Model(LLM)', 'Retrieval-Augmented Generation(RAG)', 'Agent', 'Tool Call']
---

Gentopia is a lightweight and extensible framework for LLM-driven [Agents](https://lilianweng.github.io/posts/2023-06-23-agent/) and [ALM](https://arxiv.org/abs/2302.07842)  research. It provides essential components to build, test and evaluate agents. At its core, Gentopia aims to assemble an agent with a single config, thus minimizing your effort in building, tuning, and sharing agents. 

![Genopia](/images/gentopia.png)


Gentopia maintains an agent platform [GentPool](https://github.com/Gentopia-AI/GentPool) to share specialized agents, where your agent *interacts* with other agents by cloning, hierarchical plug-in, or sharing environment. We provide a unique agent [benchmark](https://gentopia.readthedocs.io/en/latest/gentpool.html#agent-evaluation) for holistic evaluation. 

## Motivation 🧠
Agent practitioners start to realize the difficulty in tuning a "well-rounded" agent with tons of tools or instructions in a single layer.
Recent studies like [TinyStories](https://arxiv.org/abs/2301.12726), [Specializing Reasoning](https://arxiv.org/abs/2301.12726), [Let's Verify SbS](https://arxiv.org/abs/2305.20050), [ReWOO](https://arxiv.org/abs/2305.18323), etc. also point us towards an intuitive yet undervalued direction 👉 

```
An LLM is more capable if you create a context/distribution shift specialized to some target tasks.
```
Sadly, there is no silver bullet for agent specialization. For example, you can 
- Simply add `Let's think step by step.` in your **prompt** for more accurate Math QA.
- Give a **few-shot** exemplar in your prompt to guide a better reasoning trajectory for novel plotting.
- Supervise **fine-tuning** (SFT) your 70B `llama2` like [this](https://arxiv.org/abs/2305.20050) to match reasoning of 175B GPT-3.5.
- Tune your agent **paradigm** like this [demo](https://www.youtube.com/watch?v=diJ4IDaT4Z4) to easily half the execution time for Seach & Summarize.
- And more ...

Isn't it beautiful if one shares his effort in specialized intelligence, allowing others to reproduce, build on, or interact with it? 🤗 This belief inspires us to build Gentopia, 
**designed for agent *specialization, sharing, and interaction,* to stackingly achieve collective growth towards greater intelligence.**.

## Core Features 💡

- ⚙️ Config-driven agent assembling and chat.
- 🚀 Large amount of prebuilt agent types, LLM clients, tools, memory systems, and more.
- 🪶 Lightweight and highly extensible implementation of essential components.
- 🧪 Aligning with state-of-the-art AI research.
- 🤝 Enabling multi-agent interactions.
- 🦁 Unique platform of agent zoo and eval benchmark.


🌟 Highlight Topics 🌟 
- [🤖 Agent Templates](https://gentopia.readthedocs.io/en/latest/quick_start.html#vanilla-agent)
- [⛰️ Hierarchical Agents](https://gentopia.readthedocs.io/en/latest/agent_components.html#agent-as-plugin)
- [🥇 Unique Agent Benchmark](https://gentopia.readthedocs.io/en/latest/gentpool.html#agent-evaluation)
- [🦙 Open LLM Supports](https://gentopia.readthedocs.io/en/latest/agent_components.html#huggingface-open-llms)
- [🧠 High-Performance Memory](https://gentopia.readthedocs.io/en/latest/agent_components.html#long-short-term-memory)

## News 👷

**[Oct 7]** The companion paper was accepted by #EMNLP 23. See you in Singapore! 🦙🌎

**[Aug 6]** We've submitted our work as a paper for EMNLP 2023. Special thanks to the research [team](https://gentopia-ai.github.io/Gentopia-AI-Homepage/#about) and professors from NCSU, GMU, and CMU for collaboration :)
