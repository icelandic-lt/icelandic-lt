## TTS - Text to Speech

### Overview

Text-to-Speech (TTS) is the process of converting written text into natural-sounding spoken language. The Icelandic Language Technology Program has developed various TTS resources, including datasets, models, and software. While many of these are research-oriented, some TTS projects are production-ready and already serve hundreds of Icelandic users daily, such as the [Símarómur](https://github.com/icelandic-lt/simaromur) Android app. We are proud that our [G2P pronunciation dictionary](https://github.com/icelandic-lt/iceprondict) has been used as a foundation for e.g. the Microsoft Azure TTS voices Gunnar & Gudrun. 

A typical TTS pipeline includes:

1. Text normalization: Cleaning and standardizing input text
2. Grapheme-to-Phoneme (G2P) conversion: Transforming normalized text into phonetic representation
3. Synthesis: Generating speech from the phonetic representation

The first two steps (text normalization and G2P conversion) are collectively known as the TTS frontend. Step 3, 'Synthesis', is often further divided into two parts:
- Encoder or acoustic model, which outputs e.g. Mel spectrograms or latent representations
- Decoder or vocoder, which converts the encoder output into audible speech

Although end-to-end TTS approaches have gained popularity recently, where all 3 steps are combined into one monolithic model, our focus has been on this more traditional pipeline. This approach offers easier implementation across various platforms and is better suited to the currently limited amount of available Icelandic audio corpora.

Our projects are categorized into:

* [Datasets](#datasets): The foundation for training TTS-related models, including audio datasets and specialized corpora for text normalization and G2P conversion. Part-of-Speech (PoS) tagging datasets, needed for text normalization and other LT projects, are listed in the [Language Resources](./lr.md) section.
* [Models](#models):  A range of models, from experimental versions to production-ready implementations, including speech synthesis and G2P models. While many are still in the research phase, a select few are actively used in production TTS applications.
* [Software / Model Training](#software--training): Tools, scripts, and software used for model training, data preprocessing, and running the TTS pipeline on various platforms.

For additional G2P-related resources, please refer to [Language Resources](./lr.md)

---

## Datasets

### Homograph Corpus

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** This labeled corpus of Icelandic homographs contains a list of all labeled homographs and a corpus of sentences extracted from a selection of the Icelandic Gigaword Corpus (IGC-2022 - annotated version), containing these homographs, labeled by pronunciation.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/327)  

### Text normalization corpus

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** A corpus of 70,000 sentences taken from general text, both before normalization and normalized using the [Regína normalizer](https://github.com/icelandic-lt/regina_normalizer); 70,000 sentences taken from sports news, both before normalization and normalized using the [Regína normalizer](https://github.com/icelandic-lt/regina_normalizer); 40,000 sentences taken from all domains, manually normalized.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/158)  

### Talrómur 1

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** A speech corpus with 122,417 short audio clips of 8 different speakers reading short sentences. Audio files are resampled into the format 22kHz, 16bit RIFF.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/104)  

### Talrómur 2

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** A speech corpus with 56,225 audio clips of forty different speakers reading short sentences. Audio files are resampled into the format 22kHz, 16bit RIFF.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/298)  

### Talrómur 3

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** An emotional speech corpus with 15,078 audio clips of 7 different speakers reading short sentences with varying emotional intensity levels. Audio files are in 48kHz, 24bit FLAC. Corpus preparation scripts are provided on GitHub.<br>
**Locations:** [CLARIN-IS](https://repository.clarin.is/repository/xmlui/handle/20.500.12537/344), [GitHub](https://github.com/icelandic-lt/emospeech-scripts)<br>

### Talrómur 1 RAW

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** 48kHz, 16bit FLAC version of Talrómur 1 speech corpus (21.02), unprocessed and unselected.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/322)  

### TTS Intelligibility test set

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Dataset  
**Description:** This test set contains sentences for intelligibility testing of a TTS system. It is a set of 50 sentences where each sentence occurs twice: once in its correct version and once containing one spelling error. Half of the 50 sentences are constructed in the form of Semantically Unpredictable Sentences (SUS) and the other half consists of sentences extracted from the Icelandic Error Corpus and from development data for a text normalizer.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/182)  

---

## Models

### Álfur hratt - FLite voice for Símarómur up to v1.3

[![Apache-2.0 License](https://img.shields.io/badge/License-Apache--2.0-blue)](https://opensource.org/licenses/Apache-2.0)  
**Type:** Model  
**Description:** FLite voice, based on the Festival Recipe, for usage in Símarómur up to v1.3. It is considered deprecated now, as FLite voices are not supported anymore in Símarómur since v2.0.  
**Location:** [GitHub](https://github.com/icelandic-lt/simaromur_voices/releases/tag/0.2)  

### ESPnet Talrómur 1 Fastspeech2, Tacotron2 models

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** This release contains TTS models for all 8 voices from Talrómur 1, intended for use with the ESPNet toolkit. The models are trained using fully phonemized, stress-annotated inputs including syllable boundary markers ('.') and word boundary markers (','), obtainable using IceG2P. The training recipes are included in the 202207 version of the toolkit.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/294)  

### ESPnet Talrómur 2 Xvector Tacotron2 model

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** This model was trained using the talromur2 recipe in ESPnet.  
**Location:** [HuggingFace](https://huggingface.co/espnet/talromur2_xvector_tacotron2)  

### IceHoC

[![Apache-2.0 License](https://img.shields.io/badge/License-Apache--2.0-blue)](https://opensource.org/licenses/Apache-2.0)  
**Type:** Model  
**Description:** IceHoC is a binary classifier for Icelandic homographs. The repository contains all training code as well as the models and uses the Icelandic Homograph Corpus  
**Location:** [GitHub](https://github.com/icelandic-lt/IceHoc), [CLARIN-IS](http://hdl.handle.net/20.500.12537/329)  

### G2P LSTM model

[![Apache-2.0 License](https://img.shields.io/badge/License-Apache--2.0-blue)](https://opensource.org/licenses/Apache-2.0)  
**Type:** Model  
**Description:** LSTM encoder-decoder sequence-to-sequence models, trained for Icelandic G2P. The models were trained using the baseline for the Sigmorphon 2020 Shared task in multilingual G2P, with manually transcribed training data of ~5,800 words per pronunciation variant. This is the model for IceG2P.  
**Location:** [GitHub](https://github.com/icelandic-lt/g2p-lstm)  

### G2P Thrax

[![Apache-2.0 License](https://img.shields.io/badge/License-Apache--2.0-blue)](https://opensource.org/licenses/Apache-2.0)  
**Type:** Model  
**Description:** G2P grammar, models & runtime system in C++ for Edge-device usage (e.g. iOS, Android). This G2P system is a much faster but also less accurate G2P system in comparison to IceG2P.  
**Location:** [GitHub](https://github.com/icelandic-lt/g2p-thrax)  

### GlowTTS Talrómur 1 voice models

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** GlowTTS models for four different voices from the Talrómur 1 corpus. The models were trained using the Coqui TTS library after it was adapted for Icelandic.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/293)  

### GlowTTS Multi-Speaker Talrómur 2 voice model

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** This release includes a partially trained multi-speaker model using the GlowTTS architecture in the Coqui TTS library. The model is trained on all the speakers in the Talrómur 2 corpus.  
**Location:** [CLARIN-IS](http://hdl.handle.net/20.500.12537/293)  

### VITS model "Steinn" from voice Talrómur 1/H trained via Piper TTS

[![CC-BY-4.0 License](https://img.shields.io/badge/License-CC--BY--4.0-blue)](https://creativecommons.org/licenses/by/4.0/)  
**Type:** Model  
**Description:** This model is used for the Android App [Símarómur](https://github.com/icelandic-lt/simaromur) for v2.0 and later and was trained and converted using the scripts from [Piper TTS](https://github.com/rhasspy/piper).  
**Location:** [GitHub](https://github.com/grammatek/simaromur_voices)  

---

## Software / Training


| Project                   | Type     | <div style="width:350px"/> Description                                                                                                                                                                                                               | <div style="width:100px"/> Location                                                                                                                                  |
|---------------------------|----------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Document reader           | Software | Document reader web application that interfaces to a TTS service via network                                                                                                                                                                         | [GitHub](https://github.com/icelandic-lt/tts_webapp)<br>[CLARIN-IS](http://hdl.handle.net/20.500.12537/282)                                                          |
| Emotional Speech Scripts  | Software | Audio dataset recording and preparation scripts, used for generation of the [Talrómur 3](https://repository.clarin.is/repository/xmlui/handle/20.500.12537/344) dataset                                                                              | [GitHub](https://github.com/icelandic-lt/emospeech-scripts)                                                                                                          |
| G2P-service               | Software | Restful service for sequitur and fairseq g2p models                                                                                                                                                                                                  | [GitHub](https://github.com/icelandic-lt/g2p-service)                                                                                                                |
| IceG2P                    | Software | Grapheme-to-phoneme toolkit for Python. Uses G2P LSTM model.                                                                                                                                                                                         | [GitHub](https://github.com/icelandic-lt/ice-g2p)                                                                                                                    |
| LOBE                      | Software | Recording client made specifically for TTS data collections                                                                                                                                                                                          | [GitHub](https://github.com/icelandic-lt/LOBE)                                                                                                                       |
| Phrasing tool             | Software | Tool for adding pauses in text for more natural speech.                                                                                                                                                                                              | [GitHub](https://github.com/icelandic-lt/phrasing-tool)                                                                                                              |
| Regína normalizer         | Software | Text normalizer for TTS based on regular expressions.                                                                                                                                                                                                | [GitHub](https://github.com/icelandic-lt/regina_normalizer)                                                                                                          |
| Símarómur                 | Software | Icelandic TTS App for the Android TTS service. Available on [Google Play](https://play.google.com/store/apps/details?id=com.grammatek.simaromur).                                                                                                    | [GitHub](https://github.com/icelandic-lt/simaromur)<br>[Google Play](https://play.google.com/store/apps/details?id=com.grammatek.simaromur)                          |
| Text cleaner              | Software | Text cleaning module for processing raw text input. This module is a component of a TTS-Frontend engine, more specifically, it is the first step in processing raw text input before being normalized in the next step in the TTS-Frontend pipeline. | [GitHub](https://github.com/icelandic-lt/text-cleaner)                                                                                                               |
| Tiro-TTS                  | Software | TTS RESTful service in Python for serving fastspeech2 voice models as well as Amazon Polly voices                                                                                                                                                    | [GitHub](https://github.com/icelandic-lt/tiro-tts)<br>[CLARIN-IS](http://hdl.handle.net/20.500.12537/268)                                                            |
| TTS data preparation      | Software | Module for preparing text data for TTS data collections, specifically for the Icelandic language.                                                                                                                                                    | [GitHub](https://github.com/icelandic-lt/tts_data)                                                                                                                   |
| TTS frontend API          | Software | gRPC service definitions for the TTS frontend preprocessing pipeline                                                                                                                                                                                 | [GitHub](https://github.com/icelandic-lt/tts-frontend-api)                                                                                                           |
| TTS frontend pipeline     | Software | TTS text-processing pipeline for Icelandic. The pipeline includes modules for html parsing, text cleaning, text normalization for TTS, spell and grammar correction, phrasing, and grapheme-to-phoneme (g2p) conversion.                             | [GitHub](https://github.com/icelandic-lt/tts-frontend)<br>[CLARIN-IS](http://hdl.handle.net/20.500.12537/279)                                                        |
| TTS frontend service      | Software | gRPC service for the TTS frontend pipeline to provide the service in server environments as part of a network-based TTS system                                                                                                                       | [GitHub](https://github.com/icelandic-lt/tts-frontend-service)                                                                                                       |
| WebRICE                   | Software | Browser plugin is a software add-on that gives people access to listen to text on web pages. It is interfacing with a TTS service over Internet                                                                                                      | [GitHub](https://github.com/icelandic-lt/webrice-chrome-extension)<br>[CLARIN-IS](http://hdl.handle.net/20.500.12537/261)                                            |
|                           |          | **--- Training Code Below ---**                                                                                                                                                                                                                      |                                                                                                                                                                      |
| FastSpeech2               | Training | Training code adapted to Icelandic of the original paper "FastSpeech 2: Fast and High-Quality End-to-End Text to Speech".                                                                                                                            | [GitHub](https://github.com/icelandic-lt/FastSpeech2)<br>[CLARIN-IS](http://hdl.handle.net/20.500.12537/201)                                                         |
| Festival Unit-Selection   | Training | Training code for generating unit selection voice for the Festival speech system                                                                                                                                                                     | [GitHub](https://github.com/icelandic-lt/unit-selection-festival/)                                                                                                   |
| GlowTTS                   | Training | Training code for Icelandic multi-speaker GlowTTS voice                                                                                                                                                                                              | [GitHub](https://github.com/icelandic-lt/coqui-ai-TTS)<br>[CLARIN-IS](http://hdl.handle.net/20.500.12537/293)<br>[CLARIN-IS](http://hdl.handle.net/20.500.12537/292) |
| G2P LSTM model            | Training | Training code for LSTM encoder-decoder sequence-to-sequence model used in IceG2P.                                                                                                                                                                    | [GitHub](https://github.com/icelandic-lt/g2p-lstm)                                                                                                                   |
| IceHoC                    | Training | Training code for IceHoC - classifier for Icelandic homographs                                                                                                                                                                                       | [GitHub](https://github.com/icelandic-lt/IceHoc)<br>[CLARIN-IS](http://hdl.handle.net/20.500.12537/329)                                                              |
| Piper TTS                 | Training | Training code for the VITS voice "Steinn" for the Símarómur Android App.                                                                                                                                                                             | [GitHub](https://github.com/rhasspy/piper)                                                                                                                           |
| Tacotron2 and Fastspeech2 | Training | Training code for Tacotron2 and Fastspeech2 within the official ESPnet TTS project. Fork of ESPnet with updated recipes.                                                                                                                             | [GitHub](https://github.com/icelandic-lt/espnet)                                                                                                                     |
| Thrax G2P                 | Training | Training code & runtime for Thrax G2P                                                                                                                                                                                                                | [GitHub](https://github.com/icelandic-lt/g2p-thrax)                                                                                                                  |
| X-vector Tacotron2        | Training | Training code for the Icelandic port of ESPNet TTS to produce X-Vectors for Tacotron2                                                                                                                                                                | [GitHub](https://github.com/icelandic-lt/espnet)                                                                                                                     |