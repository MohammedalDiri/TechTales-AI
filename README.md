# 📚 TechTales-AI

**TechTales-AI** is an interactive AI storytelling chatbot that explains technical and abstract ideas using fun narrative styles like fairytales, sci-fi missions, detective mysteries, and kid-friendly analogies. It runs on OpenAI's GPT or Anthropic's Claude, using a clean Gradio interface.

---

## ✨ Features

- 🧠 Choose your storytelling style:
  - Classic Explanation
  - Fairytale
  - Sci-Fi
  - Detective Mystery
  - Kids Version
- 🤖 Use GPT or Claude as the engine
- 💬 Interactive, streamed chat responses
- 🌐 Gradio interface (in-browser)
- 🔧 Easily extend with new styles, models, or tools

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/TechTales-AI.git
cd TechTales-AI
```

### 2. Install Dependencies

Install the required Python libraries:

```bash
pip install openai anthropic gradio python-dotenv
```

### 3. Add Your API Keys

Create a `.env` file in the root folder with your keys:

```
OPENAI_API_KEY=your-openai-api-key
ANTHROPIC_API_KEY=your-anthropic-api-key
```

🔐 **Note**: Keep this file private. Do NOT upload it to GitHub.

---

## 🧪 Running the App

You can launch the notebook and run the final cell:

```python
demo.launch(share=True, inbrowser=True)
```

Or convert it to a script and run it:

```bash
jupyter nbconvert --to script TechTales.ipynb
python TechTales.py
```

---

## 🧠 How It Works

- Story modes are defined in `system_prompts`
- Each user message is combined with history and sent to the selected model
- Streaming response is displayed live in the Gradio chat
- Modular design to support future features like text-to-speech or style-based voices

---

## 🛠️ Files

```
TechTales-AI/
├── TechTales.ipynb        # Main interactive notebook
├── .env                   # API keys (not included)
├── README.md              # Project description
```

---

## ⚙️ Customization

- Add more creative story styles in the `system_prompts` dictionary
- Replace or extend LLMs in `generate_response()`
- Optionally add text-to-speech using Gradio’s `audio` component or Azure/Vox APIs

---

## 💡 Contributions

Got a cool storytelling style idea? PRs are welcome!
