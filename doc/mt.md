## Machine Translation

### Overview

`to be done`

Our projects are categorized into:

* [Datasets](#datasets)
* [Models](#models)
* [Training Code](#training-code)
* [Software](#software)

---

## Datasets

### Classification training set

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** This is a training set for a classifier, using one or more of the following scores to select good quality parallel segments in comparable corpora or for filtering parallel corpora: LASER, LaBSE and WAScore.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/152)  

### EN-IS/IS-EN Glossary

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** This package contains an Icelandic-English/English-Icelandic glossary. The glossary contains 232.950 Icelandic-English pairs.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/144)  

### Idiomatic expressions

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** The file contains 1000 Icelandic idioms processed from the ISLEX database of The Árni Magnusson Institute for Icelandic studies. They are listed with their English idiomatic equivalent and literal meaning in both languages, as well as example sentences and keywords.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/275)  

### Long Context Synthetic Translation Pairs

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** Backtranslation corpus  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/260)  

### Parallel Named Entity test corpus

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** This repository contains a test set for measuring the progress in Named-Entity (NE) translation between Icelandic and English. This is parallel data which has been NER-tagged with language specific NE-taggers.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/130)  

### ParIce

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** A realigned and refiltered version of the ParIce corpus, with additional material.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/145)  

### ParIce Dev/Test

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** This package contains test/dev sets with paralleled segments in English and Icelandic.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/146)  

### Semi-synthetic parallel name robustness corpus

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** A semi-synthetic parallel corpus, based on the ParIce corpus. Person names have been identified in both source and target sentences in each pair. They are then replaced with other names of the same gender and having the same declension, sourced from news articles.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/74)  

### Synthetic parallel corpus

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** Synthetic back-translated training corpus for neural machine translation. An mBART25 finetuned on English-Icelandic data created the corpus by translating Icelandic and English sentences.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/127)  

### Synthetic Parallel Astronomy Corpus

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** Synthetic parallel corpus (Icelandic-English) with astronomy terms injected into university abstracts (IPAC, https://arxiv.org/pdf/2108.05289v1.pdf  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/135)  

### Test set for parallel sentence extraction

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** This is a BUCC-style dataset for testing the accuracy of parallel sentence extraction from comparable corpora. It has 100 thousand sentences, of which 2000 are parallel pairs, and the other 98 thousand for each language randomly selected sentences from the same domain (news).  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/151)  

### Test set for sentence alignment

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** This package contains 10 documents in Icelandic and English, with text segments aligned manually on sentence level, in order to be used for testing and comparing alignment methods.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/150)  

### Translation of institutions, companies, and titles

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** This package contains 3,853 translations of institutions (domestic and international), companies, titles (governmental and registered job-titles).  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/184)  

### WMT21 data

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** Development and test data for the Icelandic-English language pair in the WMT21 Shared Task: Machine Translation of News.  
**Location:** [GitHub](https://github.com/icelandic-lt/WMT21-data)  

---

## Models

### GreynirTranslate

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** General domain IS-EN and EN-IS translation models based on a multilingual BART model  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/125)  

### GreynirTranslate (with layer-drop)

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Inference optimized version of GreynirTranslate with 40% layer drop with lower translation performance  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/128)  

### Long Context Translation Models

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Model for translating between English and Icelandic, in both directions  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/278)  

### mBART25 NMT-models

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** General domain IS-EN and EN-IS translation models based on a multilingual BART model  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/125)  

### Optimized Long Context Translation Models

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Inference optimized version of Long Context Translation Models with lower translation performance  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/283)  

### Semi-supervised Icelandic-Polish MT system

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** This Icelandic-Polish translation model (bi-directional) was trained using fairseq (https://github.com/facebookresearch/fairseq) by means of semi-supervised translation by starting with the mBART50 model.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/259)

---

## Training Code

| Training Code    | Description                                      | Location                                                   |
|------------------|--------------------------------------------------|------------------------------------------------------------|
| MT Model Scripts | Training code for all machine translation models | [GitHub](https://github.com/icelandic-lt/mt-model-scripts) |

---

## Software

| Software                               | Description | Location |
|----------------------------------------|-------------|----------|
| Chrome translation plugin              | A Chrome plugin for translating web pages | [GitHub](https://github.com/icelandic-lt/GreynirTranslateChromePlugin) |
| GreynirSeq                             | Natural language parsing toolkit for Icelandic focused on sequence modeling with neural networks | [GitHub](https://github.com/icelandic-lt/greynirseq) |
| GreynirSeq Domain Translation Pipeline | Domain Translation Pipeline built on Fairseq and mBART-derived translation models | [GitHub](https://github.com/icelandic-lt/domain-translation-pipeline), [CLARIN-IS](http://hdl.handle.net/20.500.12537/212) |
| GreynirT2T                             | Program library for training English-Icelandic neural machine translation systems, built on top of Tensor2Tensor and Tensorflow | [GitHub](https://github.com/icelandic-lt/GreynirT2T), [CLARIN-IS](http://hdl.handle.net/20.500.12537/71) |
| GreynirTerms                           | Utility program for generating synthetic parallel corpora of English and Icelandic sentences that contain rare terms | [GitHub](https://github.com/icelandic-lt/GreynirTerms) |
| Moses PBSMT                            | Moses phrase-based statistical machine translation is a system for developing and running statistical machine translations. | [GitHub](https://github.com/icelandic-lt/SMT) |
| MT-NE-Pipeline                         | Named Entity processing pipeline | [GitHub](https://github.com/icelandic-lt/MT-NE-Pipeline) |
| nnserver                               | Code to serve models trained with GreynirT2T | [GitHub](https://github.com/icelandic-lt/nnserver), [CLARIN-IS](http://hdl.handle.net/20.500.12537/72) |
| Velthyding                             | Web application frontend for Google Translate V3 compatible backends | [GitHub](https://github.com/icelandic-lt/Velthyding), [CLARIN-IS](http://hdl.handle.net/20.500.12537/23) |