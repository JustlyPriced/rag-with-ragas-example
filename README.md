# Generic RAG with RAGAS Evaluation

Inspired by:

[Modular Rag and chat implementation from URLs, PDFs and txt files. | Patreon](https://www.patreon.com/posts/modular-rag-and-106461497)

-and-

[Coding-Crashkurse/RAG-Evaluation-with-Ragas](https://github.com/Coding-Crashkurse/RAG-Evaluation-with-Ragas)

## Overview

This repository demonstrates a Retrieval-Augmented Generation (RAG) pipeline using the `Rag` class and evaluates its performance using the `Ragas` framework. The main components are:

- `chat_loop.py`: A chat loop that processes files, embeds text, and handles user queries.
- `ragas_eval.py`: Evaluates the RAG pipeline using `Ragas`.

## Prerequisites

Ensure you have the required packages installed:

```sh
pip install -r requirements.txt
```

## Running the Chat Loop

The `chat_loop.py` script processes text and PDF files, embeds the text, and allows user interaction for querying the embedded data.

### Steps:

1. Place your text and PDF files in the `data` folder.
2. Run the script:

```sh
python chat_loop.py
```

3. Follow the prompts to add URLs, search, or exit.

## Evaluating the RAG Pipeline

The `ragas_eval.py` script processes files, generates a test set, and evaluates the RAG pipeline using `Ragas`.

### Steps:

1. Ensure your data files are in the `data` folder.
2. Run the script:

```sh
python ragas_eval.py
```

3. The script will generate and save evaluation results in `evaluation_results.csv`.

## Key Files

- `chat_loop.py`: Main chat loop for processing and querying data.
- `ragas_eval.py`: Script for evaluating the RAG pipeline.
- `rag.py`: Contains the `Rag` class with methods for processing and embedding text.
- `requirements.txt`: Lists the required Python packages.

## Example Usage

### Running the Chat Loop

```sh
python chat_loop.py
```

### Running the Evaluation

```sh
python ragas_eval.py
```

## Additional Information

For more details on `Ragas`, refer to the [Ragas Documentation](https://docs.ragas.io/en/stable/).