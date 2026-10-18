# Ficus Command · TYSON v2.3 FINAL

Ready-to-run multi-agent command dashboard.

## Features
- TYSON master agent (Marathi / Hindi / English + voice)
- 23 specialist agents (AI, Investment, Finance 30/30/30, Health)
- Real-task-only pipeline (no fake blink)
- Cyan HUD dashboard + robot-dog TYSON face
- Settings: rename agents, change theme
- Gemini + OpenAI support

## Windows install

```cmd
cd ficus_tyson
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
copy .env.example .env
```

Edit `.env` → put your real key:
```
LLM_PROVIDER=gemini
LLM_API_KEY=AQ.your-real-key
LLM_MODEL=gemini-3.8-flash
```

```cmd
python run.py
```

Open: http://localhost:8000/

## Files to know
- app/ui/dashboard.html — visual HUD
- app/static/tyson_avatar.png — TYSON face
- app/services/llm.py — Gemini/OpenAI
- app/agents/ — all agents
- prompts/ — agent system prompts

## Voice
Chrome/Edge → mic button or Space → speak → auto send

## Settings
Top-right ⚙ → rename desk agents + theme
