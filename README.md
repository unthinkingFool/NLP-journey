### 01_NLP_Data_Acquisition.ipynb
### What this notebook teaches
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

### 02_NLP_Text_Preprocessing.ipynb
### What this notebook teaches
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