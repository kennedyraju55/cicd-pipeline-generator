# 🚀 cicd-pipeline-generator

Auto-generate CI/CD pipelines for any tech stack — privacy-first, locally-powered

[![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org)
[![Ollama](https://img.shields.io/badge/Ollama-Local%20LLM-green)](https://ollama.com)
[![Gemma 3](https://img.shields.io/badge/Gemma%203-Language%20Model-orange)](https://ollama.com/library/gemma2)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow)](./LICENSE)
[![Privacy First](https://img.shields.io/badge/Privacy-First-darkgreen)](#why-local)

## 🎯 What it does

- Generate complete CI/CD pipeline configurations (GitHub Actions, GitLab CI, Jenkins) from simple descriptions
- Supports multiple tech stacks: Node.js, Python, Go, Java, Rust, Docker-based apps
- Creates optimized pipelines with testing, linting, building, and deployment stages
- All processing happens locally — your pipeline configs never leave your machine

## 🛠️ Tech Stack

- Streamlit (Web UI)
- FastAPI (Backend API)
- Ollama (Local LLM inference)
- Gemma 3 (Language model)
- Python 3.8+

## ⚡ Quick Start

1. **Clone the repository**
   \\\ash
   git clone https://github.com/kennedyraju55/cicd-pipeline-generator.git
   cd cicd-pipeline-generator
   \\\

2. **Install dependencies**
   \\\ash
   pip install -r requirements.txt
   \\\

3. **Download and start Ollama**
   - Download from [ollama.com](https://ollama.com)
   - Start Ollama service:
   \\\ash
   ollama serve
   \\\
   - In another terminal, pull Gemma 3:
   \\\ash
   ollama pull gemma2
   \\\

4. **Run the application**
   \\\ash
   streamlit run app.py
   \\\

Access the app at: http://localhost:8501

## 🏗️ Architecture

\\\
User describes pipeline needs → Streamlit UI → FastAPI processes request → Ollama generates config using Gemma 3 → Returns complete YAML/JSON → Download directly
\\\

All processing happens locally on your machine. No data is sent to external services.

## 🔒 Why Local?

CI/CD pipeline configs often contain sensitive build secrets, deployment credentials, and infrastructure details. Generating these locally ensures your deployment strategies, service endpoints, and infrastructure topology remain completely private.

## 📦 Environment Variables

Create a \.env\ file in the project root:

\\\nv
OLLAMA_BASE_URL=http://localhost:11434
MODEL_NAME=gemma2
LOG_LEVEL=INFO
\\\

## 🤝 Contributing

We love contributions! Here's how to help:

1. Fork the repository
2. Create a feature branch: \git checkout -b feature/your-feature\
3. Make your changes and commit: \git commit -am 'Add feature'\
4. Push to the branch: \git push origin feature/your-feature\
5. Submit a Pull Request

Please ensure:
- Code follows PEP 8 style guidelines
- Changes include appropriate comments
- Updates to documentation are included

## 📄 License

This project is licensed under the MIT License — see [LICENSE](./LICENSE) for details.

---

**Part of 114+ privacy-first AI tools by [Nrk Raju](https://github.com/kennedyraju55)**