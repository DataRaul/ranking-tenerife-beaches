# 🏖️ Tenerife Beach Rank

👉 **[Access the Website](https://dataraul.github.io/ranking-tenerife-beaches/)**

A real-time weather dashboard that ranks **60 beaches** across Tenerife. The application calculates a live "Beachability Score" out of 10 by analyzing wind, temperature, and cloud cover to help you find the sunniest, calmest spot on the island at any given moment.

## ✨ Features

* **Smart Ranking:** Beaches are automatically sorted from "Best" to "Worst" based on live conditions.
* **Emoji-Driven UI:** Visual cues for quick scanning:
    * 🌡️ **Temperature:** Dynamic icons like 🔥 for heatwaves or ☀️ for perfect warmth.
    * 🌬️ **Wind:** Visual alerts like 🚩 for high winds or 💨 for light breezes.
    * ☁️ **Clouds:** Ranges from ☀️ (Clear) to ☁️ (Overcast).
* **Color-Coded Status:** * 🟢 **Green Top Border:** Perfect conditions (Score 8+).
    * 🟡 **Yellow Top Border:** Moderate/Acceptable (Score 6-7).
    * 🔴 **Red Top Border:** Poor conditions for sunbathing (Score < 6).
* **7 Languages:** Seamlessly switch between 🇬🇧, 🇪🇸, 🇩🇪, 🇫🇷, 🇷🇺, 🇳🇱, and 🇵🇹.
* **Privacy-Friendly:** No cookies, no tracking, and uses the open-source Open-Meteo API.

## 🧮 The Scoring Logic

The total score (max 10) is calculated using a weighted algorithm:

| Factor | Max Points | Optimal Range |
| :--- | :--- | :--- |
| **Temperature** | 4 pts | 22°C to 30°C |
| **Wind Speed** | 3 pts | Under 15 km/h |
| **Cloud Cover** | 3 pts | Under 20% coverage |

## 🚀 Technical Overview

* **Data Source:** [Open-Meteo API](https://open-meteo.com/) (Real-time weather).
* **Frontend:** Single-file HTML5/CSS3/Vanilla JS.
* **Typography:** System-native sans-serif stack for fast loading.
* **License:** [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) (Attribution-NonCommercial).

## 🛠️ Usage

Simply open the live link in any browser. The script will fetch the current coordinates for all 60 locations and update the ranking instantly.

---
*Developed for the Tenerife community and visitors. Stay sun-safe!*
