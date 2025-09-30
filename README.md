# RAG Knowledge Base Curation Pipeline

A comprehensive RAG (Retrieval-Augmented Generation) pipeline for knowledge base curation and evaluation.

## 🚀 Quick Start

### Prerequisites
- Python 3.11 or higher
- [uv](https://docs.astral.sh/uv/getting-started/installation/) package manager

### Installation

1. **Install uv** (if not already installed):
   ```bash
   # Windows (PowerShell)
   powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
   
   # macOS/Linux
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

2. **Clone this repository**:
   ```bash
   git clone <your-repo-url>
   cd RAG
   ```

3. **Install dependencies**:
   ```bash
   uv sync
   ```

4. **Activate the environment** (optional):
   ```bash
   uv shell
   ```

5. **Run the setup script** (optional):
   ```bash
   python setup.py
   ```

## 📚 Usage

### Jupyter Notebooks
```bash
uv run jupyter notebook
```

### Python Scripts
```bash
uv run python main.py
```

### Key Files
- `kb_curation_pipeline.ipynb` - Main knowledge base curation pipeline
- `main.py` - Main Python script entry point
- `good_test_cases.json` - Test cases for evaluation
- `qa_pairs.json` - Question-answer pairs for RAG evaluation

## 📊 Evaluation

The project includes comprehensive evaluation metrics:
- **RAGAS metrics** - For RAG quality assessment
- **LlamaIndex metrics** - For retrieval and generation evaluation
- **Multiple parsers** - Base, Docling, and LlamaParse comparisons

## 🔧 Development

### Adding Dependencies
```bash
uv add package-name
```

### Updating Dependencies
```bash
uv lock --upgrade
```

### Running Tests
```bash
uv run python -m pytest
```
├── main.py                # Main script
├── pyproject.toml         # Project configuration
└── uv.lock               # Locked dependencies
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📝 Notes

- The `uv.lock` file ensures everyone gets identical dependency versions
- Large data files may need to be downloaded separately (see data/ folder)
- Environment variables should be set in `.env` file (not committed to repo)
