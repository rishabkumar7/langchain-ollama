# langchain-ollama

Run Ollama models with LangChain.

## Overview

This project demonstrates how to use LangChain with Ollama models to generate summaries from documents loaded from a URL.

## Requirements

You will need [Ollama](https://ollama.com/) installed, and pull the open-source models, like phi3 or gemma2.

```sh
ollama pull phi3
```

Additonally, make sure you have the following Python packages installed:

- langchain
- langchain-community
- langchain-text-splitters
- transformers
- bs4

You can install these dependencies using the `requirements.txt` file:

## Usage

To use this script, follow these steps:

1. Clone the repository:

```sh
git clone https://github.com/rishabkumar7/langchain-ollama.git
cd langchain-ollama
```

2. Create a virtual environment, I recommend using [venv](https://docs.python.org/3/library/venv.html).

```sh
python -m venv .venv
```

3. Install the required dependencies:

```sh
pip install -r requirements.txt
```

4. Run the main.py script:

```sh
python main.py
```

The script will load documents from the specified URL, split them into chunks, and generate a summary using the Ollama model. You can change the `url` in `main.py` to any blog/article you want to summarize.
