
# 🚀 3DOSA MAKE BOT — Automate Your MangoNet Tasks

A fully automated bot to handle **daily check-ins**, **API key generation**, and **node connection** for the [MangoNet](https://mangonet.io/) testnet — with **multi-account support and proxy rotation** built-in.

## 🛠️ Features

| ✅ Feature                    | 📌 Description                                 |
|-----------------------------|-----------------------------------------------|
| Auto Daily Check-In         | Automatically checks in every 24 hours        |
| Auto API Key Generation     | Instantly generates your MangoNet API key     |
| Auto Node Connect           | Automatically connects nodes via script       |
| Multi-Account Support       | Easily manage multiple wallets/accounts       |
| Proxy Rotation              | Supports public & private proxies via `proxy.txt` |
| Smart Proxy Handling        | Detects dead proxies and skips them           |

---

## 📁 Project Structure

## ⚙️ How to Use

### 1. Clone the Repository
```bash
git clone https://github.com/ZonaAirdrop/3DOSA-MAKE-BOT.git
cd 3DOSA-MAKE-BOT
````

### 2. Install Python Dependencies

```bash
pip install -r requirements.txt
```

### 3. Create Your `accounts.json` File

This file contains a list of your MangoNet accounts:

```json
[
  {
    "Email": "your_email_1@example.com",
    "Password": "your_password_1"
  },
  {
    "Email": "your_email_2@example.com",
    "Password": "your_password_2"
  }
]
```

### 4. (Optional) Use Proxies via `proxy.txt`

Create a file named `proxy.txt` in the same folder. The bot will automatically rotate and validate proxies.

**Supported formats:**

```
ip:port  
http://ip:port  
http://username:password@ip:port
```

**Example:**

```
188.166.10.55:8080
http://103.14.36.194:3128
http://user123:pass456@45.77.53.25:8000
```

🧠 Each proxy must be on a new line. Invalid proxies will be skipped.

---

### 5. Run the Bot

```bash
python bot.py
```

---

## 💡 Tips & Recommendations

* ✅ Use Python **3.9+**
* 🧵 You can run multiple accounts at once — the bot uses threading
* 🛡️ For better performance, use **reliable proxies** if you're using many accounts
* 📡 Run with `screen` or `tmux` to keep the bot running on a VPS

---

## 🤝 Contribute & Contact

Have a suggestion, bug report, or idea?

* Fork the repo & submit a Pull Request
* Or chat with us on [Zona Airdrop Telegram](https://t.me/ZonaAirdrop)

