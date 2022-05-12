---
title: "Clinical Prompt Learning with Frozen Language Models"
authors: 
- nt
- "Yi Zhang"
- dwj
- anh
- ak

date: "2022-05-11T00:00:00Z"
doi: "https://arxiv.org/abs/2205.05535"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-05-11T18:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
# publication: "Rationale production to support clinical decision-making"
publication_short: ""

abstract: Prompt learning is a new paradigm in the Natural Language Processing (NLP) field which has shown impressive performance on a number of natural language tasks with common benchmarking text datasets in full, few-shot, and zero-shot train-evaluation setups. Recently, it has even been observed that large but frozen pre-trained language models (PLMs) with prompt learning outperform smaller but fine-tuned models. However, as with many recent NLP trends, the performance of even the largest PLMs such as GPT-3 do not perform well on specialized domains (e.g. medical text), and the common practice to achieve State of the Art (SoTA) results still consists of pre-training and fine-tuning the PLMs on downstream tasks. The reliance on fine-tuning large PLMs is problematic in clinical settings where data is often held in non-GPU environments, and more resource efficient methods of training specialized domain models is crucial. We investigated the viability of prompt learning on clinically meaningful decision tasks and directly compared with more traditional fine-tuning methods. Results are partially in line with the prompt learning literature, with prompt learning able to match or improve on traditional fine-tuning with substantially fewer trainable parameters and requiring less training data. We argue that prompt learning therefore provides lower computational resource costs applicable to clinical settings, that can serve as an alternative to fine-tuning ever increasing in size PLMs.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- NLP
- MIMIC
- Prompt-based Learning
- Clinical AI

featured: false

links:
#- name: Custom Link
#  url: http://example.org
url_pdf: https://arxiv.org/abs/2205.05535
url_code: 'https://github.com/NtaylorOX/Public_Clinical_Prompt'
# url_dataset: '#'
# url_poster: '#'
# url_project: ''
# url_slides: ''
# url_source: '#'
# url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
#  focal_point: ""
#  preview_only: false
---

