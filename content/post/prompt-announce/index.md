---
title: Prompt-based Learning for Clinical Natural Language Processing
date: 2022-05-12
image:
  focal_point: "top"
author: dwj
---

Led by Niall Taylor and Yi Zhang, a new [paper](/publication/taylor2022/) on [prompt-based](https://en.wikipedia.org/wiki/Prompt_engineering) learning for clinical support tasks. 

A major concern in the field of Natural Language Processing (NLP) is that even the largest pre-trained language models, such as GPT-3, do not perform well on specialized domains such as clinical texts. Typically to adapt large PLMs to new domains requires fine-tuning entire models on new texts and downstream tasks, which can require entire fleets of high-end GPUs that are often only available to commercial enterprises.  Prompt learning is a new paradigm of NLP to fully utilize the pretrained language model based on its pretraining task and can require substantially fewer training parameters given a new task.

In this work, we have investigated the feasibility of using prompt learning with small or medium domain trained frozen language models versus "a traditional" fine-tuning on clinical tasks using MIMIC-III data with full-data and few-shot settings. We also develop a new clinical triage task based on the ICD-9 codes, available for future use.

We demonstrated that prompt learning requires fewer tuned parameters to match  and even outperform traditional fine-tuning in few-shot settings. We actually observed prompt learning could match the performance of traditional fine-tuning with 1000 times fewer trained parameters. This is particularly encouraging for high-stake domains, such as medicine, where high-quality annotated data is scarce.

Prompt tuning can offer a competitive alternative to the fine-tuning of large language models in the medical domain and act as a framework moving forward. 




