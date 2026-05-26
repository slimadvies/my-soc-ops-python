🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# 🎮 Soc Ops — Social Bingo for Mixers

**Break the ice at any event.** Soc Ops is an interactive bingo game that gets people talking, laughing, and connecting at in-person gatherings. Players mingle to find others matching bingo prompts, building genuine connections while competing for five in a row.

> **Also:** A hands-on GitHub Copilot agent lab for learning modern AI-assisted development with Python, FastAPI, and Jinja2.

---

## ✨ What's It For?

### 🎯 **Event Hosts & Facilitators**
Turn awkward mingling into genuine connection. Soc Ops creates natural conversation starters, encourages movement across the room, and keeps energy high.

### 👨‍💻 **Developers Learning Copilot**
A complete, production-like workshop app that teaches:
- Building interactive web apps with **FastAPI** & **Jinja2**
- Designing UX with **Copilot** agents (Design-First workflow)
- Building custom **agent skills** for domain-specific workflows
- Multi-agent systems and advanced prompt engineering
- Testing, linting, and best practices

---

## 🚀 Quick Start

### For Event Hosts
```bash
# Install dependencies
uv sync

# Run the app
uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```
Then open [http://localhost:8000](http://localhost:8000) in your browser. Print the bingo cards, and let the mingling begin!

### For Copilot Lab Participants
Start with **[Part 00: Overview](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview)** to set up your environment and understand the workshop structure.

---

## 📚 Copilot Agent Lab

Hands-on learning across 5 guided parts (2–3 hours total).

| Part | Learning Goal | Duration |
|------|---------------|----------|
| [**00**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview) | Overview & Setup Checklist | — |
| [**01**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=01-setup) | Context Engineering & Workspace Setup | 15 min |
| [**02**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=02-design) | Design-First Frontend with AI | 15 min |
| [**03**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=03-quiz-master) | Building Custom Quiz Master Agent | 10 min |
| [**04**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=04-multi-agent) | Multi-Agent Systems & Orchestration | 20 min |

**📝 Prefer offline?** Guides are in the [`workshop/`](workshop/) folder with full instructions and references.

---

## 🛠️ Tech Stack

- **Backend:** FastAPI (Python 3.13+)
- **Frontend:** Jinja2 templates + HTMX + CSS utilities
- **Game Logic:** Rule-based state machine
- **Testing:** pytest + httpx
- **Quality:** Ruff linter

---

## 📂 Project Structure

```
soc-ops/
├── app/
│   ├── main.py              # FastAPI routes
│   ├── game_service.py      # Game state & session management
│   ├── game_logic.py        # Bingo rules & validation
│   ├── models.py            # Data schemas
│   ├── data.py              # Initial game prompts
│   ├── templates/           # Jinja2 HTML templates
│   └── static/              # CSS, images, client-side assets
├── tests/                   # pytest test suite
├── workshop/                # Copilot agent lab guides
├── pyproject.toml           # Dependencies & configuration
└── README.md                # You are here
```

---

## 🧪 Run Tests & Linting

```bash
# Check code quality
uv run ruff check .

# Run test suite
uv run pytest
```

---

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## 📄 License & Support

- **License:** [MIT](LICENSE)
- **Code of Conduct:** [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
- **Security:** [SECURITY.md](SECURITY.md)
- **Support:** [SUPPORT.md](SUPPORT.md)

---

## 🎓 Learning Resources

- [FastAPI Docs](https://fastapi.tiangolo.com/)
- [GitHub Copilot Agents Intro](https://github.blog/ai-and-ml/github-copilot/)
- [Jinja2 Template Engine](https://jinja.palletsprojects.com/)

---

**Ready to build?** Start with [Part 00](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview) → [Setup](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=01-setup) → [Create your first feature with AI](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=02-design)! 🚀
