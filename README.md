# 🚀 Sales Agent Fleet

> 6 specialized AI agents to help your sales team close more deals — hosted on GitHub Pages, no coding required to use.

---

## What's Inside

| Agent | Purpose |
|---|---|
| 🛡️ **Objection Crusher** | Handles any pushback on price, timing, or competitors |
| ⚡ **Follow-Up Forge** | Writes cold-reviving follow-up emails that actually get replies |
| 🔍 **Discovery Driller** | Generates SPIN-style questions to uncover pain and urgency |
| 🎯 **Deal Strategist** | Diagnoses a stuck deal and tells you your next 3 moves |
| ⚔️ **Battlecard Bot** | Instant competitive positioning against any rival |
| 🧠 **Call Coach** | Real-time script and talk track for awkward call moments |

## 🔑 How To Use It

Each team member needs their own Anthropic API key.

### Getting an API Key
1. Go to [console.anthropic.com](https://console.anthropic.com)
2. Sign up / log in
3. Click **API Keys** → **Create Key**
4. Copy it (starts with `sk-ant-...`)
5. Add a small amount of credit (e.g. $10 — this lasts a long time at ~$0.01–0.03 per query)

### Logging In
1. Visit your GitHub Pages URL (https://brioengineer.github.io/sales-agent-fleet/)
2. Paste your API key into the unlock screen
3. Click **Unlock Agents**
4. The key is saved for your browser session only — it disappears when you close the tab

---

## 💰 Cost Estimate

| Usage | Approx. Cost |
|---|---|
| 1 agent query | ~$0.01–0.03 |
| 50 queries/month per rep | ~$0.50–$1.50 |
| 5-person team, heavy use | ~$5–15/month |

Each person pays for their own usage via their own API key — or you can fund one shared account.

---

## 🔒 Security Notes

- **API keys are never stored on any server.** They live only in your browser's session memory and are gone when you close the tab.
- The app makes calls **directly from your browser** to Anthropic's API.
- Because the repo is public, the source code is visible — but there are **no secrets in the code**. Keys are entered at runtime.
- For extra security, keep the URL within your team (don't post it publicly).

---

## 🛠️ Customizing the Agents

Want to change what an agent does or add your own? Open `index.html` and find the `AGENTS` array near the top. Each agent has:

```js
{
  name: "Agent Name",
  systemPrompt: `The instructions that define what this agent does...`,
  placeholder: "The hint text shown in the input box",
}
```

Edit the `systemPrompt` to change behavior, or copy-paste an agent block to add a new one.

---

## ❓ Troubleshooting

| Problem | Fix |
|---|---|
| "API key rejected" | Double-check you copied the full key from console.anthropic.com |
| Page not loading | Wait 2–3 minutes after enabling GitHub Pages, then hard refresh |
| Blank page | Make sure the file is named exactly `index.html` (lowercase) |
| "Connection error" | Check your internet; Anthropic's API may be briefly down |

---

*Built with some help from Claude. Powered by the Anthropic API.*
