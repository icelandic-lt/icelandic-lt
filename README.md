# Icelandic Language Technology Program

Welcome to the main entry page for the Icelandic Language Technology program **Icelandic-LT**.

Here, you'll find an overview over all relevant repositories and resources of this program, which has been developing core technologies for the Icelandic language since its inception in 2018.
You can read more about the Icelandic Language Technology program [here](https://www.stjornarradid.is/lisalib/getfile.aspx?itemid=56f6368e-54f0-11e7-941a-005056bc530c) (in Icelandic) and [here](https://clarin.is/media/uploads/mlt-en.pdf) (in English).

In this context, the term *core technologies* refer to resources that can be used by appropriately skilled individuals to reproduce our results, continue our research, develop products based on these resources, or educate themselves about the subject.

As is not uncommon for a development program spanning multiple years, some of the core technologies and models developed in the program may be already outdated.
For source code-based projects, this is often related to frameworks and 3rd party dependencies. For instance, in cases where Python is used as the programming language, sometimes Python versions that have reached end-of-life status are used,
as well as older versions of dependencies. Some of the resources have experimental status and need further research or development to be usable in a production environment.

If you encounter difficulties when trying out any of the resources, we encourage you to send us feedback via a GitHub issue, either on this main repository or at the appropriate repository's issue tracker.

We always welcome contributions and discussions!

**We are currently in the process of updating the status of all projects and testing their applicability with current technologies.**

## Resource Locations

We use several web locations to store the LT program's deliverables:

- [Clarin.is](https://clarin.is/en/): For general archiving purposes, i.e., source code snapshots, datasets, models
- [GitHub](https://github.com/icelandic-lt): Primarily for source code, sometimes also for models or binaries
- [Hugging Face](https://huggingface.co/Icelandic-lt): For models and datasets

### Clarin.is

CLARIN stands for [*Common Language Resources and Technology Infrastructure*](https://www.clarin.eu/), which is a part of the *European Research Infrastructure Consortium* (ERIC), an EU initiative.

The resources on [Clarin.is](https://clarin.is) are mainly for archiving milestone results, as Clarin.is offers stricter archiving guarantees. You can find most Icelandic-LT resources there, but these are in some cases outdated compared to their corresponding repositories on GitHub or Hugging Face. Most resources on Clarin.is are source code snapshots or archives of models and datasets, sometimes lacking usage documentation. Therefore, you should generally prefer the GitHub or Hugging Face repositories if you'd like to work with them. However, some resources are only available on Clarin.is. 

### GitHub

Numerous computer programs, libraries, Python packages, training scripts, web applications, etc., have been developed within the Icelandic-LT program, and most of these are available as GitHub repositories. We have assembled all these repositories - currently more than 75 - under the umbrella organization [GitHub Icelandic-LT](https://github.com/icelandic-lt), where you can browse and search all organization repositories.

### Hugging Face

On [Hugging Face](https://huggingface.co/Icelandic-lt), we have created an Icelandic-LT organization that provides datasets and many models. Hugging Face is the leading hub for machine learning models and datasets and is easily integrable into Machine Learning training scripts. Many of the Icelandic LT models and datasets weren't created with Hugging Face in mind, so some are very raw and not directly loadable in a convenient way. Nevertheless, having these on Hugging Face makes it possible to use them with some minor adaptations to existing scripts.
**We are still in the process of moving most of the existing datasets and models here.**

## Language technology domains

In the Icelandic LT program, we have addressed the following LT categories:

### Language Resources

Language Resources are general resources needed by many language technology domains. These are mostly datasets, lexica, corpora & dictionaries. More specific datasets & dictionaries can be found under their respective category.

Browse [Language resources](https://github.com/icelandic-lt/icelandic-lt/blob/main/doc/lr.md)

### ASR (Automatic Speech Recognition)

ASR, also known as Speech-to-Text (STT), is the technology that converts spoken words into written text. It aims to mimic the human ability to listen and transcribe spoken words. Related technologies include speaker diarization, which segments audio recordings by speaker labels to determine "who spoke when".

Browse [ASR resources](https://github.com/icelandic-lt/icelandic-lt/blob/main/doc/asr.md)

### Machine Translation

Machine Translation is the process of automatically translating text from one natural language to another using computer applications.

Browse [Machine Translation resources](https://github.com/icelandic-lt/icelandic-lt/blob/main/doc/mt.md)

### Support Tools

General NLP tools (tokenizer, tagger, parser) that are often used as part of LT pipelines.

Browse [Support Tools](https://github.com/icelandic-lt/icelandic-lt/blob/main/doc/st.md)

### Spell and Grammar Checking

Spelling and Grammar Checkers are computer programs that identify apparent misspellings and grammatical errors in text.

Browse [Spell and Grammar Checking resources](https://github.com/icelandic-lt/icelandic-lt/blob/main/doc/sc.md)

### TTS (Text-to-Speech)

Text-to-Speech (TTS) is the task of generating natural-sounding speech from text input. TTS models can be used in any speech-enabled application that requires converting text to speech imitating human voice.

Browse [Text-to-Speech resources](https://github.com/icelandic-lt/icelandic-lt/blob/main/doc/tts.md)

## License

The aim of the Icelandic LT program has been to provide permissive licenses for all our projects and deliverables, ensuring their usability for everyone, including in commercial, educational, and research environments.

Unless explicitly stated otherwise within a project's repository, datasets and models are provided under the [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/) license, and source code is provided under the [Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0) license.
