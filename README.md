# 🏖️ Tenerife Beach Rank

👉 **[Access the Website](https://dataraul.github.io/ranking-tenerife-beaches/)**
https://bit.ly/tenerife-beaches-rank

A real-time weather dashboard that ranks **60 beaches** across Tenerife. The application calculates a live "Beachability Score" out of 10 by analyzing wind, temperature, cloud cover, and **wave heights** to help you find the perfect spot on the island.

## ✨ Features

* **Smart Ranking:** Beaches are automatically sorted from "Best" to "Worst" based on live conditions.
* **Emoji-Driven UI:** Visual cues for quick scanning:
    * 🌡️ **Temperature:** Dynamic icons like 🔥 for heatwaves or ☀️ for perfect warmth.
    * 🌬️ **Wind:** Visual alerts like 🚩 for high winds or 💨 for light breezes.
    * ☁️ **Clouds:** Ranges from ☀️ (Clear) to ☁️ (Overcast).
    * 🌊 **Waves:** Real-time wave height with safety flags (🟢 🟡 🔴).
* **Safety Bypass Logic:** High waves (over 2.0m) automatically trigger a **Red** status, regardless of how sunny or warm it is, ensuring user safety.
* **Color-Coded Status:**
    * 🟢 **Green Top Border:** Perfect conditions (Score 8+).
    * 🟡 **Yellow Top Border:** Moderate/Acceptable (Score 6-7).
    * 🔴 **Red Top Border:** Poor conditions or unsafe sea (Score < 6 or High Waves).
* **7 Languages:** Seamlessly switch between 🇬🇧, 🇪🇸, 🇩🇪, 🇫🇷, 🇷🇺, 🇳🇱, and 🇵🇹.
* **Privacy-Friendly:** No cookies, no tracking, and uses the open-source Open-Meteo API.

## 🧮 The Scoring Logic

The total score (max 10) is calculated using a weighted algorithm:

| Factor | Max Points | Optimal Range | Safety Indicator |
| :--- | :--- | :--- | :--- |
| **Temperature** | 4 pts | 22°C to 30°C | — |
| **Wind Speed** | 3 pts | Under 15 km/h | — |
| **Cloud Cover** | 3 pts | Under 20% coverage | — |
| **Wave Height** | **Bypass** | Under 1.2m | 🟢 (Safe) |
| **Wave Height** | **Bypass** | 1.2m - 2.0m | 🟡 (Caution) |
| **Wave Height** | **Bypass** | Over 2.0m | 🔴 (Danger/Red Flag) |

> **Note:** If waves exceed 2.0m, the beach status is forced to **Red** to warn against swimming, overriding the weather score.

## 🚀 Technical Overview

* **Data Sources:** [Open-Meteo Weather API](https://open-meteo.com/) & [Open-Meteo Marine API](https://open-meteo.com/en/docs/marine-weather-api).
* **Frontend:** Single-file HTML5/CSS3/Vanilla JS (No frameworks).
* **Performance:** Uses `Promise.all` to fetch weather and marine data concurrently for 60 locations.
* **License:** [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) (Attribution-NonCommercial).

## 🛠️ Usage

Simply open the live link in any browser. The script will fetch the current coordinates for all 60 locations and update the ranking instantly based on the latest available data.

---
*Developed for the Tenerife community and visitors. Stay sun-safe and respect the flags!*
