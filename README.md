

# Gyaan Deck: Instantly Turn Text into Beautiful PowerPoint Presentations

**Transform your notes, markdown, or reports into a polished, styled PowerPoint deck in seconds.**

---

## 🚩 What is Gyaan Deck?

Gyaan Deck is a simple web app that converts long-form text (markdown, prose, notes, reports) into a ready-to-present PowerPoint file. Just paste your content, add optional guidance, upload your favorite template, and provide your LLM API key—Gyaan Deck does the rest.

---

## ✨ Key Features

- **Flexible Input:** Paste text, markdown, or prose of any length.
- **Guidance:** Add a one-line instruction for tone or structure (e.g., “make it an investor pitch deck”).
- **Bring Your Own API Key:** Supports OpenAI, Anthropic, Gemini, and more. (Your keys are never stored.)
- **Template Support:** Upload your `.pptx` or `.potx` to apply your own colors, fonts, and layouts.
- **Image Reuse:** Automatically reuses images from your uploaded template.
- **Instant Download:** Get a `.pptx` file ready to present.
- **Smart Slide Splitting:** Automatically divides your content into a reasonable number of slides.
- **Privacy First:** No logging or saving of your text, keys, or files.

---

## ⚡ Quick Start

1. **Clone the repository:**
  ```bash
  git clone https://github.com/23f1000805/tds-bonus-project-Auto-PPT-Generator-GyaanSetu-Deck.git
  cd tds-bonus-project-Auto-PPT-Generator-GyaanSetu-Deck
  ```
2. **Install dependencies:**
  ```bash
  # Backend (Python FastAPI + pptx libraries)
  pip install -r requirements.txt
  # Frontend (static HTML/JS/CSS, no build step needed)
  ```
3. **Run locally:**
  ```bash
  uvicorn app:app --reload
  ```
  Visit: [http://localhost:8000](http://localhost:8000)
4. **Deploy:**
  - Works out-of-the-box on Railway, Render, Vercel, Heroku, and similar platforms. Just connect your repo and deploy.

---

## 🖥️ How to Use

1. Paste your text or markdown.
2. (Optional) Add a one-line guidance (e.g., “make it a research summary”).
3. Paste your LLM API key (OpenAI, Anthropic, Gemini, etc.).
4. Upload a `.pptx` or `.potx` template.
5. Click **Generate** and download your styled PowerPoint deck!

---

## 🏗️ Architecture Overview

**Frontend:**
- Responsive HTML + Tailwind UI
- Handles text input, template upload, and file download
- Provides toasts, progress feedback, and a history of past generations

**Backend (FastAPI):**
- Accepts text, guidance, API key, and template
- Splits input into slide sections
- Maps new content onto your template’s style, layout, fonts, and images
- Generates `.pptx` output using `python-pptx`

---

## � Potential Enhancements

- Auto-generate speaker notes
- Offer prebuilt guidance templates (sales deck, investor pitch, research summary, etc.)
- Live slide previews before download
- Improved error handling and retry logic for unstable APIs

---

## 📄 License

MIT License – free to use, modify, and share.

