# 🧠 AI Prompt Library

A curated, searchable collection of prompts for Claude, GPT, DeepSeek, Gemini, and more. Copy what works, add your own.

**Zero dependencies. One HTML file. Works offline.**

## Features

- **Searchable** — Instantly search across titles, descriptions, tags, categories, and prompt text
- **Tagged & Filtered** — Filter by category (coding, writing, analysis, etc.) or target LLM (Claude, GPT, DeepSeek, Gemini, etc.)
- **Copy-to-Clipboard** — One-click copy of any prompt, ready to paste into your LLM
- **Add Your Own** — Use the "＋ Add Prompt" button to add and save custom prompts (persisted in localStorage)
- **Export / Import** — Export your custom prompts as JSON and import them on another machine
- **Responsive** — Works on desktop and mobile browsers

## Supported Models

Works with any LLM. Curated prompts target:

| LLM | Prompts |
|---|---|
| **Any** (model-agnostic) | Most prompts |
| Claude | Refactoring, blog writing, UI copy, research |
| GPT | General-purpose prompts |
| DeepSeek | Coding & analysis prompts |
| Gemini | General-purpose prompts |

## Quick Start

1. **Clone or download** the repository
2. **Open `index.html`** in any modern browser
3. **Browse, search, and copy** prompts
4. **Add your own** via the "＋ Add Prompt" button

No server, no build step, no installation — just open the file.

## Tech Stack

- **Single file** — Everything lives in `index.html`
- **Zero dependencies** — Pure HTML, CSS, and vanilla JavaScript
- **localStorage** — Custom prompts persist across sessions
- **No framework, no bundler, no server**

## Project Structure

```
ai-prompt-library/
└── index.html    ← the entire app (~400 lines)
```

## Categories

The library includes 30 curated prompts spanning:

- **Coding** — debugging, code review, refactoring, API design, Git, shell scripts, Docker, CRON
- **SAP** — SuccessFactors EC configuration, audit diff analysis, position management, picklist migration
- **Writing** — blog posts, LinkedIn content, README generation, personal branding
- **Productivity** — meeting notes, weekly reviews
- **Analysis** — data analysis planning, competitive analysis, decision matrices, UK property
- **Creative** — UI microcopy, product naming
- **Education** — UK lesson plans, 11+ exam questions
- **DevOps** — Docker Compose generation
- **Research** — academic paper summarization
- **AI Tools** — Hermes Agent skill authoring

## Contributing

Want to add prompts or improve the library?

1. **Fork** this repository
2. **Add your prompts** directly in the `SEEDS` array in `index.html`, or use the in-app "＋ Add Prompt" feature and export the JSON
3. **Submit a Pull Request**

Prompt format for the `SEEDS` array:

```js
{
  id: "s99",
  title: "My Awesome Prompt",
  description: "What this prompt is good for",
  category: "coding",
  llm: "any",
  tags: ["python", "debugging"],
  prompt: "Your prompt text goes here..."
}
```

Guidelines:
- Keep prompts **specific and actionable**
- Use **lowercase, hyphenated** tag names
- Choose from existing **categories** or add a new one if justified
- Set `llm` to `"any"` for model-agnostic prompts, or specify (`"claude"`, `"gpt"`, `"deepseek"`, `"gemini"`)

## License

MIT
