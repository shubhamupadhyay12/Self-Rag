# Self-RAG (Self-Reflective RAG)

A step-by-step implementation of **Self-RAG** over three company PDFs. Regular RAG retrieves once and answers. Self-RAG makes the pipeline check itself: is the retrieved context relevant, is the answer actually supported by that context, and is the answer good enough? If not, it retrieves again or regenerates.

## The idea

```
question -> retrieve -> is the context relevant?
                          no  -> retrieve again
                          yes -> generate answer -> is it supported by the context?
                                                      no  -> regenerate
                                                      yes -> is it a useful answer? -> return
```

## Knowledge base

Three PDFs stand in for a small company's documents:

- `Company_Policies.pdf`: rules and guidelines
- `Company_Profile.pdf`: company overview and background
- `Product_and_Pricing.pdf`: offerings and pricing tiers

## Notebooks

The pipeline is built up in seven stages. Run them in order:

`self_rag_step1.ipynb` -> `self_rag_step2.ipynb` -> ... -> `self_rag_step7.ipynb`

Each notebook adds one stage to the pipeline, ending with the full self-reflective loop in step 7.

## Setup

Requires Python 3.9+.

```bash
git clone https://github.com/shubhamupadhyay12/Self-Rag.git
cd Self-Rag

python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install notebook langchain langchain-community pypdf chromadb openai
```

Set your key, then start Jupyter:

```bash
export OPENAI_API_KEY="your-openai-api-key"
jupyter notebook
```

## Stack

Python, LangChain, ChromaDB (vector store), OpenAI, pypdf, Jupyter

## License

MIT. See [LICENSE](LICENSE).

## Author

Shubham Upadhyay · [GitHub](https://github.com/shubhamupadhyay12) · [LinkedIn](https://www.linkedin.com/in/shubhamupadhyay25)
