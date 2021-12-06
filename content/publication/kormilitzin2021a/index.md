---
title: "Med7: a transferable clinical natural language processing model for electronic health records"
authors: 
- ak
- "Nemanja Vaci"
- "Liu Qiang"
- anh

date: "2021-11-15T00:00:00Z"
doi: "https://doi.org/10.1016/j.artmed.2021.102086"

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

abstract: "Electronic health record systems are ubiquitous and the majority of patients’ data are now being collected electronically in the form of free text. Deep learning has significantly advanced the field of natural language processing and the self-supervised representation learning and the transfer learning have become the methods of choice in particular when the high quality annotated data are limited. Identification of medical concepts and information extraction is a challenging task, yet important ingredient for parsing unstructured data into structured and tabulated format for downstream analytical tasks. In this work we introduced a named-entity recognition (NER) model for clinical natural language processing. The model is trained to recognise seven categories: drug names, route of administration, frequency, dosage, strength, form, duration. The model was first pre-trained on the task of predicting the next word, using a collection of 2 million free-text patients’ records from MIMIC-III corpora followed by fine-tuning on the named-entity recognition task."
# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- NLP
- Med7
- Medication extraction
- EHR
- Named entity recognition (NER)

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

