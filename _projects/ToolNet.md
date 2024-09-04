---
title: "ToolNet: Connecting Large Language Models With Massive Tools"
collection: publications
authors: 'Xukun Liu, Zhiyuan Peng, DK Xu'
permalink: /publication/2024-toolnet
excerpt: 'We introduce ToolNet, a plug-and-play method to assists LLMs in handling massive tools. ToolNet organizes tools in a weighted directed graph (node represents tools and edges denote tool transition) based on the tool-use trajectories produced by LLMs. An LLM navigates in the graph by iteratively choosing the next one from its successors until the task is resolved. Graphs are updated online, enabling adjustment to accommodate the frequent updates of tools and new tasks.'
date: 2024-02-29
paperurl: 'https://arxiv.org/abs/2403.00839'
img: '/images/toolnet.png'
---
We introduce ToolNet, a plug-and-play method to assists LLMs in handling massive tools. ToolNet organizes tools in a weighted directed graph (node represents tools and edges denote tool transition) based on the tool-use trajectories produced by LLMs. An LLM navigates in the graph by iteratively choosing the next one from its successors until the task is resolved. Graphs are updated online, enabling adjustment to accommodate the frequent updates of tools and new tasks.
![toolnet](/images/toolnet.png)
