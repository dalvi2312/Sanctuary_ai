# SanctuaryAI 🕊️

**SanctuaryAI** — A compassionate AI mental-health companion that listens, understands, and responds with empathy. Built as a safe-space assistant powered by agent orchestration, specialist healthcare models, and practical integrations (e.g., Twilio for emergency escalation).

---

## Key features ✨
- 🤖 **Agent-driven architecture** to coordinate tasks and responses  
- 🩺 **Specialist healthcare models** for clinically-informed replies  
- 🚨 **Emergency escalation** via Twilio (calls/SMS) when necessary  
- 📍 **Location-aware resources** to provide region-specific help (with consent)  
- 🧩 **Lightweight Python codebase** with clear frontend & backend entry points

---

## Key highlights (project goals & capabilities) 🔎
- 🔁 Switches to **Specialist Mode** using local LLM runtimes (e.g., Ollama) and specialist models (e.g., MedGemma) for higher-fidelity clinical guidance.  
- 📞 Detects emergencies and can **automatically call/message** hotlines via Twilio-like integrations.  
- 🌐 Uses user location (with explicit consent) to provide region-specific resources and contacts.  
- 🧑‍⚕️ Escalates to professional support workflows when risk is detected — supports human-in-the-loop review.  
- 🔗 Integrates multiple LLM endpoints (e.g., GPT-4o-mini, Claude-style) to gather diverse insights and cross-check responses.  
- 🔒 Emphasizes ethical behavior, privacy, and strict handling of personal health information.

---

## Technical walkthrough ⚙️
- 🧭 Agent orchestration patterns (LangChain / LangGraph style)  
- 🗄️ Local specialist model hosting with Ollama runtimes and MedGemma models  
- 🔌 Tool integration into agentic workflows (APIs, webhooks, action layers)  
- 📲 Emergency communication via Twilio API with configurable escalation rules  
- 🗺️ Location-based services to tailor recommendations and local help links  
- 🖥️ Frontend for lightweight interaction (Streamlit or similar)  
- 🧩 Backend APIs and services implemented with FastAPI  
- 📈 Logging, monitoring, and safety checks for responsible operation

---

## Quick setup 🧰

```bash
# clone the project
git clone https://github.com/dalvi2312/Sanctuary_ai.git
cd SanctuaryAI

# create virtual environment
python -m venv .venv
source .venv/bin/activate   # macOS / Linux
.venv\Scripts\activate      # Windows

# install requirements
pip install -r requirements.txt

# run backend (example)
uvicorn backend.main:app --reload

# run frontend (example)
streamlit run frontend.py
