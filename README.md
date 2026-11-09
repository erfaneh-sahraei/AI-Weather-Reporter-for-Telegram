# AI Weather Reporter for Telegram using n8n

An automated workflow built in **n8n** that fetches live weather data from **OpenWeatherMap API**, processes and enhances it using an **AI Agent / LLM** with custom prompt guardrails, and sends a beautifully formatted weather report directly to a **Telegram** channel or chat.

---

## 🚀 Features
- **Automated Trigger:** Runs periodically using the `Schedule Trigger`.
- **Live Weather Data:** Integrates with OpenWeatherMap API to fetch accurate temperature and city details.
- **AI-Enhanced Formatting:** Uses a strictly-prompted AI model to generate concise, engaging descriptions with relevant weather emojis.
- **Telegram Integration:** Automatically dispatches the final polished report to Telegram.

---

## 📂 Workflow Architecture
1. **Schedule Trigger:** Initiates the workflow at set intervals.
2. **OpenWeatherMap Node:** Fetches current meteorological data.
3. **AI Agent / LLM Node:** Formats the city name and temperature into a human-readable, emoji-rich forecast based on custom system prompts.
4. **Telegram Node:** Sends the final message to your target chat/channel.

---

## 🛠️ Setup & Configuration
1. Import `weather-telegram-workflow.json` into your n8n instance.
2. Add your **OpenWeatherMap** API credentials.
3. Configure your **OpenAI / Chat Model** credentials.
4. Set up your **Telegram Bot** token and target `chat_id` in the Telegram node.
5. Activate the workflow and enjoy automated weather updates!
