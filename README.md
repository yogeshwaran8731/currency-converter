🚀 NexGen FX: Real-Time Currency Converter
NexGen FX is a high-performance, minimalist currency converter designed for the modern web. Built with a "Glassmorphism" aesthetic, it combines real-time financial data with sleek visual analytics to provide a premium user experience.

✨ Key Features
Real-Time Data Fetching: Utilizes the Frankfurter API to provide live exchange rates directly from the European Central Bank.

Historical Sparkline: Features a dynamic Chart.js integration that visualizes the 10-day price trend for any selected currency pair.

Persistent Memory (Cache): Built-in localStorage integration ensures your last searched amount and currency pairs are saved even after a page refresh.

Glassmorphic UI: A futuristic design utilizing -webkit-backdrop-filter for deep blur effects, vibrant gradients, and floating ambient animations.

Full Responsiveness: Optimized for desktop, tablet, and mobile with a strict focus on WebKit compatibility (iOS/Safari).

Integrated Social CTC: One-tap access to connect with the developer via floating GitHub and LinkedIn buttons.

🛠️ Tech Stack
Frontend: HTML5, CSS3 (Modern Gradients & Flexbox/Grid)

Logic: Vanilla JavaScript (ES6+ Async/Await)

Visuals: Chart.js for real-time trend visualization

Icons: Lucide Icons for high-fidelity vector graphics

API: Frankfurter Open Source API

📸 Interface Preview
The application features a centralized "Frosted Glass" card containing:

Input Field: Live-updating amount input.

Currency Selectors: Dynamic dropdowns populated directly from the API.

Sparkline Chart: A neon-cyan trend line showing market movement.

Result Display: High-visibility converted value with a "Last Synced" timestamp.

🚀 Getting Started
Since this is a client-side application, there is no installation required.

Clone the Repository:

Bash
git clone https://github.com/yogeshwaran8731/currency-converter.git
Open the Project:
Simply double-click index.html or use a "Live Server" extension in VS Code.

🧠 Technical Highlights
💾 Smart Caching
The app automatically remembers your preferences so you don't have to re-enter data every time:

JavaScript
// Example of the cache logic
amountInp.value = localStorage.getItem('v_amt') || "1.00";
fromSel.value = localStorage.getItem('v_from') || "USD";
📉 Real-Time Analytics
The app doesn't just show numbers; it shows trends. By calculating a 10-day lookback period, it renders a custom gradient-filled sparkline:

JavaScript
const start = new Date(Date.now() - 10 * 24 * 60 * 60 * 1000).toISOString().split('T')[0];
// Fetches history and updates the UI instantly
👨‍💻 Developed By
Yogeshwaran V

GitHub: @yogeshwaran8731

LinkedIn: Yogeshwaran V

📜 License
This project is open-source and available under the MIT License.
