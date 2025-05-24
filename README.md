# 🚀 GPT4All LangChain NL2SQL Enterprise

**Transform your natural language into SQL queries using local LLMs with enterprise database support**

[![GitHub](https://img.shields.io/badge/GitHub-dorialn68%2Fgtp4all--db--langchain--enterprise-blue?logo=github)](https://github.com/dorialn68/gtp4all-db-langchain-enterprise)
[![LangChain](https://img.shields.io/badge/LangChain-Enterprise%20Ready-green?logo=langchain)](https://python.langchain.com/)
[![GPT4All](https://img.shields.io/badge/GPT4All-Local%20LLM-orange)](https://gpt4all.io/)
[![Flask](https://img.shields.io/badge/Flask-Web%20App-red?logo=flask)](https://flask.palletsprojects.com/)

---

## 🎯 **Project Overview**

This project combines **GPT4All** local LLMs with **LangChain** to create an enterprise-grade Natural Language to SQL (NL2SQL) system. It features a complete Flask web application with multi-agent orchestration, iterative query refinement, and comprehensive GitHub automation tools.

### **Key Features:**
- 🤖 **Local LLM Integration** - GPT4All models for privacy and cost efficiency
- 🔄 **Multi-Agent Orchestration** - AutoGen-based iterative query refinement
- 🌐 **Modern Web Interface** - Beautiful Flask app with real-time chat
- 📊 **Database Connectivity** - SQLite, PostgreSQL, and Vertica support
- 🛠️ **GitHub Automation** - PowerShell scripts for streamlined development
- 📈 **Natural Language Responses** - Human-friendly explanations of query results

### **Current Capabilities:**
- ✅ **Automatic SQL vs NL detection** - Smart query classification
- ✅ **Multi-turn conversation** - Context-aware query refinement
- ✅ **Error handling & recovery** - Automatic SQL error correction
- ✅ **Real-time web interface** - Interactive chat with suggestions
- ✅ **Local model support** - GPT4All Phi-3, Orca, and other models

---

## 🛠️ **GitHub Automation Tools**

This project includes powerful automation scripts to streamline your development workflow:

### **🎮 Interactive Menu (`github-automation.ps1`)**

**Full-featured automation with interactive menu:**

```powershell
# Launch interactive menu
.\github-automation.ps1

# Or use direct commands
.\github-automation.ps1 -Action save -Message "Implemented SQL agent"
.\github-automation.ps1 -Action feature
.\github-automation.ps1 -Action status
```

**Menu Features:**
- 🌐 **GitHub Operations**: Open repo, branches, PRs, issues, actions
- 🌿 **Branch Management**: Switch branches, create new ones
- 💾 **Commit & Push**: Quick save, custom messages, commit-only
- 🔄 **Workflows**: Start feature development, create PRs, emergency push
- 📊 **Information**: Git status, repository info

### **⚡ Ultra-Fast Shortcuts (`quick-shortcuts.ps1`)**

**Load once, use everywhere:**

```powershell
# Load shortcuts into your PowerShell session
. .\quick-shortcuts.ps1

# Now use one-word commands:
github           # Open main repository
github-feature   # Open feature branch
quick-save       # Add, commit, push with timestamp
start-work       # Switch to feature + open GitHub
end-work         # Save work + open GitHub
to-feature       # Switch to feature branch
shortcuts        # Show all available commands
```

---

## 🚀 **Quick Start Guide**

### **1. Clone Repository**
```bash
git clone https://github.com/dorialn68/gtp4all-db-langchain-enterprise.git
cd gtp4all-db-langchain-enterprise
```

### **2. Install Dependencies**
```bash
# Create virtual environment
python -m venv .venv
.venv\Scripts\activate  # Windows
# source .venv/bin/activate  # Linux/Mac

# Install requirements
pip install flask flask-cors
pip install langchain langchain-community
pip install sqlite3
```

### **3. Download GPT4All Models**
```bash
# Download models to project directory
# Phi-3 Mini (2.2GB) - Recommended
# Orca Mini (1.8GB) - Alternative
```

### **4. Run the Application**
```bash
# Start Flask web server
python app/app.py

# Open browser to http://localhost:5000
```

### **5. Start Using Automation**
```powershell
# Load shortcuts for ultra-fast commands
. .\quick-shortcuts.ps1

# Start working
start-work

# Make changes, then save quickly
quick-save

# Or use the full menu system
.\github-automation.ps1
```

---

## 📁 **Project Structure**

```
gtp4all-db-langchain-enterprise/
├── 📄 README.md                     # This file
├── 🚀 github-automation.ps1         # Full automation script with menu
├── ⚡ quick-shortcuts.ps1           # Ultra-fast one-word commands
├── 📋 PROJECT_PLAN.md               # Original project plan
├── 📋 CHECKPOINTS.md                # Development milestones
├── ⚙️ .gitignore                    # Git ignore patterns
│
├── 📂 app/                          # Flask Web Application
│   ├── app.py                       # Main Flask server
│   ├── autogen_iterative.py         # Multi-agent orchestrator
│   ├── natural_language_responder.py # NL response generation
│   ├── database.py                  # Database connectivity
│   └── __init__.py                  # Package initialization
│
├── 📂 tests/                        # Testing Suite
│   ├── test_api.py                  # API endpoint tests
│   ├── test_db.py                   # Database tests
│   ├── test_simple.py               # Basic functionality tests
│   ├── test_complex.py              # Advanced query tests
│   └── validate_system.py           # System validation
│
├── 📂 models/                       # GPT4All Models (downloaded)
│   ├── Phi-3-mini-4k-instruct-q4.gguf
│   └── q4_0-orca-mini-3b.gguf
│
└── 📂 data/                         # Sample Databases
    ├── Chinook_Sqlite.sqlite        # Sample database
    └── chinook.zip                  # Database backup
```

---

## 🎮 **Automation Commands Reference**

### **🌐 One-Click GitHub Operations**
| Command | Action | Example |
|---------|--------|---------|
| `github` | Open main repository | `github` |
| `github-feature` | Open feature branch | `github-feature` |
| `github-prs` | Open pull requests | `github-prs` |
| `github-issues` | Open issues page | `github-issues` |

### **💾 Quick Save Operations**
| Command | Action | Example |
|---------|--------|---------|
| `quick-save` | Add, commit, push with timestamp | `quick-save` |
| `emergency-save` | Emergency save with alert | `emergency-save` |
| `end-work` | Save with custom message | `end-work "Implemented SQL agent"` |

### **🌿 Branch Management**
| Command | Action | Example |
|---------|--------|---------|
| `to-main` | Switch to main branch | `to-main` |
| `to-feature` | Switch to feature branch | `to-feature` |
| `to-dev` | Switch to development | `to-dev` |
| `start-work` | Switch to feature + open GitHub | `start-work` |

### **📊 Status & Info**
| Command | Action | Example |
|---------|--------|---------|
| `git-status` | Show current git status | `git-status` |
| `shortcuts` | Show all available commands | `shortcuts` |

---

## 🛠️ **Dependencies & Installation**

### **Core Dependencies**
```bash
# Web Framework
pip install flask flask-cors

# LangChain & AI
pip install langchain langchain-community langchain-experimental

# Database Support
pip install sqlite3 sqlalchemy
pip install psycopg2-binary  # PostgreSQL

# Local LLM Support
# GPT4All models downloaded separately
```

### **GPT4All Model Setup**
1. **Download Models**: Place in project root
   - `Phi-3-mini-4k-instruct-q4.gguf` (2.2GB)
   - `q4_0-orca-mini-3b.gguf` (1.8GB)

2. **Model Configuration**: Update paths in `app/ollama_integration.py`

---

## 📈 **System Capabilities**

### **Multi-Agent Processing**
- **Query Analyzer**: Classifies SQL vs Natural Language
- **SQL Generator**: Creates optimized SQL queries
- **Error Handler**: Fixes syntax and logical errors
- **Result Formatter**: Generates natural language explanations

### **Web Interface Features**
- **Real-time Chat**: Interactive conversation interface
- **Query Suggestions**: Context-aware recommendations
- **Result Visualization**: Tables and natural language summaries
- **Error Recovery**: Automatic query refinement

### **Database Support**
- **SQLite**: File-based databases (development)
- **PostgreSQL**: Enterprise database (production)
- **Vertica**: Analytics database (planned)

---

## 🎯 **Use Cases**

### **Business Intelligence**
```
User: "Show me top 5 customers by revenue this quarter"
System: Generates SQL, executes query, explains results
```

### **Data Exploration**
```
User: "What tables contain customer information?"
System: Analyzes schema, lists relevant tables and columns
```

### **Report Generation**
```
User: "Compare sales by region for last 3 months"
System: Creates complex JOIN queries, formats results
```

---

## 🤝 **Contributing**

1. **Create feature branch**: `git checkout -b feature/your-feature`
2. **Make changes**: Edit code, test thoroughly
3. **Quick save**: Use `quick-save` or `end-work "Description"`
4. **Create PR**: Use `./github-automation.ps1` → option 15

---

## 📞 **Support & Contact**

- **GitHub Issues**: [Report bugs or request features](https://github.com/dorialn68/gtp4all-db-langchain-enterprise/issues)
- **Discussions**: [Ask questions or share ideas](https://github.com/dorialn68/gtp4all-db-langchain-enterprise/discussions)
- **Project Owner**: [@dorialn68](https://github.com/dorialn68)

---

## 📜 **License**

MIT License - see [LICENSE](LICENSE) file for details.

---

## 🚀 **Get Started Now!**

```powershell
# 1. Clone repository
git clone https://github.com/dorialn68/gtp4all-db-langchain-enterprise.git
cd gtp4all-db-langchain-enterprise

# 2. Setup environment
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt

# 3. Load automation tools
. .\quick-shortcuts.ps1

# 4. Start development
start-work

# 5. Run the application
python app/app.py
```

**🎯 Ready to query your data with natural language? Let's build something amazing! 🚀**