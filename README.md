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

# Ingesting Your Own Dataset

To make your PersonalGPT assistant smarter, you can feed it your own dataset. Follow these steps:

1. **Prepare Your Files**: Gather the documents you want to include in your dataset. Supported file formats are:

    - `.csv`: CSV files
    - `.docx`, `.doc`: Word Documents
    - `.enex`: EverNote
    - `.eml`: Email
    - `.epub`: EPub
    - `.html`: HTML Files
    - `.md`: Markdown
    - `.msg`: Outlook Messages
    - `.odt`: Open Document Text
    - `.pdf`: Portable Document Format (PDF)
    - `.pptx`, `.ppt`: PowerPoint Documents
    - `.txt`: Text files (UTF-8)
    - `.xls`, `.xlsx`: Excel Spreadsheets

2. **Place Files in Directory**: Move all these files into the `source_documents` directory.

3. **Ingest the Data**: To incorporate your files into PersonalGPT's knowledge base, use the following command:

    On Windows:
    ```shell
    python run_PersonalGPT.py
    ```

    On Linux / Mac:
    ```shell
    python3 run_PersonalGPT.py
    ```

# Giving Voice Commands

Now, let's dive into interacting with your PersonalGPT assistant using voice commands. Just speak naturally and watch the magic happen!

1. **Open Browser**: Want to open a browser window? Simply say:
    ```
    open browser
    ```

2. **Load My Files**: To instruct the assistant to load your files, say:
    ```
    load my files
    ```

3. **Ask GPT**: Need answers or information? Use the command:
    ```
    ask gpt
    ```

4. **Tell Me a Joke**: In the mood for some humor? Try:
    ```
    tell me a joke
    ```

5. **Open YouTube**: Want to watch videos? Just say:
    ```
    open youtube
    ```

... and many more commands that make your interactions with PersonalGPT productive and enjoyable!

## Open for Contributions

GPTAssist isn't just lines of code; it's a living, breathing project fueled by the passion and collaboration of countless individuals. This project thrives on openness, sharing, and the collective drive to make it better each day.

**1. Open to All**: GPTAssist is a welcoming oasis for developers, enthusiasts, and curious minds alike. It's an open-source project, which means anyone can use, modify, and share it without any restrictions. Whether you're a seasoned coder or just starting your journey, you're invited to join in.

**2. Embracing Collaboration**: The beauty of open source lies in collaboration. If you stumble upon any issues or bugs while using GPTAssist, please don't hesitate to open an Issue request. Your feedback is invaluable, and it's the first step towards improvement.

**3. Be the Change**: If you're the kind of person who loves to roll up their sleeves and dive into the nitty-gritty of code, don't hold back from submitting a Pull Request. Your contributions can be the key to solving problems, enhancing features, and taking GPTAssist to the next level.

**4. A Journey Together**: Your journey with GPTAssist starts right here, right now. By being a part of this community, you're not just a user; you're a fellow traveler. You'll learn, grow, and connect with others who share your passion for technology and innovation.

So, whether you're here to explore the code, fix a bug, suggest an improvement, or simply be part of this exciting journey, GPTAssist welcomes you with open arms. Together, we can harness the power of this project and shape it into something truly remarkable.

Thank you for taking the time to dive into GPTAssist. Your curiosity and enthusiasm are the driving forces behind the success of this project. Let's make the most of this incredible opportunity to learn, create, and collaborate.
