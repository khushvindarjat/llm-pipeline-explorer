# LLM Pipeline Explorer 🚀

An interactive web application exploring how Large Language Models (LLMs) transform raw natural language text into tokens, high-dimensional vector embeddings, and 3D geometric projections.

Inspired by and built as a faithful enhancement of the LLM Pipeline Explorer.

![LLM Pipeline Explorer](https://img.shields.io/badge/Made%20with-Vanilla%20HTML%20%2F%20JS-blue)
![Plotly](https://img.shields.io/badge/3D%20Graphics-Plotly.js-orange)
![Deployable](https://img.shields.io/badge/Deploy-Vercel%20%7C%20GitHub%20Pages-green)

---

## 🌟 Features

1. **Subword BPE Tokenizer**:
   - Dynamic vocabulary extraction from arbitrary training corpora with word frequency calculation.
   - Interactive vocabulary size slider: shrink vocabulary to watch out-of-vocabulary words break down into subwords (prefixed with `##`) and individual characters.
   - Visual colored token chips with unique integer token IDs and compression ratio (`characters / token`).
   - Special `[UNK]` handling for unmapped tokens.

2. **64-Dimensional Trigram Sentence Embeddings**:
   - Computes L2-normalized 64-dimensional character trigram vectors using deterministic hashing.
   - Pairwise Cosine Similarity matrix calculation for all input sentences.

3. **In-Browser 3D PCA Projection**:
   - Implements Principal Component Analysis directly in JavaScript:
     - Mean-centering
     - Covariance matrix computation
     - Power iteration with deflation to extract top 3 eigenvectors
   - High-performance interactive 3D scatter plot using Plotly (rotate, zoom, pan, hover tooltips).

4. **Interactive Sentence Tracer**:
   - Type any custom sentence or word to follow its step-by-step path:
     - **Step 1:** Subword tokenization and ID assignment.
     - **Step 2:** 64-D vector spectrum visualization and preview.
     - **Step 3:** Dynamic projection into 3D space as an orange diamond with nearest neighbor similarity ranking.

5. **Modern Polished UI**:
   - Single-file `index.html` with zero build step.
   - Dark mode & Light mode support.
   - Preset buttons for quick testing.

---

## 💻 Quick Start

Simply open `index.html` in any web browser!

Or serve locally with any static server:
```bash
# Using Python
python3 -m http.server 3000

# Using Node.js npx
npx serve .
```

Open `http://localhost:3000` in your browser.

---

## 🚀 Deployment

### Deploy to Vercel

You can deploy directly using Vercel CLI:
```bash
npx vercel
```
Or connect this GitHub repository in your [Vercel Dashboard](https://vercel.com/new).

---

## 📄 License
MIT License
