---
title: "Named entity recognition in electronic health records using transfer learning bootstrapped Neural Networks"
authors: 
- "Luka Gligic"
- ak
- "Paul Goldberg"
- anh

date: "2021-11-15T00:00:00Z"
doi: "https://doi.org/10.1016/j.neunet.2019.08.032"

# Schedule page publish date (NOT publication's date).
publishDate: "2021-11-14T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
# publication: ""
publication_short: ""

abstract: "Neural networks (NNs) have become the state of the art in many machine learning applications, such as image, sound (LeCun et al., 2015) and natural language processing (Young et al., 2017; Linggard et al., 2012). However, the success of NNs remains dependent on the availability of large labelled datasets, such as in the case of electronic health records (EHRs). With scarce data, NNs are unlikely to be able to extract this hidden information with practical accuracy. In this study, we develop an approach that solves these problems for named entity recognition, obtaining 94.6 F1 score in I2B2 2009 Medical Extraction Challenge (Uzuner et al., 2010), 4.3 above the architecture that won the competition. To achieve this, we bootstrap our NN models through transfer learning by pretraining word embeddings on a secondary task performed on a large pool of unannotated EHRs and using the output embeddings as a foundation of a range of NN architectures. Beyond the official I2B2 challenge, we further achieve 82.4 F1 on extracting relationships between medical terms using attention-based seq2seq models bootstrapped in the same manner."

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- Neural Networks
- NLP
- Named entity recognition
- NER
- Electronic health records
- EHR
- Transfer learning
- LSTM

featured: false

links:
#- name: Custom Link
#  url: http://example.org
url_pdf: 
# url_code: '#'
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

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides:
---

