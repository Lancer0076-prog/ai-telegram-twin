# 🤖 AI Telegram Twin & Sales Assistant

Архитектура автономного UserBot-ассистента в Telegram (**Telethon / MTProto**), который воспроизводит стиль общения владельца отдельно от базы знаний и прайса.

## Ключевые модули
- **Style Mimic Core:** анализ истории диалогов (длина фраз, дробление мыслей, пунктуация) изолированно от фактов.
- **Hybrid LLM Adapter (Local + Cloud Fallback):** приоритетный инференс на локальной **RTX 3090** (LM Studio / Ollama) с мгновенным переключением на облачные API (Gemini / DeepSeek) при отключениях электричества.
- **Anti-Detection & Human-in-the-Loop:** `Smart Typing` (реалистичная задержка набора), `Smart Pause` (автопауза, если владелец сам зашёл в чат), `Lead Radar` и уведомления менеджеру при готовности к оплате.

📄 Полная спецификация: [ROADMAP_AND_SPECS.md](./ROADMAP_AND_SPECS.md)  
🌐 Сайт проекта: [LancerLab](http://lancer0076.keenetic.pro:8081/projects/#telegram-twin)
