# Query Processor (RAG) Project

This repository contains a small Retrieval-Augmented Generation (RAG) experiment that uses a local dataset and a querying script to answer questions.

**Status:** Draft — in progress

**Quick Summary:**
- **Purpose:** Run retrieval over `rag_data.json` and generate answers via a chosen model pipeline.
- **Key scripts:** `RAG_setup.py` (data / environment setup) and `querypross.py` (run queries).

**Prerequisites**
- Python 3.8+ installed
- A virtual environment (recommended)

**Install dependencies**
Run these commands in your project root:

```bash
python -m venv .venv
source .venv/Scripts/activate   # Windows PowerShell: .venv\\Scripts\\Activate.ps1
pip install -r requirement.txt
```

**Configuration**
- Edit `rag_data.json` to provide your retrieval dataset.
- Configure any model keys or endpoints used by `RAG_setup.py` or `querypross.py` (if required) inside those files.

**Usage**
- Prepare data and environment:

```bash
python RAG_setup.py
```

- Run a query (example):

```bash
python querypross.py --question "What is the project about?"
```

Adjust CLI options in `querypross.py` as needed.

**Files**
- `RAG_setup.py`: data preparation and setup
- `querypross.py`: main query/processing script
- `rag_data.json`: dataset used for retrieval
- `requirement.txt`: Python dependencies

**Notes & Next steps**
- Currently using Mistral for question-answering and a selection-transformer for retrieval/selection — this is experimental.
- Improve README with configuration examples for model credentials and example outputs.

**Contributing**
- Open an issue or submit a pull request with improvements.

**License**
- No license has been selected for this project yet.
- A license will be chosen and documented in this repository once the project terms are finalized.

