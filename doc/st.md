## Support Tools

### Overview

Support Tools are general NLP tools (tokenizers, taggers, parsers) that are often used as part of LT pipelines.<br>
Additionally, this category also includes Icelandic language models under the BERT and Electra architectures. Language models are very time-consuming to train and often require large amounts of text data. The models developed here are provided as pre-trained models and can be used for various downstream tasks, such as Named Entity Recognition (NER), Part-of-Speech (PoS) Tagging, etc.

How well these models perform on Icelandic can be seen in the [IceEval results](https://github.com/icelandic-lt/IceEval/blob/master/doc/results.md).<br>
You can also find general training scripts for these models in the [IceEval repository](https://github.com/icelandic-lt/IceEval), for using these language models to train on your own data.

Our projects are categorized into:

* [Models](#models)
* [Software](#software)

---

## Models

### Biaffine-based UD Parser

[![Apache-2.0 License](https://img.shields.io/badge/License-Apache--2.0-blue)](https://opensource.org/licenses/Apache-2.0) 
**Type:** Model  
**Description:** Universal Dependencies parser for Icelandic trained with Diaparser  
**Location:** [Clarin.is](http://hdl.handle.net/20.500.12537/302), [HuggingFace](https://huggingface.co/Icelandic-lt/biaffine_parser)  

### COMBO-based UD Parser

[![Apache-2.0 License](https://img.shields.io/badge/License-Apache--2.0-blue)](https://opensource.org/licenses/Apache-2.0)   
**Type:** Model  
**Description:** Universal Dependencies parser for Icelandic trained with COMBO  
**Location:** [Clarin.is](http://hdl.handle.net/20.500.12537/301), [HuggingFace](https://huggingface.co/Icelandic-lt/combo_parser)  

### ConvBert base

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Icelandic Language Model with 106.9 mio. parameters, suitable for downstream tasks like Embedding generation, named entity generation (NER), Part of Speech (PoS) tagging, etc. For an evaluation of this model, see [IceEval results](https://github.com/icelandic-lt/IceEval/blob/master/doc/results.md).  
**Location:** [HuggingFace](https://huggingface.co/Icelandic-lt/convbert-base-igc-is)

### ConvBert small

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Icelandic Language Model with 21.52 mio. parameters, suitable for downstream tasks like Embedding generation, named entity generation (NER), Part of Speech (PoS) tagging, etc.  For an evaluation of this model, see [IceEval results](https://github.com/icelandic-lt/IceEval/blob/master/doc/results.md).  
**Location:** [HuggingFace](https://huggingface.co/Icelandic-lt/convbert-small-igc-is)

### Electra base

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Icelandic Language Model with 110.11 mio. parameters, suitable for downstream tasks like Embedding generation, named entity generation (NER), Part of Speech (PoS) tagging, etc.  For an evaluation of this model, see [IceEval results](https://github.com/icelandic-lt/IceEval/blob/master/doc/results.md).  
**Location:** [HuggingFace](https://huggingface.co/Icelandic-lt/electra-base-igc-is)

### Electra small

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Icelandic Language Model with 13.69 mio. parameters, suitable for downstream tasks like Embedding generation, named entity generation (NER), Part of Speech (PoS) tagging, etc. For an evaluation of this model, see [IceEval results](https://github.com/icelandic-lt/IceEval/blob/master/doc/results.md).  
**Location:** [HuggingFace](https://huggingface.co/Icelandic-lt/electra-small-igc-is)

### Neural constituency Parser

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Experimental variant of the Berkeley neural parser architecture  
**Location:** [Clarin.is](http://hdl.handle.net/20.500.12537/149), [HuggingFace](https://huggingface.co/Icelandic-lt/neural_parser)  

---

## Software

| Project name | Description | Location |
|--------------|-------------|----------|
| ABLTagger | A Part-of-Speech (PoS) tagger and lemmatizer for Icelandic in Python. | [GitHub](https://github.com/icelandic-lt/POS)<br>[Clarin.is](http://hdl.handle.net/20.500.12537/115)<br>[Clarin.is](http://hdl.handle.net/20.500.12537/134) |
| Alexia | Lexicon Acquisition Tool in Python. ALEXIA is a command-line based corpus tool used for comparing a certain vocabulary to that of a larger corpus or corpora. | [GitHub](https://github.com/icelandic-lt/ALEXIA_ordtokutol)<br>[Clarin.is](http://hdl.handle.net/20.500.12537/123) |
| Embeddings generation | Scripts for generation of embeddings for the Icelandic language via word2vec, fastText, GloVe including scripts to evaluate trained models | [GitHub](https://github.com/icelandic-lt/ordgreypingar_embeddings) |
| GreynirEngine | Python package for working with Icelandic natural language text. Greynir can parse text into sentence trees, find lemmas, inflect noun phrases, assign part-of-speech tags and much more. | [GitHub](https://github.com/icelandic-lt/GreynirEngine)<br>[Clarin.is](http://hdl.handle.net/20.500.12537/269) |
| Icelandic NER API | A dockerized Named Entity Recognition (NER) API for Icelandic using Icelandic language models. | [GitHub](https://github.com/icelandic-lt/Icelandic-NER-API)<br>[Clarin.is](http://hdl.handle.net/20.500.12537/159)<br>[Clarin.is](http://hdl.handle.net/20.500.12537/118) |
| IceEval | Benchmark for evaluating and comparing the quality of pre-trained language models. The models are evaluated on a selection of four NLP tasks for Icelandic. | [Clarin.is](http://hdl.handle.net/20.500.12537/297) |
| IceParser | Shallow parser for Icelandic written in Java. The parser comprises a sequence of finite-state transducers, which add syntactic information, in an incremental manner, into the input text. | [GitHub](https://github.com/icelandic-lt/icenlp)<br>[Clarin.is](http://hdl.handle.net/20.500.12537/122) |
| Íslenska | Python module that embeds the vocabulary of the Database of Icelandic Morphology (Beygingarlýsing íslensks nútímamáls, BÍN) and offers various lookups and queries of the data. | [GitHub](https://github.com/icelandic-lt/BinPackage) |
| Skiptir | A command-line tool that uses Pyphen (https://pyphen.org) to hyphenate text according to the newest hyphenation patterns from the Icelandic Hyphenation Dictionary. | [GitHub](https://github.com/icelandic-lt/skiptir)<br>[Clarin.is](http://hdl.handle.net/20.500.12537/87) |
| Tokenizer | Python executable program and module for tokenizing Icelandic text. It converts input text to streams of tokens, where each token is a separate word, punctuation sign, number/amount, date, e-mail, URL/URI, etc. | [GitHub](https://github.com/icelandic-lt/Tokenizer)<br>[Clarin.is](http://hdl.handle.net/20.500.12537/262) |
| UDConverter | Python module for converting bracket-parsed PPCHE-format treebanks to the Universal Dependencies framework. The module is specifically configured to convert treebanks in the IcePaHC format, which is based on PPCME. | [GitHub](https://github.com/icelandic-lt/UDConverter) |
| UDConverter-GreynirCorpus | Tool for converting the constituency treebanks of GreynirCorpus to dependency treebanks following the Universal Dependencies framework | [GitHub](https://github.com/icelandic-lt/UDConverter-GreynirCorpus)<br>[Clarin.is](http://hdl.handle.net/20.500.12537/222) |
