# Self-RAG (Self-Reflective Retrieval-Augmented Generation)

A step-by-step implementation of **Self-RAG** using custom PDF documents (`Company Policies`, `Company Profile`, and `Product and Pricing`) as knowledge bases.

Self-RAG improves traditional Retrieval-Augmented Generation by introducing self-reflection mechanisms—evaluating whether retrieved context is relevant, if generated responses are grounded in the retrieved facts, and if the final answer meets quality standards.

---

## 📁 Repository Structure

Self-Rag/
├── Company_Policies.pdf       # Knowledge base: Company rules & guidelines
├── Company_Profile.pdf        # Knowledge base: Company overview & background
├── Product_and_Pricing.pdf    # Knowledge base: Offerings & pricing tiers
├── self_rag_step1.ipynb       # Notebook Step 1
├── self_rag_step2.ipynb       # Notebook Step 2
├── self_rag_step3.ipynb       # Notebook Step 3
├── self_rag_step4.ipynb       # Notebook Step 4
├── self_rag_step5.ipynb       # Notebook Step 5
├── self_rag_step6.ipynb       # Notebook Step 6
├── self_rag_step7.ipynb       # Notebook Step 7
├── LICENSE                    # Project license
└── README.md                  # Project documentation

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.9+ installed along with Jupyter Notebook or JupyterLab.

### 1. Clone the Repository

git clone https://github.com/shubhamupadhyay12/Self-Rag.git
cd Self-Rag

### 2. Set Up Environment & Install Dependencies

Create a virtual environment (optional but recommended):

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

Install the required packages:

pip install langchain langchain-community pypdf chromadb openai

---

## 📖 Step-by-Step Workflow

Follow the notebooks in numerical order:

1. `self_rag_step1.ipynb`
2. `self_rag_step2.ipynb`
3. `self_rag_step3.ipynb`
4. `self_rag_step4.ipynb`
5. `self_rag_step5.ipynb`
6. `self_rag_step6.ipynb`
7. `self_rag_step7.ipynb`

---

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.
