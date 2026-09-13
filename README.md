<div align="center">

#  NLP Mastery Journey
### From Zero to Production — 10 Hands-On Notebooks Covering Everything Modern NLP

*A self-contained, copy-paste-ready course through Natural Language Processing — from loading your first CSV to fine-tuning Transformers and building RAG pipelines.*

**Created by [Swapnil Das](#-about-the-author)**

[![Author](https://img.shields.io/badge/Author-Swapnil%20Das-blueviolet?style=for-the-badge)](#-about-the-author)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github)](https://github.com/unthinkingFool)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/swapnil-das-603824236)


**📌 Found this useful? The fastest way to say thanks is a visit to [my profile](#-about-the-author) — it takes 10 seconds and means a lot.**

</div>

---

## 👋 About the Author

This repository is written and maintained by **Swapnil Das**.

If these notebooks saved you time, taught you something new, or you're now using pieces of this code in your own NLP projects — **please take a moment to check out my profile and say hi.** Every star, follow, and connection genuinely helps.

> ### 🔗 [**GitHub**](https://github.com/unthinkingFool) · [**LinkedIn**](https://www.linkedin.com/in/swapnil-das-603824236) 


If you use this repo, fork it, or build on it — a ⭐ on the GitHub repo and a mention/tag when you share your work is always appreciated.

---

## 📖 What This Repo Is

Ten Jupyter notebooks, meant to be worked through **in order**, that take you from "I've never loaded a text file in Python" to "I can build, fine-tune, and evaluate a real RAG or classification system." Every notebook follows the same philosophy:

- **Every line of code is commented — explaining *why*, not just *what*.** You should be able to read a cell once and understand it, even on your first pass through NLP.
- **Live, runnable cells wherever possible.** Math (attention, BLEU, ROUGE, positional encoding, LoRA) is implemented from scratch in NumPy so you see it actually work, not just described. No hidden magic.
- **🔀 Alternatives callouts** — every technique is shown next to the other tools that exist for the same job, and when you'd reach for each one instead.
- **📋 Copy-paste templates** — functions and pipelines are written generically on purpose, so you can lift them almost unchanged into your own next project.
- **Industry-grounded, not just academic.** Each module explains where the technique actually shows up in production at real companies — not only how it works in theory.

---

## 🗺️ The Learning Path

Work through these **in order** — each notebook builds directly on ideas and sometimes literal code (datasets, functions) from the ones before it.

| # | Notebook | You'll learn | Cells |
|---|----------|---------------|:---:|
| 01 | [`01_NLP_Data_Acquisition.ipynb`](01_NLP_Data_Acquisition.ipynb) | Loading CSV/JSON/Excel, public datasets, web scraping, REST APIs, extracting text from PDFs/images (OCR)/audio/video, building a clean corpus | 46 |
| 02 | [`02_NLP_Text_Preprocessing.ipynb`](02_NLP_Text_Preprocessing.ipynb) | Cleaning noisy text, tokenization, stopwords, stemming vs. lemmatization, POS tagging & NER, a reusable `TextPreprocessor` pipeline | 81 |
| 03 | [`03_NLP_Text_Representation.ipynb`](03_NLP_Text_Representation.ipynb) | Bag-of-Words, n-grams, TF-IDF, feature hashing, co-occurrence matrices, a preview of embeddings | 33 |
| 04 | [`04_NLP_Word_Sentence_Embeddings.ipynb`](04_NLP_Word_Sentence_Embeddings.ipynb) | Word2Vec (CBOW/skip-gram) & FastText trained live, GloVe, PCA/t-SNE visualization, sentence embeddings, semantic search | 30 |
| 05 | [`05_NLP_Classical_Machine_Learning.ipynb`](05_NLP_Classical_Machine_Learning.ipynb) | Naive Bayes, Logistic Regression, SVM, gradient-boosted trees, cross-validation, imbalanced data, calibration, production deployment | 41 |
| 06 | [`06_NLP_Neural_Networks_RNN_LSTM.ipynb`](06_NLP_Neural_Networks_RNN_LSTM.ipynb) | RNNs, LSTMs, GRUs, bidirectional models, sequence labeling, attention — all trained in PyTorch | 31 |
| 07 | [`07_NLP_Transformer_Architecture.ipynb`](07_NLP_Transformer_Architecture.ipynb) | Self-attention & multi-head attention from scratch in NumPy, positional encoding, encoder/decoder/encoder-decoder, BPE tokenization | 31 |
| 08 | [`08_NLP_Fine_Tuning_Transformers.ipynb`](08_NLP_Fine_Tuning_Transformers.ipynb) | Prompting vs. fine-tuning vs. RAG, the `Trainer` API, layer freezing, LR warmup, **LoRA implemented from scratch** | 25 |
| 09 | [`09_NLP_RAG_and_LLM_Patterns.ipynb`](09_NLP_RAG_and_LLM_Patterns.ipynb) | Chunking, building a live retriever, prompt augmentation, retrieval metrics, hybrid search, agents & tool use | 27 |
| 10 | [`10_NLP_Summarization_Translation_QA_Evaluation.ipynb`](10_NLP_Summarization_Translation_QA_Evaluation.ipynb) | Extractive summarization, translation, QA, and **BLEU/ROUGE implemented from scratch**, BERTScore, LLM-as-judge | 31 |

**Total: ~370 cells of hands-on, commented, production-grounded NLP.**

---

## 📚 Detailed Module Breakdown

A closer look at exactly what's inside each notebook.

<details>
<summary><strong>01 — NLP Data Acquisition</strong></summary>

| # | Source | You will learn |
|---|--------|-----------------|
| 1 | Local files (CSV/TSV/JSON/Excel) | `pandas`, the standard `csv` module, and when to use each |
| 2 | Public NLP datasets | `datasets` (Hugging Face), `sklearn`, `nltk` corpora |
| 3 | Web scraping | `requests` + `BeautifulSoup`, pagination, ethics/`robots.txt` |
| 4 | REST APIs | auth, pagination, rate limits, a reusable fetch template |
| 5 | Text-bearing files | `.txt`, `.docx`, `.pdf` (two libraries compared) |
| 6 | Images (OCR) | `pytesseract`, image pre-processing |
| 7 | Audio | Whisper & `SpeechRecognition` for transcription |
| 8 | Video | extracting the audio track, then transcribing it |
| 9 | Consolidation | turning everything into one clean corpus format |
| 10 | Production practices | retries, caching, logging, rate-limiting, legal notes |

</details>

<details>
<summary><strong>02 — NLP Text Preprocessing</strong></summary>

| # | Stage | What it does |
|---|-------|---------------|
| 1 | Setup & Sample Data | Get some deliberately messy text to practice on |
| 2 | Cleaning (Noise Removal) | Strip HTML, URLs, emojis, punctuation, slang, typos |
| 3 | Tokenization | Break text into words / subwords the model can consume |
| 4 | Stopword Removal | Drop low-information filler words ("the", "is", "a") |
| 5 | Stemming vs Lemmatization | Reduce words to their root form |
| 6 | POS Tagging & NER | Extract grammatical & entity signals (used in some pipelines) |
| 7 | Reusable Pipeline Class | Package everything into one copy-paste `TextPreprocessor` |
| 8 | Apply to Real Data | Run the pipeline on actual IMDB movie reviews |
| 9 | Text → Numbers | Bag-of-Words & TF-IDF (the bridge to modeling) |
| 10 | Best Practices & Pitfalls | What big tech teams actually do differently, and why |
| 11 | Cheat Sheet | Every snippet in one place for fast copy-paste |

</details>

<details>
<summary><strong>03 — NLP Text Representation</strong></summary>

| # | Technique | Why it still matters |
|---|-----------|------------------------|
| 1 | Bag of Words (BoW) | The simplest, most interpretable baseline — still used for quick baselines & spam filters |
| 2 | N-grams (unigram/bigram/trigram) | Captures local word order BoW alone throws away |
| 3 | TF-IDF | The industry-standard classical representation for search & text classification |
| 4 | Feature Hashing | How production systems handle vocabularies too large to fit in memory |
| 5 | Co-occurrence matrices | The bridge concept between counting and embeddings |
| 6 | Word embeddings (Word2Vec/GloVe/FastText) | Dense vectors that capture meaning, not just counts |
| 7 | Contextual embeddings (BERT-style) preview | The modern default for anything accuracy-critical |
| 8 | Choosing + productionizing | A decision guide, and a save/load `Pipeline` template |

</details>

<details>
<summary><strong>04 — Word & Sentence Embeddings</strong></summary>

| # | Topic | Why it matters |
|---|-------|------------------|
| 1 | The distributional hypothesis | The one idea every embedding method is built on |
| 2 | Word2Vec internals (CBOW vs Skip-gram, negative sampling) | So "just call `.fit()`" stops being a black box |
| 3 | GloVe | Global co-occurrence statistics, count-based vs. predict-based |
| 4 | FastText | Subword embeddings — the fix for out-of-vocabulary words |
| 5 | Exploring the vector space | Similarity, analogies, PCA/t-SNE visualization |
| 6 | Word vectors → document vectors | Averaging, TF-IDF-weighted averaging, Doc2Vec |
| 7 | Sentence embeddings (transformer-based) | The modern default; pooling strategies explained |
| 8 | Evaluation | Intrinsic vs. extrinsic evaluation of embeddings |
| 9 | Production: semantic search end-to-end | Embedding index + nearest-neighbor retrieval, saving/loading |

</details>

<details>
<summary><strong>05 — Classical Machine Learning</strong></summary>

| # | Topic | Industry relevance |
|---|-------|----------------------|
| 1 | Naive Bayes | The classic spam-filter algorithm; still a strong, tiny, fast baseline |
| 2 | Logistic Regression | The single most common production text classifier — fast, interpretable, calibratable |
| 3 | Linear SVMs | Excellent on high-dimensional sparse text features (TF-IDF) |
| 4 | Gradient-boosted trees | Standard when combining text features with structured/tabular signals |
| 5 | Cross-validation & hyperparameter tuning | How you actually pick a model + settings responsibly |
| 6 | Evaluation deep-dive | Precision/recall/F1, confusion matrices, ROC-AUC, PR-AUC |
| 7 | Handling class imbalance | Real-world data is rarely balanced (fraud, abuse, spam...) |
| 8 | Interpretability | Explaining *why* a model predicted what it predicted |
| 9 | Production: calibration, thresholds, monitoring | Turning a notebook model into a safe production system |

</details>

<details>
<summary><strong>06 — Neural Networks: RNN & LSTM</strong></summary>

| # | Topic | Why it matters |
|---|-------|------------------|
| 1 | Why sequence matters | The concrete gap classical ML leaves open |
| 2 | RNN fundamentals | The recurrence idea — a hidden state carried across a sentence |
| 3 | Building & training an RNN classifier | End-to-end PyTorch, on real (small) data |
| 4 | LSTM & GRU | The gating mechanism that fixes RNNs' vanishing-gradient problem |
| 5 | Bidirectional RNNs | Reading context from both directions at once |
| 6 | Sequence labeling (NER/POS-style) | The other major use of RNNs: tagging every token, not just the sentence |
| 7 | Attention | The idea that broke RNNs' long-range bottleneck — and directly seeded Transformers |
| 8 | Why Transformers replaced RNNs | The specific limitation (no parallelism) that made the switch inevitable |
| 9 | Production patterns | Padding, packing, batching, checkpointing — the engineering, not just the math |

</details>

<details>
<summary><strong>07 — Transformer Architecture</strong></summary>

| # | Topic | Why it matters |
|---|-------|------------------|
| 1 | Self-attention, from scratch | The core mechanism — every token looking at every other token, in parallel |
| 2 | Multi-head attention | Why one attention pattern isn't enough |
| 3 | Positional encoding | How position gets back in, once recurrence is gone |
| 4 | The full Transformer block | Residual connections, LayerNorm, feedforward sublayers |
| 5 | Encoder vs. decoder vs. encoder-decoder | BERT-style vs. GPT-style vs. T5-style, and when each is used |
| 6 | Building a mini Transformer classifier | End-to-end PyTorch, compared against Module 6's RNN/LSTM results |
| 7 | Subword tokenization (BPE) | Why Transformers don't tokenize on whitespace |
| 8 | From scratch to pretrained | Why virtually nobody trains a Transformer from scratch in practice |
| 9 | Production: inference costs, KV-caching, quantization | The engineering reality of serving these models at scale |

</details>

<details>
<summary><strong>08 — Fine-Tuning Transformers</strong></summary>

| # | Topic | Why it matters |
|---|-------|------------------|
| 1 | Prompting vs. fine-tuning vs. RAG | The decision every real LLM project starts with |
| 2 | Loading & using a pretrained model | `AutoTokenizer` / `AutoModel*` — the standard entry point |
| 3 | Fine-tuning with the `Trainer` API | The high-level, production-standard training workflow |
| 4 | A manual PyTorch fine-tuning loop | What `Trainer` is actually doing underneath |
| 5 | Freezing layers / partial fine-tuning | Full fine-tune vs. feature-extraction vs. partial unfreeze |
| 6 | Learning rate warmup & scheduling | Why fine-tuning needs a different LR strategy than training from scratch |
| 7 | LoRA (Low-Rank Adaptation) | The modern, dominant technique for cheap, scalable fine-tuning |
| 8 | Other PEFT methods | Adapters, prefix tuning — the landscape beyond LoRA |
| 9 | Token classification (NER) fine-tuning | The other major fine-tuning shape, beyond sentence classification |
| 10 | Production: evaluation, forgetting, serving | Shipping a fine-tuned model safely |

</details>

<details>
<summary><strong>09 — RAG & LLM Application Patterns</strong></summary>

| # | Topic | Why it matters |
|---|-------|------------------|
| 1 | What RAG actually is, and why | The problem it solves that neither prompting nor fine-tuning solves alone |
| 2 | Chunking documents | How you break long text into retrievable pieces, and why chunk size matters |
| 3 | Building a simple retriever, step by step | The full "search my documents" pipeline, in plain, readable code |
| 4 | Building the augmented prompt | Turning retrieved chunks into something an LLM can actually use |
| 5 | The generation step | Where a real LLM call plugs in |
| 6 | Evaluating RAG quality | Retrieval metrics AND generation metrics — they measure different things |
| 7 | Advanced RAG: re-ranking, hybrid search, query rewriting | The upgrades real production RAG systems add |
| 8 | Vector databases in production | Where FAISS/Pinecone/Weaviate fit in, and why |
| 9 | Beyond RAG: agents, tool use, structured output | The wider landscape of how LLM products are actually built |

</details>

<details>
<summary><strong>10 — Summarization, Translation, QA & Evaluation</strong></summary>

| # | Topic | Why it matters |
|---|-------|------------------|
| 1 | Extractive summarization, from scratch | A real, working summarizer using only TF-IDF (Module 3) |
| 2 | Abstractive summarization | The pretrained-model approach, and how it differs |
| 3 | Machine translation | Encoder-decoder Transformers (Module 7) applied to translation |
| 4 | Question answering | Extractive QA (span-finding) vs. generative QA |
| 5 | BLEU, from scratch | The classic translation/generation metric — the actual math, not just a library call |
| 6 | ROUGE, from scratch | The classic summarization metric — ROUGE-N and ROUGE-L |
| 7 | BERTScore & perplexity | Semantic-similarity-based and probability-based metrics |
| 8 | LLM-as-judge | The metric most production teams actually lean on today |
| 9 | Choosing the right metric | A decision guide — different tasks need different metrics |
| 10 | Production evaluation pipelines | Regression testing generation quality over time |

</details>

---

## 🚀 How to Use These Notebooks

### 1. Get the files
Clone this repo, or just download the `.ipynb` files if that's all you have:
```bash
git clone https://github.com/unthinkingFool/NLP-journey.git nlp-mastery-journey
cd nlp-mastery-journey
```

### 2. Set up your environment
A virtual environment is strongly recommended so this doesn't collide with other Python projects on your machine.
```bash
python3 -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

pip install jupyter notebook
```
Each notebook lists its own dependencies in its **Setup** cell (Section 0), as commented-out `pip install` lines. Install them as you reach each notebook — don't install everything up front. As a rough guide:

| Notebooks | Core dependencies |
|-----------|----------------------|
| 01–03, 05 | `pandas`, `scikit-learn`, `numpy`, `matplotlib`, `beautifulsoup4`, `requests` |
| 04 | + `gensim` (Word2Vec/FastText), optionally `sentence-transformers` |
| 06–08 | + `torch` (CPU build is enough — see each notebook's Setup cell) |
| 08–09 | + `transformers`, `datasets`, `peft`, `faiss-cpu` (for the production templates) |
| 10 | + `rouge-score`, `sacrebleu`, `bert-score` (for the production templates — the from-scratch versions need nothing extra) |

### 3. Launch Jupyter
```bash
jupyter notebook
```
Or open the files in **VS Code**, **JupyterLab**, or upload them straight to **Google Colab** if you'd rather not install anything locally — every notebook is a single self-contained `.ipynb` file.

### 4. Work through them in order, and actually run the cells
This isn't meant to be read passively. Run every cell, read the comments as you go, and do the **"Try this before the next lesson"** exercises at the end of each notebook — that's where the material actually sticks.

### 5. A note on cells that are "commented out"
You'll notice some code cells — usually ones that call an external API, download a large model, or need an API key — are written correctly but left commented out (`# `) rather than run automatically. This is deliberate: it keeps every notebook safely runnable start-to-finish with no surprise downloads, costs, or network calls. **Uncomment and run those cells yourself** once you have the relevant API key / internet access / installed library.

---

## 🧩 Repo Structure

```
nlp-mastery-journey/
├── 01_NLP_Data_Acquisition.ipynb
├── 02_NLP_Text_Preprocessing.ipynb
├── 03_NLP_Text_Representation.ipynb
├── 04_NLP_Word_Sentence_Embeddings.ipynb
├── 05_NLP_Classical_Machine_Learning.ipynb
├── 06_NLP_Neural_Networks_RNN_LSTM.ipynb
├── 07_NLP_Transformer_Architecture.ipynb
├── 08_NLP_Fine_Tuning_Transformers.ipynb
├── 09_NLP_RAG_and_LLM_Patterns.ipynb
├── 10_NLP_Summarization_Translation_QA_Evaluation.ipynb
└── README.md   ← you are here
```

---

## ✅ Prerequisites

- **Comfortable with basic Python** (variables, functions, loops, lists/dicts). No prior ML or NLP knowledge needed — that's the whole point of Module 1.
- **No GPU required.** Every notebook is written to run on CPU; datasets are kept intentionally small so training finishes in seconds to minutes.
- **Curiosity, and a willingness to actually run the code**, not just read it.

---

## 🎯 Who This Is For

- Beginners who want a genuine **zero-to-advanced** path through NLP, not a scattered collection of tutorials.
- Developers who want **copy-paste-ready templates** for their next NLP project — every function in every notebook is written generically on purpose.
- Anyone who wants to understand **what's actually happening inside** attention, embeddings, BLEU/ROUGE, and LoRA — implemented from scratch, not just imported from a library.

---

## 🤝 Contributing & Feedback

Found a bug, an unclear explanation, or have a suggestion for a Module 11? Open an issue or a pull request — or better yet, reach out directly:

> ### 🔗 [**GitHub**](https://github.com/unthinkingFool) · [**LinkedIn**](https://www.linkedin.com/in/swapnil-das-603824236) 


---

<div align="center">

### If this repo helped you, the best way to say thanks is two clicks away 👇

**[⭐ Star this repo](https://github.com/unthinkingFool/NLP-journey)** &nbsp;·&nbsp; **[👤 Visit my profile](https://github.com/unthinkingFool)** &nbsp;·&nbsp; **[💼 Connect on LinkedIn](https://www.linkedin.com/in/swapnil-das-603824236)**

Made with care by **Swapnil Das**

</div>
