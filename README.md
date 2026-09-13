# JNTUH AI Predicted Paper Engine

RAG + CNN-OCR powered, 3-stage AI pipeline that generates two exam-ready predicted question papers (Set A / Set B) for any JNTUH R22 subject — with Bloom's taxonomy tagging, ★ repetition-frequency ratings, HTML dropdown solutions, marking rubrics, a self-assessment scorecard, and PDF/JPG/Markdown export.

**Designed and developed by Nikhil Chary Sriramoju**
- GitHub: https://github.com/Nikhil-creat
- LinkedIn: https://in.linkedin.com/in/nikhil-chary-sriramoju-95041b38a
- Email: sriramojunikhil66@gmail.com

## Features
- Works for BOTH JNTUH R22 papers and Autonomous college papers (custom pattern input)
- Bring-your-own API key (Anthropic Claude or Google Gemini) — works standalone on GitHub Pages
- Subject-agnostic — works for any JNTUH R22 subject
- RAG retrieval engine (TF-IDF chunk ranking) over syllabus + PYQ text
- CNN-OCR fallback (Tesseract) for scanned/image-only PYQ pages
- 3-stage AI pipeline: deep frequency analysis → generation → self-verification
- ★ star rating on questions based on PYQ repetition frequency
- Difficulty calibration: pass-focus / balanced / distinction-push
- Live confidence dashboard (prediction confidence %, years analyzed, coverage %)
- Export: Markdown, PDF, JPG
- Single static file — no backend, no build step

## Run locally
Just open `index.html` in a browser.

## Deploy on GitHub Pages
See the deployment guide provided with this project, or:
1. Push these files to a GitHub repo
2. Settings → Pages → Source: `main` branch, `/root`
3. Live at `https://<your-username>.github.io/<repo-name>/`

## ⚠️ Note on API usage
This page calls the Anthropic API directly from the browser. Since GitHub Pages is public, anyone with the link can trigger calls billed to your key. Keep the link private, or add an access gate, before sharing widely.
