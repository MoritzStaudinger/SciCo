# SciCo: A Dataset for Institutional and Publication Level Comparisons of Scientific Contributions

**SciCo** is a novel dataset designed for structured, comparative analysis of scientific publications and institutions. It combines full-text research papers with rich metadata (including author affiliations, countries, topics, and more) to enable query-driven multi-document comparisons across institutions and publication venues. SciCo is particularly suited for benchmarking contributions, tracking topic evolution, and exploring overlaps in research agendas.

## 📂 Dataset Overview

The dataset consists of:
- **Corpus file** (JSON): Full-texts with detailed metadata for 12,610 unique publications (2015–2025).
- **Question files** (JSON): 97 curated queries to guide comparative analyses (e.g., comparing universities, summarizing institutional contributions, tracking topic trends).

### Example Corpus Entry
```json
{
  "title": "MinTL: Minimalist Transfer Learning ...",
  "authors": ["Zhaojiang Lin", "..."],
  "abstract": "...",
  "DOI": "10.18653/v1/2020.emnlp-main.273",
  "publication_year": 2020,
  "language": "en",
  "affiliations": ["University of Hong Kong", "..."],
  "countries": ["HK"],
  "keywords": ["Transfer of learning"],
  "topic": "Speech and dialogue systems",
  "pdf_path": "2020.emnlp-main.273.pdf",
  "local_pdf_path": "pdfs/2020.emnlp-main.273.pdf",
  "fulltext": "..."
}
```

### Example Query
```json
{
    "question": "What did MIT ...",
    "question_type": "overview_university",
    "topic": "Syntax and Morphology",
    "uni1": "MIT",
    "uni2": "",
    "year_start": "2019",
    "year_end": "2025",
    "country": "",
    ...
}
```

### Fulltext
As the fulltext is too big, to be hosted on Github, it is available for download from [Google Drive](https://drive.google.com).


## License

This project is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-nc-sa/3.0/).
