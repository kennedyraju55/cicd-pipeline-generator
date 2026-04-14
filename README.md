# 🔧 CI/CD Pipeline Generator

Generate production-ready CI/CD pipeline configurations in seconds.

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![Ollama](https://img.shields.io/badge/Ollama-Compatible-green.svg)](https://ollama.com)
[![Gemma 3](https://img.shields.io/badge/Gemma-3-orange.svg)](https://ollama.com)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Privacy First](https://img.shields.io/badge/Privacy-First-red.svg)](#why-local)

## What It Does

- **Auto-generates CI/CD configs** for GitHub Actions, GitLab CI, Jenkins, and more
- **Intelligent templates** tailored to your tech stack and requirements
- **No cloud dependencies** — all generation happens locally on your machine
- **Customizable outputs** with variable interpolation and conditional steps

## Tech Stack

- **Python 3.8+** — Core generation engine
- **Gemma 3** (via Ollama) — LLM-powered config intelligence
- **Jinja2** — Template rendering
- **PyYAML** — Pipeline configuration parsing

## Quick Start

`ash
# Clone the repository
git clone https://github.com/kennedyraju55/cicd-pipeline-generator.git
cd cicd-pipeline-generator

# Install dependencies
pip install -r requirements.txt

# Pull Gemma 3 model locally
ollama pull gemma3:4b

# Generate a CI/CD pipeline
python generator.py --platform github-actions --language python
`

## Architecture

`
input (tech stack, requirements)
    ↓
[Gemma 3 LLM Processing] ← offline, local
    ↓
template + config rules
    ↓
YAML/JSON output (ready to use)
`

## Why Local?

- **Security**: Your pipeline configs stay on your machine — no upload to external services
- **Privacy**: No SaaS vendor has visibility into your infrastructure setup
- **Speed**: Instant generation without API latency
- **Reliability**: Works offline, independent of cloud availability

## Contributing

Contributions welcome! Please fork, create a feature branch, and submit a pull request.

## License

MIT License — see [LICENSE](LICENSE) for details.

---

*Part of 114+ privacy-first AI tools by Nrk Raju*