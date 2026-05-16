<div align="center">

# 🚗💚 FlousiDrive

### The ride-hailing income tracker built for Moroccan drivers

**Log rides. Track expenses. Maximize profit.**  
A beautiful, offline-first PWA designed from the ground up for drivers on InDrive, Bolt, Careem, Heetch, and Yango.

[![Live App](https://img.shields.io/badge/🌐_Live_App-flousidrive.netlify.app-10B981?style=for-the-badge)](https://flousidrive.netlify.app)
![Platform](https://img.shields.io/badge/Platform-iOS_%7C_Android_%7C_Web-3B82F6?style=for-the-badge)
![Language](https://img.shields.io/badge/Languages-4-F59E0B?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-8B5CF6?style=for-the-badge)

</div>

---

## ✨ What is FlousiDrive?

FlousiDrive is a **mobile-first progressive web app** for ride-hailing drivers in Morocco. No accounts, no subscriptions, no cloud — everything lives on your phone, offline, always fast.

Whether you're on a night shift in Casablanca or doing Iftar-rush rides in Marrakech, FlousiDrive gives you a real-time picture of your earnings, expenses, and profit — in your language, in MAD.

---

## 📱 Screenshots

> *Dark mode · Mobile optimized · Works on all phones*

| Dashboard | Log Ride | Stats | Config |
|:---------:|:--------:|:-----:|:------:|
| Today's net profit, goal bar, live data | Quick ride logging with auto-commission | Peak hours chart, platform breakdown | City, vehicle, platform, language |

---

## 🚀 Features

### 💰 Earnings Tracker
- Log rides with **gross fare, commission, tip, distance, and duration**
- Auto-calculates commission from your default rate as you type
- Real-time **net preview** before saving
- Tracks **Cash vs Digital** payment separately
- Per-platform logging: InDrive, Bolt, Careem, Heetch, Yango, Independent

### 📊 Smart Dashboard
- **Today's net profit** at a glance with motivational messages
- Daily goal progress bar with rides-remaining estimate
- **MAD/hour** and **MAD/km** efficiency metrics
- Estimated fuel cost for the day
- 7-day earnings chart (net vs expenses)

### ⚡ Live Data (AI-Powered)
- 🌤️ **Real-time weather** for your city
- 💱 **USD/MAD exchange rate** (live)
- ⛽ **Fuel prices** fetched via AI web search (Gasoil S50 + Essence SP95)
- 🤖 **AI driving tip** tailored to your city and language

### 📈 Performance Stats
- All-time totals: rides, earned, kilometers, best day
- **Peak hours chart** — see exactly which hours make you the most money
- **Platform breakdown** — compare InDrive vs Bolt vs Careem performance
- **Expense breakdown** by category with percentage bars

### 🧾 Expense Logging
- 10 categories: Fuel, Wash, Maintenance, Tolls, Food, Mobile, Insurance, Vignette, Visite Technique, Other
- Full activity ledger with filter by rides / expenses / all
- Swipe-friendly cards with one-tap delete

### ⛽ Quick Fuel Log
- Log a fillup in seconds: type, liters, price/liter
- Auto-calculates total cost
- Saved as an expense automatically

### 🎯 Goal Calculator
- Set daily and weekly income targets
- Tells you exactly how many more rides you need to hit your goal
- Updates live as you log rides

### 🌙 Ramadan Mode
- Shows Iftar (20h–24h) and Suhoor (3h–5h) as peak hour reminders
- Toggle on/off anytime

### ⏱️ Shift Timer
- Start/stop your shift with one tap
- Live elapsed time displayed in the header

---

## 🌍 Multi-Language Support

FlousiDrive speaks your language:

| Language | Code | Direction |
|----------|------|-----------|
| 🇬🇧 English | `en` | LTR |
| 🇫🇷 Français | `fr` | LTR |
| 🇸🇦 العربية الفصحى | `ar` | RTL |
| 🇲🇦 الدارجة المغربية | `ma` | RTL |

Full RTL layout support — the entire UI flips for Arabic/Darija.

---

## 🏙️ Supported Cities

> Casa · Rabat · Marrakech · Fès · Tanger · Agadir · Meknès · Oujda · Tétouan · Kenitra · Safi · El Jadida · Béni Mellal · Nador

City selection affects weather data and AI fuel tip context.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| 🎨 UI Framework | Tailwind CSS (CDN) |
| 📊 Charts | Chart.js |
| 🤖 AI / Live Data | Anthropic Claude API (claude-sonnet) |
| 🌤️ Weather | Open-Meteo API (free, no key needed) |
| 💱 Exchange Rate | Open Exchange Rates / ExchangeRate-API |
| 💾 Storage | `localStorage` (offline, no backend) |
| 🔤 Fonts | Inter + Tajawal (Google Fonts) |
| 🎯 Icons | Font Awesome 6 |
| 🚀 Hosting | Netlify |

---

## 📲 Mobile Optimization

FlousiDrive is engineered for phones — not just "responsive":

- ✅ **iOS Safari `-webkit-text-fill-color` fix** — buttons always show text
- ✅ **44px minimum touch targets** (Apple HIG standard)
- ✅ **16px input font-size** — prevents Safari auto-zoom on focus
- ✅ **`env(safe-area-inset-bottom)`** — nav never hides behind iPhone home bar
- ✅ **Swipe-down to close** bottom sheets
- ✅ **Body scroll lock** when sheets are open
- ✅ **Apple PWA meta tags** — add to home screen support
- ✅ **`-webkit-overflow-scrolling: touch`** — smooth scroll everywhere
- ✅ **No number input spinners** — cleaner mobile UI

---

## ⚙️ Getting Started

FlousiDrive is a single HTML file — zero build step, zero dependencies to install.

### Option 1 — Use it live
👉 [flousidrive.netlify.app](https://flousidrive.netlify.app)

### Option 2 — Run locally
```bash
git clone https://github.com/YOUR_USERNAME/flousidrive.git
cd flousidrive
# Open the file directly in your browser
open FlousiDrive_mobile_optimized.html
```

### Option 3 — Add to iPhone home screen
1. Open [flousidrive.netlify.app](https://flousidrive.netlify.app) in Safari
2. Tap the **Share** button
3. Tap **Add to Home Screen**
4. Done — it works like a native app 📱

---

## 🗂️ Project Structure

```
flousidrive/
│
├── FlousiDrive_mobile_optimized.html   # The entire app (single file)
└── README.md                           # This file
```

Everything — HTML, CSS, JavaScript, translations, chart logic, API calls — lives in one portable file. Open it anywhere, share it anywhere.

---

## 🔒 Privacy

- **Zero data leaves your device.** All rides and expenses are stored in your browser's `localStorage`.
- No user accounts, no sign-up, no tracking.
- The only external calls are: weather API, exchange rate API, and Anthropic API for live fuel prices — none of these receive any personal data.

---

## 🗺️ Roadmap

- [ ] 📤 Export to PDF (weekly/monthly report)
- [ ] 🔔 Push notifications for shift reminders
- [ ] 📅 Monthly goal tracking
- [ ] 🗺️ Route distance auto-calculation
- [ ] 👥 Multi-driver / family mode
- [ ] ☁️ Optional cloud backup (encrypted)

---

## 🤝 Contributing

Contributions are welcome! If you're a Moroccan driver and something doesn't work the way you expect, open an issue — you're the target user and your feedback matters most.

```bash
# Fork the repo, make your changes, then open a PR
git checkout -b fix/your-fix-name
git commit -m "fix: description of what you changed"
git push origin fix/your-fix-name
```

---

## 📄 License

MIT — free to use, modify, and distribute.

---

<div align="center">

Made with 💚 for Moroccan drivers

**FlousiDrive** · [flousidrive.netlify.app](https://flousidrive.netlify.app)

*"Log it. Track it. Own your shift."*

</div>
