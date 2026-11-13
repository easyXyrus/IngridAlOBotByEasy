<div align="center">

# Stardevs AIO

### One bot. A complete Discord server toolkit.

A feature-rich, all-in-one Discord bot built with **Python** and **discord.py** — bringing moderation, server security, community utilities, automation, and interactive management into one place.

<br>

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![discord.py](https://img.shields.io/badge/discord.py-2.6%2B-5865F2?style=for-the-badge&logo=discord)
![Database](https://img.shields.io/badge/Database-SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![License](https://img.shields.io/badge/License-FXD--NC-lightgrey?style=for-the-badge)

<br>

**Built for communities that want more control, less clutter, and a smoother server experience.**

</div>

---

## ✦ What’s Inside

Stardevs AIO combines essential server tools in a single bot, with interactive Discord interfaces and configurable server settings.

<table>
<tr>
<td width="50%" valign="top">

### 🛡️ Security & Moderation
- Antinuke protection modules
- Server and user moderation tools
- AutoMod with allowlist / blocklist support
- Whitelist and extra-owner controls
- Message purge utilities
- Moderation and event logging

</td>
<td width="50%" valign="top">

### 🎫 Community & Engagement
- Interactive ticket system
- Giveaways
- Welcome and greeting messages
- Reaction roles
- Automatic role assignment
- Message and invite tracking
- AutoResponder and AutoReact

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ⚙️ Server Management
- Server, user, role, and channel information
- Embed builder
- Role and channel utilities
- Per-server command prefix
- Ignored-channel controls
- Command and category help menus

</td>
<td width="50%" valign="top">

### ✨ Bot Features
- NoPrefix system
- Premium-system module
- SQLite-backed storage
- Webhook event notifications
- Rotating bot status
- Prefix and slash-command support where implemented
- Discord Components V2 interfaces

</td>
</tr>
</table>

---

## 🚀 Getting Started

### 1. Requirements

- Python **3.10 or newer**
- A Discord application and bot account
- Bot token and application/client ID
- Required Python packages from `requirements.txt`

### 2. Download the project

```bash
git clone <YOUR_REPOSITORY_URL>
cd <YOUR_PROJECT_FOLDER>
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Configure environment variables

Create a file named `.env` in the project root. Add your own values:

```env
DISCORD_TOKEN=your_bot_token
CLIENT_ID=your_application_id
OWNER_IDS=your_discord_user_id
BOT_PREFIX=&

SUPPORT_SERVER=https://discord.gg/your-server
WEBSITE=https://your-website.example
STATUS_PAGE=https://your-status-page.example

# Optional channel IDs
NOPREFIX_LOG_CHANNEL_ID=
NOPREFIX_CLAIM_CHANNEL_ID=

# Optional webhook URLs
WEBHOOK_COMMANDS=
WEBHOOK_GUILD_JOIN=
WEBHOOK_GUILD_LEAVE=
WEBHOOK_ERRORS=
WEBHOOK_READY=
```

**Keep your `.env` private.** Never upload your bot token, webhook URLs, or other secrets to GitHub. Add `.env` to `.gitignore`.

### 5. Enable Discord intents

Open the [Discord Developer Portal](https://discord.com/developers/applications), select your application, and review the **Bot → Privileged Gateway Intents** settings.

The current bot configuration requests `discord.Intents.all()`. Enable the privileged intents required by your bot and make sure your application is authorized to use them.

### 6. Start Ingrid

```bash
python main.py
```

On first startup, the project attempts to upload its application emojis automatically. If that process is unavailable, the bot catches the failure and continues with fallback emoji IDs.

---

## 🧩 Project Layout

```text
.
├── Ingrid/
│   └── emojis.py
├── cogs/
│   ├── antinuke_core.py
│   ├── antinuke_modules.py
│   ├── automod.py
│   ├── moderation.py
│   ├── ticket.py
│   ├── giveaway.py
│   ├── welcome.py
│   ├── logging.py
│   ├── reactionrole.py
│   ├── autorole.py
│   ├── autoresponder.py
│   ├── autoreact.py
│   ├── tracker.py
│   ├── premium.py
│   ├── noprefix.py
│   └── ...
├── data/
├── scripts/
├── utils/
├── main.py
├── requirements.txt
├── LICENSE
└── README.md
```

The bot loads its extensions from `cogs/`, shared helpers and configuration from `utils/`, emoji resources from `Stardevs/`, and supporting scripts from `scripts/`.

---

## 🔧 Configuration Notes

| Variable | Purpose |
|---|---|
| `DISCORD_TOKEN` | Bot authentication token |
| `CLIENT_ID` | Discord application ID |
| `OWNER_IDS` | Owner user IDs; multiple IDs can be comma-separated |
| `BOT_PREFIX` | Default prefix; defaults to `&` |
| `SUPPORT_SERVER` | Support-server invite |
| `WEBSITE` | Project website; falls back to support server |
| `STATUS_PAGE` | Status page; falls back to support server |
| `INVITE_URL` | Optional custom bot invite URL |
| `NOPREFIX_LOG_CHANNEL_ID` | Optional NoPrefix log channel |
| `NOPREFIX_CLAIM_CHANNEL_ID` | Optional NoPrefix claim channel |
| `WEBHOOK_*` | Optional event and error webhook endpoints |

Use numeric Discord IDs where an ID is requested. Do not put quotation marks around `.env` values unless they are genuinely part of the value.

---

## 📌 Important

- Keep the supplied `LICENSE` file and original credits when sharing or modifying this project.
- Do not publish bot tokens, webhook URLs, or private server configuration.
- Review permissions before inviting the bot to a server. Grant only the permissions your deployment requires.
- Back up the project’s persistent data before making upgrades or replacing files.
- This repository is provided under the license included with the source. Read `LICENSE` before using, modifying, or redistributing it.

---

## Credits

<div align="center">

**Stardevs**  
Credits: **Easy**

[Discord Support](https://discord.gg/stardevs)

<br>

<sub>© 2026 Easy</sub>

</div>
