# 🌤️ SkyCast — Weather App with Interactive Map

A lightweight, browser-based weather app that lets you click anywhere on an interactive map and instantly see real-time weather data for that location. No search bars, no typing — just click and know.

**[🔗 Live Demo](https://7ds-adarsh.github.io/Weather-app/)**

---

## ✨ Features

- **Interactive Map** — Powered by Leaflet.js + OpenStreetMap; load it on demand with a single button click
- **Click-to-Weather** — Click anywhere on the map to fetch weather for the nearest city via reverse geocoding
- **Real-Time Data** — Pulls live weather from the OpenWeatherMap API
- **Weather Details** — Displays temperature, weather condition, humidity, wind speed, pressure, and sunrise/sunset times
- **Zero Dependencies to Install** — Pure HTML, CSS, and JavaScript; no build tools, no npm

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML / CSS / JS | Core structure, styling, and logic |
| [Leaflet.js](https://leafletjs.com/) | Interactive map rendering |
| [OpenStreetMap](https://www.openstreetmap.org/) | Map tile layer |
| [Nominatim API](https://nominatim.org/) | Reverse geocoding (coordinates → city name) |
| [OpenWeatherMap API](https://openweathermap.org/api) | Live weather data |

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/7ds-adarsh/Weather-app.git
cd Weather-app
```

### 2. Add your API key

Open `index.html` and replace the placeholder with your own [OpenWeatherMap API key](https://home.openweathermap.org/api_keys):

```js
const API_KEY = "your_api_key_here";
```

> A free-tier OpenWeatherMap account is enough to run this app.

### 3. Run it

Simply open `index.html` in any browser — no server required.

---

## 📖 How It Works

1. Click **"Show Map"** to initialize the Leaflet map centered on New Delhi.
2. Click any location on the map.
3. The app reverse-geocodes the coordinates using Nominatim to find the nearest city name.
4. It then calls the OpenWeatherMap API with that city name.
5. Weather data is displayed below the map in real time.

---

## 📁 Project Structure

```
Weather-app/
└── index.html   # All HTML, CSS, and JavaScript in a single file
```

---

## ⚠️ Notes

- The OpenWeatherMap API key in the source is publicly visible — for production use, consider proxying requests through a backend.
- Reverse geocoding depends on Nominatim, which may not resolve every map click to a named city (e.g., oceans, remote areas).

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
