# File Q&A Bot

A simple command-line tool that answers questions based only on the content of a text file. It uses a Retrieval-Augmented Generation (RAG) approach with LangChain and OpenRouter.

## How It Works

The bot reads a `.txt` file and splits it into small chunks. Each chunk is converted into an embedding and stored in a Chroma vector database. When you ask a question, the most relevant chunks are retrieved and passed to the LLM, which answers using only that context.

## Example

```text
Enter file path: yoga.txt

You: Where does the word 'yoga' come from?

Assistant: The word 'yoga' comes from the Sanskrit word 'yuj', which means 'to unite'.
```

## Tech Stack

The project is built with Python and LangChain. It uses OpenRouter for the LLM and HuggingFace for embeddings.
