# FlousiDrive 🚕🇲🇦

**FlousiDrive** is a premium, mobile-first Single Page Application (SPA) designed specifically for ride-hailing drivers (InDrive, Yango, Careem) in Morocco. It replaces messy spreadsheets and notepad calculations with a sleek, native-feeling dashboard that tracks gross income, daily expenses, and true net profit in Moroccan Dirhams (MAD).

Built with a focus on UI/UX, the app features a deep-dark theme to reduce eye strain during night shifts, glassmorphism UI components, and real-time analytical metrics.

## 🚀 Features

* **True Net Profit Tracking:** Automatically deducts app commissions and daily expenses (fuel, tolls, food) from gross fares to display exact take-home pay.
* **Advanced Analytics:** Calculates intelligent performance metrics on the fly:
  * Earnings per Hour (MAD/hr)
  * Earnings per Kilometer (MAD/km)
  * Estimated Fuel Costs based on vehicle consumption settings.
* **Shift Management:** A built-in shift timer to log exact working hours.
* **Daily Goal System:** Visual progress bars tracking daily earnings against a customizable target (e.g., 300 MAD/day).
* **Premium Mobile UI:** Features a custom bottom-sheet modal system, a floating action button (FAB) dock, and smooth CSS animations mimicking high-end iOS/Android applications.
* **Offline Ready (Local Storage):** All data is saved directly to the browser's `localStorage`. No backend database or internet connection is required to log rides.

## 🛠️ Tech Stack

* **HTML5:** Semantic structure with native date-pickers optimized for mobile OS.
* **Tailwind CSS:** Utility-first styling via CDN, utilizing custom configurations for deep-slate dark modes and glassmorphism (`backdrop-blur`).
* **Vanilla JavaScript (ES6+):** Lightweight, dependency-free state management, DOM manipulation, and local storage handling.
* **Chart.js:** For rendering the responsive 7-day net earnings vs. expenses bar chart.
* **FontAwesome:** Scalable vector icons for the UI.

## 📦 Quick Start

Because FlousiDrive is a purely client-side application, getting it running is instant:

1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/flousidrive.git](https://github.com/yourusername/flousidrive.git)
