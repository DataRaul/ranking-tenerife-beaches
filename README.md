# 🏖️ Tenerife Beach Rank

A real-time ranking dashboard for 60 beaches across Tenerife. This application fetches live meteorological data and ranks beaches based on ideal swimming and sunbathing conditions.

## 🚀 Live Demo
**[[visit the website]](https://dataraul.github.io/ranking-tenerife-beaches/)**

---

## 📊 How it Works
The application uses the **Open-Meteo API** to fetch high-accuracy weather data for 60 specific GPS coordinates across the island. 

### **The Ranking Algorithm**
Every beach is assigned a score from **0 to 10** based on four key metrics:
1.  **Temperature:** Optimized for the 22°C – 30°C range.
2.  **Wind Speed:** Penalizes high winds (ideal for El Médano for sports, but low for sunbathing).
3.  **Cloud Cover:** Higher points for clear, blue skies.
4.  **Flag Status:** Integrated logic for safety indicators.

### **Color Coding**
- 🟢 **8-10 Points:** Excellent conditions.
- 🟡 **6-7 Points:** Fair/Average conditions.
- 🔴 **Below 6 Points:** Poor conditions (high wind, cold, or cloudy).

---

## 🕒 Update Schedule
The app simulates the standard Canary Island beach report updates:
* **08:00** - Morning report
* **11:00** - Mid-day peak
* **16:00** - Afternoon report

*Note: Since this is a client-side app, data refreshes instantly whenever a user visits the site.*

---

## 🛠️ Technology Stack
- **Frontend:** HTML5, CSS3 (Flexbox/Grid), Vanilla JavaScript.
- **Data Source:** [Open-Meteo API](https://open-meteo.com/) (No-key required).
- **Hosting:** GitHub Pages.
- **Tracking:** [GoatCounter / Analytics]

---

## 📍 Beaches Included
The dataset covers 60 locations including:
- **South:** Las Vistas, El Duque, Fañabé, Abama.
- **North:** Playa Jardín, El Socorro, Las Teresitas.
- **Hidden Gems:** Benijo, Montaña Roja, Diego Hernández.

---

## 📝 License
Creative Commons Non-Commercial (CC BY-NC 4.0)
