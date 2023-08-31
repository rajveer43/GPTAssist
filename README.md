# GPTAssist


Introducing GPTAssist, your very own virtual assistant that comes to life with the power of voice commands! Imagine a world where tasks get accomplished and questions get answered just by the sound of your voice. Built using an ensemble of cutting-edge technologies, including [LangChain](https://github.com/hwchase17/langchain), [GPT4All](https://github.com/nomic-ai/gpt4all), [LlamaCpp](https://github.com/ggerganov/llama.cpp), Chroma, and the incredible [SentenceTransformers](https://www.sbert.net/)., this project redefines the way you interact with technology.

## The Power Behind GPTAssist

This project stands on the shoulders of giants:

**LangChain**: Laying the foundation for seamless communication between you and your assistant.
**GPT4All**: Fueling your assistant's intelligence with advanced language processing capabilities.
**LlamaCpp**: Making the magic happen with lightning-fast text processing.
**Chroma**: Enhancing the visual appeal and user experience.
**SentenceTransformers**: Adding a layer of context and understanding to responses.

But that's not all! With support for OpenAI's *GPT3, GPT4 models, and Cohere* **GPTAssist** opens up a world of possibilities.

## Inspired from PrivateGPT

Inspired by the remarkable [privateGPT](https://github.com/imartinez/privateGPT) project, PersonalGPT takes assistance-making to a whole new level. While drawing inspiration, this project also introduces a unique twist by utilizing [DeepLake VectorStores](https://github.com/activeloopai/deeplake) to efficiently store and manage your dataset and files. It's innovation upon innovation!

# Installing dependencies

Install the necessary dependencies. If you're on Windows, open your command shell and type:
```shell
    pip install -r requirements.txt
```
or Linux and Mac aficionados:
```
   pip3 install -r requirements.txt
```
# Setting Environment Variables

- Open the `PersonalGPT/env_vars.py`. 
- Customize your assistant's behavior by tweaking the `env_vars.py` file. From the model type to voice preferences and API keys, you're in control!



```
MODEL_TYPE: supports LlamaCpp, GPT4All, OpenAI & Cohere
PERSIST_DIRECTORY: is the folder you want your vectorstore in
MODEL_PATH: Path to your GPT4All or LlamaCpp supported LLM
MODEL_N_CTX: Maximum token limit for the LLM model
MODEL_N_BATCH: Number of tokens in the prompt that are fed into the model at a time. Optimal value differs a lot depending on the model (8 works well for GPT4All, and 1024 is better for LlamaCpp)
EMBEDDINGS_MODEL_NAME: SentenceTransformers embeddings model name (see https://www.sbert.net/docs/pretrained_models.html)
TARGET_SOURCE_CHUNKS: The amount of chunks (sources) that will be used to answer a question
VOICE_MODEL=pyttsx3
VOICE_REC_ENGINE=SpeechRecognition
API_KEY=OpeAI or Cohere API Key
```

## Instructions for ingesting your own dataset

Put any and all your files into the `source_documents` directory.

The supported extensions are:

   - `.csv`: CSV,
   - `.docx`: Word Document,
   - `.doc`: Word Document,
   - `.enex`: EverNote,
   - `.eml`: Email,
   - `.epub`: EPub,
   - `.html`: HTML File,
   - `.md`: Markdown,
   - `.msg`: Outlook Message,
   - `.odt`: Open Document Text,
   - `.pdf`: Portable Document Format (PDF),
   - `.pptx`: PowerPoint Document,
   - `.ppt`: PowerPoint Document,
   - `.txt`: Text file (UTF-8),
   - `.xls`: Excel Spreadsheet
   - `.xlsx`: Excel Spreadsheet

Give the following command to ingest all the data.

# Run PersonalGPT
On Windows:
```shell
    python run_PersonalGPT.py
```
On Linux / Mac:
```shell
    python3 run_PersonalGPT.py
```
### Now Give Voice commands whatever you use
```shell
open browser
load my files
ask gpt
tell me a joke
open youtube
```
and many more

This module is free to use, modify, share

Contribution is open for everyone, if you find some issue feel free to pull an Issue request or you've fixed this then do a PR

Thank You, for reading this.
