## Language Resources

### Overview

The following language resources are deliverables from the Icelandic Language Technology
Programme 2018-2022 (LT-Programme).

They are categorized into the following groups:

* [Monolingual text corpora](#monolingual-text-corpora)
* [Morphological resources](#morphological-resources)
* [Part-of-Speech (PoS) tagging and parsing corpora](#part-of-speech-pos-tagging-and-parsing-corpora)
* [Pronunciation tools and dictionaries](#pronunciation-tools-and-dictionaries)
* [Word semantics and embeddings](#word-semantics-and-embeddings)

---

## Monolingual text corpora

### Icelandic Gigaword Corpus (IGC)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)  
**License (parts):** [Custom (MÍM)](https://igc.arnastofnun.is/index.html#Licencing)  
**Type:** Dataset  
**Description:** The IGC-project (Icelandic Gigaword Corpus) aims to collect as much as possible of Icelandic texts that can be published, under an open or restricted licence. The project is divided into nine individual corpora. Each corpus comes in two versions. One contains the texts untokenized and untagged where each paragraph is contained inside of a `<p>` tag, while the other one has been tokenized, POS-tagged and lemmatized.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/254),
[Website](https://igc.arnastofnun.is/is/index.html)  
**Last update:** 2022

### Icelandic Crawled Corpus (ICC)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** The Icelandic Crawled Corpus (ICC) contains approximately 930M tokens which have been scraped from a selection of Icelandic websites, including news sites, government websites and forums. The scraped text is presented in its original form, unannotated, untokenized and without deduplication.  
**Location:** [HuggingFace](https://huggingface.co/datasets/jonfd/ICC)  
**Last update:** 2022  
*Comment/TBD: Move to Icelandic-LT HuggingFace site*

---

## Morphological resources

### DMII/BÍN
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC_BY--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)  
**Type:** Dataset  
**Description:** This package contains the Comprehensive Format of The Database of Modern Icelandic Inflection - (DMII). DMII is a part of The Database of Icelandic Morphology (DIM). DIM is a multipurpose linguistic resource, created for use in language technology (LT), as a reference for the general public in Iceland, and for use in research on the Icelandic language.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/162), [Website](https://bin.arnastofnun.is/DMII/)  
**Last update:** October 2021

### Valency Structure Database
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC_BY--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)  
**Type:** Dataset  
**Description:** This package contains valency structures that are part of The Database of Icelandic Morphology (DIM) which is a multipurpose linguistic resource, created for use in language technology (LT), as a reference for the general public in Iceland, and for use in research on the Icelandic language.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/163), [Website](https://bin.arnastofnun.is/DMII/LTdata/DIM-valency/)  
**Last update:** September 2021

### DMII Abbreviations
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC_BY--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)  
**Type:** Dataset  
**Description:** A list of common abbreviations in Icelandic texts, with explanations and classification.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/164), [Website](https://bin.arnastofnun.is/DMII/LTdata/DIMabbr/)  
**Last update:** October 2021

### Icelandic Hyphenation Dictionary
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** A hyphenated word list for Icelandic, and hyphenation patterns derived therefrom, based on data from Icelandic dictionaries and texts.  
**Location:** [GitHub](https://github.com/icelandic-lt/hyphenation-is), [CLARIN-IS](http://hdl.handle.net/20.500.12537/86)  
**Last update:** 2020

---

## Part-of-Speech (PoS) tagging and parsing corpora

### MIM-GOLD
**License:** [Custom (MÍM)](https://repository.clarin.is/repository/xmlui/page/license-mim-gold)  
**Type:** Dataset  
**Description:** MIM-GOLD 21.05 is a gold standard for PoS-tagging and lemmatizing Icelandic texts. This new version contains the same texts as version 20.05 but lemmas have been added and some corrections have been made to the PoS-tagging. The gold standard contains approximately 1 million running words with manually annotated PoS-tags and lemmas.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/113), [CLARIN-IS (train/test set)](http://hdl.handle.net/20.500.12537/114)  
**Last update:** June 2021

### GreynirCorpus
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** Training corpus for constituency parsing and PoS tagging.
The treebank consists of 10 million parsed sentences containing approximately
140 million words.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/119), [GitHub](https://github.com/icelandic-lt/GreynirCorpus)  
**Last update:** 2021

### Icelandic Frequency Dictionary Train/Test
**License:** [Custom (IFD)](https://repository.clarin.is/repository/xmlui/page/license-frequency-dictionary)  
**Type:** Dataset  
**Description:** Testing and training sets for PoS tagging from IFD 2020.05 (Icelandic Frequency Dictionary) which contains fragments from 100 texts, published between the years 1980 and 1989.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/38)  
**Last update:** 2020

---

## Pronunciation tools and dictionaries

### Pedi
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)  
**Type:** Software  
**Description:** Pedi is a web application to read, edit and export pronunciation dictionaries. It has been used to create the Icelandic Pronunciation Dictionary.  
**Location:** [GitHub](https://github.com/icelandic-lt/pedi)  
**Last update:** May 2024

### Icelandic Pronunciation Dictionary
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** The Icelandic Pronunciation Dictionary contains manually revised transcriptions in four pronunciation variants of Icelandic: the standard pronunciation, the northern post-aspiration variant ("harðmæli"), the north-eastern variant post-aspiration + voiced pronunciation, and the southern hv-variant.  
**Location:** [GitHub](https://github.com/icelandic-lt/iceprondict), [CLARIN-IS](http://hdl.handle.net/20.500.12537/154)  
**Last update:** October 2023

---

## Word semantics and embeddings

### Icelandic Wordweb
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** A single RDF file housing the Icelandic Wordweb in an LT-appropriate format. The Wordweb's features have been encoded with OntoLex and SKOS, with the new version designed in such a way as to replicate all core functionality of the original, and offer an extensive suite of new options for inspection and research.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/117)  
**Last update:** June 2021

### Icelandic Multi-SimLex
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** MSL, short for Multi-SimLex, is an evaluation protocol and associated dataset for lexical semantics. The original English-language MSL builds on several older, well-known datasets, most notably SimLex-999, and has already been released in a dozen languages. A fully processed MSL dataset consists of 1,888 unordered word pairs, where each pair is tagged with grammatical categories and marked with a numerical score that indicates the words' semantic similarity.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/121)  
**Last update:** June 2021

### IceBATS
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** IceBATS is an Icelandic adaptation of the Bigger Analogy Test Set (BATS). BATS is intended to evaluate word embeddings based on word analogy tasks. This extensive set demonstrates a language model's ability to recognize various linguistic relations with the use of the vector offset method.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/120)  
**Last update:** June 2021
