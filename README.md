# LatentStudio 🔬

**Interactive LLM Tokenization, High-Dimensional Vector Embeddings & 3D Latent Space Explorer**

A self-contained web laboratory exploring how Large Language Models (LLMs) turn raw natural language into subwords, continuous vectors, and geometric semantic projections.

---

## 🌟 What Makes This Distinct

- **Modern Studio Interface**: Sleek tabbed workspace dividing the workflow into **1. Tokenizer & Subword Engine**, **2. 3D Latent Space & Clusters**, and **3. Custom Sentence Tracer**.
- **Fresh Multi-Domain Corpus**: Real-world knowledge bases spanning Deep Learning & AI, Astrophysics, Marine Biology, and Philosophy.
- **In-Browser 3D Projection**: Custom PCA (Principal Component Analysis) implementation running purely in client-side JavaScript, rendered with Plotly.js.
- **Single-File Architecture**: Everything is contained in [`index.html`](index.html) with zero build systems or node dependencies needed.

---

## 🚀 How to Run Locally

Simply open `index.html` in any web browser!

Or spin up a local server:
```bash
# Python
python3 -m http.server 3000

# Node / NPX
npx serve .
```
Then visit `http://localhost:3000`.

---

## 📦 How to Deploy It Yourself

Because `index.html` is completely static and self-contained, you can deploy it to any hosting platform in seconds:

### Option 1: Vercel
1. Install Vercel CLI or visit [vercel.com](https://vercel.com).
2. Run in this directory:
   ```bash
   vercel
   ```
   Or import this repository directly in your Vercel Dashboard.

### Option 2: GitHub Pages
1. Go to your repository **Settings** → **Pages**.
2. Under **Build and deployment**, select `Deploy from a branch` (Branch: `main`, Folder: `/ (root)`).
3. Click **Save**.

### Option 3: Netlify / Cloudflare Pages
Drag and drop this folder into the Netlify or Cloudflare Pages web interface.

---

## 📄 License
MIT
