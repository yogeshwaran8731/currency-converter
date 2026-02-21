# 🚀 NexGen FX: Real-Time Currency Converter

**NexGen FX** is a high-performance, minimalist currency converter designed for the modern web. Built with a "Glassmorphism" aesthetic, it combines real-time financial data with sleek visual analytics to provide a premium user experience.

---

## ✨ Key Features

* **Real-Time Data Fetching:** Utilizes the Frankfurter API to provide live exchange rates directly from the European Central Bank.
* **Historical Sparkline:** Features a dynamic **Chart.js** integration that visualizes the 10-day price trend for any selected currency pair.
* **Persistent Memory (Cache):** Built-in `localStorage` integration ensures your last searched amount and currency pairs are saved even after a page refresh.
* **Glassmorphic UI:** A futuristic design utilizing `-webkit-backdrop-filter` for deep blur effects, vibrant gradients, and floating ambient animations.
* **Full Responsiveness:** Optimized for desktop, tablet, and mobile with a strict focus on WebKit compatibility (iOS/Safari).
* **Integrated Social CTC:** One-tap access to connect with the developer via floating GitHub and LinkedIn buttons.

---

## 🛠️ Tech Stack

| Technology | Purpose |
| :--- | :--- |
| **HTML5 / CSS3** | Layout, Glassmorphism & Animations |
| **JavaScript (ES6+)** | Async Data Fetching & App Logic |
| **[Chart.js](https://www.chartjs.org/)** | Real-time Trend Visualization |
| **[Lucide Icons](https://lucide.dev/)** | High-fidelity Vector UI Icons |
| **[Frankfurter API](https://www.frankfurter.app/)** | Open-source Currency Exchange Data |

---

## 📸 Interface Breakdown

The application features a centralized "Frosted Glass" card containing:
1.  **Dynamic Input:** Live-updating amount field.
2.  **Currency Selectors:** Dropdowns populated dynamically via API.
3.  **Sparkline Chart:** A neon-cyan trend line showing market movement.
4.  **Result Display:** High-visibility converted value with a "Live Sync" timestamp.

---

## 🚀 Getting Started

Since this is a client-side application, there is no heavy installation required.

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/yogeshwaran8731/currency-converter.git](https://github.com/yogeshwaran8731/currency-converter.git)
    ```
2.  **Open the Project:**
    Simply open `index.html` in your preferred browser.
3.  **Deployment:**
    This project is ready to be hosted on **GitHub Pages**, **Vercel**, or **Netlify** with zero configuration.

---

## 🧠 Technical Highlights

### 💾 Smart Caching
The app automatically remembers your preferences using a persistent cache layer:
```javascript
// Recalling user data on initialization
amountInp.value = localStorage.getItem('v_amt') || "1.00";
fromSel.value = localStorage.getItem('v_from') || "USD";
```
---
## 📉 Real-Time Analytics
The app doesn't just show numbers; it shows trends. By calculating a 10-day lookback period, it renders a custom gradient-filled sparkline:

```javascript
const start = new Date(Date.now() - 10 * 24 * 60 * 60 * 1000).toISOString().split('T')[0];
// Fetches history and updates the UI instantly on every input change
```
---

## 👨‍💻 Developed By
Yogeshwaran V

---

## 📜 License
This project is open-source and available under the MIT License.

---
