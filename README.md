# RAG component experiments

**Document ingestion, chunking, embeddings and vector storage with LangChain.**

This repository, named Advanced-RAG-Systems, is a learning lab for the building blocks of retrieval-augmented generation. The current notebooks explore document metadata, text/PDF loaders, splitting, SentenceTransformer embeddings and persistent Chroma storage.

## Start with the notebooks

- [Documents](notebook/Documents.ipynb): document objects, text/directory loaders and PDF loading.
- [PDF pipeline](notebook/pdf_loader.ipynb): PDF ingestion, chunking, embedding generation and Chroma indexing.

The root `main.py` is a placeholder, not an application entry point. The repository does not yet demonstrate complete agentic, hybrid or multi-hop RAG products. For a more integrated application, see [TruthGuard](https://github.com/Laabh-Gupta/TruthGuard).

## Explore locally

```bash
git clone https://github.com/Laabh-Gupta/Advanced-RAG-Systems.git
cd Advanced-RAG-Systems
python -m venv .venv
```

Activate the environment. Review [pyproject.toml](pyproject.toml) and the notebook imports when choosing a compatible Python 3.12+ environment, then install the project dependencies and Jupyter:

```bash
python -m pip install -e .
python -m pip install jupyterlab
jupyter lab
```

Some cells use older LangChain import paths; adjust those or use a matching dependency environment before rerunning. Work from `notebook/` so relative data paths resolve. Supply PDFs/text you have permission to process and use a new local vector-store directory for your own experiments.

## Scope

**Python · LangChain · SentenceTransformers · ChromaDB · Jupyter**

There is no hosted demo, benchmark or locked, newly verified reproduction claimed here. Committed sample documents/vector artifacts are development material. The useful evidence is the notebook implementation of individual RAG components.
