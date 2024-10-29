## Spell Checking and Grammar Correction

### Overview

`to be done`

Our projects are categorized into:

* [Datasets](#datasets)
* [Models](#models)
* [Training Code](#training-code)
* [Software](#software)

---

## Datasets

### Grammatical Error Correction Test Set

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** The Grammatical Error Correction Test Set contains test data for spell and grammar checking with a focus on semantic analysis.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/320)  

### Nonwords

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** A list of Icelandic nonwords (1323 words) and their corrections, originating from the Icelandic Error Corpus.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/63)  

### Nonwords, systematic errors

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** A list of automatically prepared word forms (16155163 words) containing systematic errors along with their corrections.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/50)  

### Specialized Error Corpora

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** Collection of three error corpora: IceL2EC (Icelandic L2 Error Corpus), IceDEC (Icelandic Dyslexia Error Corpus), and IceCLEC (Icelandic Child Language Error Corpus).  
**Location:** [GitHub](https://github.com/icelandic-lt/iceErrorCorpusSpecialized), [CLARIN-IS (IceL2EC)](http://hdl.handle.net/20.500.12537/280), [CLARIN-IS (IceDEC)](http://hdl.handle.net/20.500.12537/281), [CLARIN-IS (IceCLEC)](http://hdl.handle.net/20.500.12537/133)  

### Taboo word list

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** A list of words in Icelandic that may be considered inappropriate, taboo and/or loaded in use or meaning.  
**Location:** [GitHub](https://github.com/icelandic-lt/iceTaboo), [CLARIN-IS](http://hdl.handle.net/20.500.12537/64)  

### Thesis testing

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** List of manually corrected items in a student thesis from https://skemman.is.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/258)  

---

## Models

### Binary error classifier

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Fine-tuned byT5-base Transformer model for error detection in natural language.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/256)

### Byte level neural correction model

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Byte-Level Neural Error Correction Model for Icelandic, fine-tuned byT5-base Transformer model for error correction.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/255)  

### GPT-SW3

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** GPT-SW3 model finetuned on Icelandic for spell and grammar checking tasks.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/326)  

### Multilabel error classifier

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Finetuned IceBert-base model with classification heads.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/183)  

### T5 Byte-Level Model

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** Byte-Level Neural Error Correction Model for Icelandic, fine-tuned byT5-base Transformer model for error correction.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/324)

---

## Training Code

| Training Code    | Description                                                        | Location                                                   |
|------------------|--------------------------------------------------------------------|------------------------------------------------------------|
| SG Model Scripts | Training code for all spell and grammar checking/correction models | [GitHub](https://github.com/icelandic-lt/sg-model-scripts) |

---

## Software

| Software                                  | Description                                                                                                                      | Location                                                                                                                      |
|-------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|
| AnySoftKeyboard                           | Version with a new autocompleter module based on finite-state-transducers (FST).                                                 | [GitHub](https://github.com/icelandic-lt/AnySoftKeyboard/tree/v1.0.0-gt), [CLARIN-IS](http://hdl.handle.net/20.500.12537/290) |
| AnySoftKeyboard / Icelandic language pack | Plugin for Icelandic language pack for the AnySoft Android Keyboard project. Now part of the main AnySoftKeyboard repository.    | [GitHub](https://github.com/AnySoftKeyboard/AnySoftKeyboard)                                                                  |
| GreynirCorrect                            | Python package and command line tool for checking and correcting various types of spelling and grammar errors in Icelandic text. | [GitHub](https://github.com/icelandic-lt/GreynirCorrect), [CLARIN-IS](http://hdl.handle.net/20.500.12537/270)                 |
| GreynirCorrect4LT                         | Slightly adapted version of GreynirCorrect package for use in a text-to-speech text pre-processing pipeline.                     | [GitHub](https://github.com/icelandic-lt/GreynirCorrect4LT)                                                                   |
| IceGrams                                  | Python 3 package that encapsulates a large trigram library for Icelandic.                                                        | [GitHub](https://github.com/icelandic-lt/Icegrams), [CLARIN-IS](http://hdl.handle.net/20.500.12537/80)                        |
| OCR Post-processing tool                  | Transformer models to correct OCR errors, along with ca 50,000 line pairs of OCRed/corrected text.                               | [GitHub](https://github.com/icelandic-lt/ocr-post-processing), [CLARIN-IS](http://hdl.handle.net/20.500.12537/271)            |
| Réttritun                                 | Spell checker that provides spell and grammar correction for Icelandic on Android devices.                                       | [GitHub](https://github.com/icelandic-lt/simacorrect)                                                                         |
| Yfirlestur                                | Web server where a user can enter or submit Icelandic text and have it checked for spelling and grammar errors.                  | [GitHub](https://github.com/icelandic-lt/Yfirlestur), [CLARIN-IS](http://hdl.handle.net/20.500.12537/266)                     |
| Yfirlestur Plugin, Google Docs            | Plugin for Google Docs for Yfirlestur network service.                                                                           | [GitHub](https://github.com/icelandic-lt/Yfirlestur-Docs), [CLARIN-IS](http://hdl.handle.net/20.500.12537/288)                |
| Yfirlestur Plugin, Microsoft Word         | Plugin for Microsoft Word for Yfirlestur network service.                                                                        | [GitHub](https://github.com/icelandic-lt/Yfirlestur-Word), [CLARIN-IS](http://hdl.handle.net/20.500.12537/289)                |