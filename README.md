# 📊 Gleam Deck – Auto-Generate a Presentation from Text

**Your Text, Your Style – Turn bulk text or markdown into a polished PowerPoint presentation.**

Gleam Deck is a lightweight web app that lets anyone paste long-form text (markdown, prose, notes, reports) and instantly convert it into a styled, ready-to-present PowerPoint deck. Simply upload your own template, add optional guidance, and supply your preferred LLM API key — the app will handle the rest.

---

## ✨ Features

- 📝 **Input Options**: Paste large chunks of text, markdown, or prose.
- 🎯 **Guidance**: Add a one-line instruction for tone or structure (e.g., “make it an investor pitch deck”).
- 🔑 **Bring Your Own API Key**: Supports OpenAI, Anthropic, Gemini, and more (keys are never stored or logged).
- 🎨 **Template Reuse**: Upload your `.pptx` or `.potx` template to apply colors, fonts, and layouts.
- 🖼️ **Image Reuse**: Recycles existing images from your uploaded template.
- 📥 **Instant Download**: Outputs a new `.pptx` file you can download directly.
- ⚡ **Smart Splitting**: Automatically divides input text into a reasonable number of slides.
- 🔒 **Privacy First**: No logging or saving of user text, API keys, or files.

---

## 🚀 Quick Start

git clone https://github.com/yourusername/gleamdeck.git
cd gleamdeck
pip install -r requirements.txt
uvicorn app:app --reload


## Live at 

Visit: [http://localhost:8000](http://localhost:8000)

Or try the live demo at: [https://pptx-generator-dftp.onrender.com/](https://pptx-generator-dftp.onrender.com)

---

## 🖥 Usage

1. Paste your text or markdown.
2. (Optional) Add a one-line guidance prompt (e.g., “make it a research summary”).
3. Paste your LLM API key (e.g., OpenAI, Anthropic, Gemini).
4. Upload a `.pptx` or `.potx` template file.
5. Click **Generate** and download your styled PowerPoint deck.

---

## 🏗 Architecture

- **Frontend**: Responsive UI using Tailwind CSS; handles input, template upload, and download.
- **Backend**: FastAPI application that processes text, splits it into slide sections, maps content to the template styles, and generates `.pptx` files using `python-pptx`.

---

## 🔮 Future Enhancements

- Auto-generate speaker notes.
- Built-in guidance templates (e.g., sales pitch, investor deck).
- Live slide previews before download.
- Enhanced error handling and retry logic for API calls.

---

## 📄 License

MIT License — free for personal and commercial use.

---

## 📧 Contact

For questions or contributions, see the [GitHub repo](https://github.com/yourusername/gleamdeck).
