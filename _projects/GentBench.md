---
title: "GentBench"
collection: projects
permalink: /projects/gentbench
excerpt: 'Benchmark and Evaluation for Gentopia.'
date: 2024-6-27
img: '/images/gentopia.png'
tags: ['Large Language Model(LLM)', 'Retrieval-Augmented Generation(RAG)', 'LLM Evaluation', 'Benchmark']
---

Benchmark and Evaluation for Gentopia.

A good ALM Benchmark should aim to solve problems and tasks hard/unsolvable by LLMs (else there's no meaning to pay tool tax).

Tasks in Gentbench will be half-public and half-private. We open-source a demonstrative public benchmark to encourage agent tuning, but will use a private bench (of similar distribution) for fair eval.

![image](https://github.com/Gentopia-AI/GentBench/assets/65674752/d5b3553c-9787-4ff2-a282-ac0fd471454e)


## Eval Tasks
We are still expanding! Check `./gentbench/benchmark/public/` for some available public benchmarks.
```
Reasoning
 - Math 
 - Coding
 - Planning
 - Commonsense

Knowledge
 - World_Knowledge (Offline)
 - Domain_Specific_Knowledge (Offline)
 - Web_Retrieval (Online)

Safety
 - Integrity (Jailbreaks, Ethics, ..)
 - Harmlessness (Toxicity, Bias, ..)

Multilingual 
 - Translation
 - Understanding
Robustness
 - Consistency 
 - Resilience (Self-correct when presented with false info.

Memory 
 - Context Length
 - Accuracy

Efficiency 
 - Token usage.
 - Run time.
```


## Eval pipeline run
```
from gentopia.assembler import AgentAssembler
from gentbench.eval import EvalPipeline
import os
import dotenv

# Store OPENAI_API_KEY in .env file
dotenv.load_dotenv(".env")

eval = EvalPipeline(eval_config="gentbench/eval/config/eval_config.yaml")
agent = AgentAssembler(file="gentbench/eval/config/chatgpt.yaml").get_agent()

eval.run_eval(agent)
```
