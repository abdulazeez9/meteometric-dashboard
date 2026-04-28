# Metrometric Dashboard 🌤️

> A modern, responsive weather monitoring Progressive Web App built with React, TypeScript, and Chakra UI.

Track real-time weather conditions, air quality, interactive forecasts, and multiple locations — all from a clean, installable dashboard.

---

## ✨ Features

- **Real-Time Weather Data** — Current conditions including temperature, humidity, wind speed, and more
- **Weather Forecast** — Multi-day forecast with interactive charts powered by Recharts
- **Air Quality Monitoring** — Track air quality index (AQI) and pollutant breakdown
- **Multi-Location Tracking** — Save and switch between multiple cities
- **Interactive Map** — Leaflet-powered map for visualizing weather by location
- **Dark Mode Support** — Full light/dark theme via Chakra UI color mode
- **PWA Ready** — Installable on desktop and mobile as a Progressive Web App
- **Responsive Design** — Optimized for all screen sizes

---

## 🛠 Tech Stack

| Technology | Purpose |
|---|---|
| React 18 + TypeScript | UI framework and type safety |
| Vite | Build tool and dev server |
| Chakra UI v2 | Component library and theming |
| Recharts | Interactive weather charts and graphs |
| React Leaflet + Leaflet | Interactive weather map |
| React Router DOM v7 | Client-side routing |
| Framer Motion | Animations and transitions |
| React Icons + Lucide React | Icon sets |
| `vite-plugin-pwa` | Progressive Web App support |

---

## 🚀 Getting Started

### Prerequisites

- Node.js `>=18`
- npm or yarn
- A weather API key (e.g. [OpenWeatherMap](https://openweathermap.org/api) or [Open-Meteo](https://open-meteo.com/))

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/metrometric-dashboard.git
cd metrometric-dashboard

# Install dependencies
npm install
```

### Environment Variables

Create a `.env` file in the root of the project:

```env
VITE_WEATHER_API_KEY=your_api_key_here
VITE_WEATHER_API_BASE_URL=https://api.openweathermap.org/data/2.5
```

> **Note:** Never commit your `.env` file. It is already listed in `.gitignore`.

### Running Locally

```bash
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Building for Production

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

---

## 📁 Project Structure

```
metrometric-dashboard/
├── src/
│   ├── components/
│   │   ├── WeatherCard.tsx         # Current conditions display
│   │   ├── ForecastChart.tsx       # Recharts forecast graph
│   │   ├── AirQualityPanel.tsx     # AQI and pollutant details
│   │   ├── WeatherMap.tsx          # Leaflet map integration
│   │   ├── LocationSearch.tsx      # City search and saved locations
│   │   ├── Header.tsx
│   │   └── Footer.tsx
│   ├── pages/
│   │   ├── Dashboard.tsx           # Main weather dashboard
│   │   └── LocationDetail.tsx      # Per-city detail view
│   ├── hooks/
│   │   └── useWeather.ts           # Weather data fetching hook
│   ├── types/
│   │   └── index.ts                # Shared TypeScript types
│   ├── utils/
│   │   └── weatherHelpers.ts       # Unit conversions, formatters
│   └── main.tsx
├── public/
│   └── icons/                      # PWA icons
├── .env.example
├── package.json
└── vite.config.ts
```

---

## 🌍 Key Sections

| Section | Description |
|---|---|
| Current Weather | Temperature, feels like, humidity, wind, UV index |
| Hourly Forecast | Hour-by-hour chart for the next 24 hours |
| 7-Day Forecast | Daily high/low with condition icons |
| Air Quality | AQI score with PM2.5, PM10, CO, NO₂ readings |
| Weather Map | Interactive map with weather layer overlays |
| Saved Locations | Quickly switch between tracked cities |

---

## 📱 PWA Support

Metrometric is installable as a Progressive Web App on both desktop and mobile:

- Works offline with cached weather data
- Add to Home Screen on iOS and Android
- App-like experience without a browser toolbar

---

## 📜 Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start local dev server |
| `npm run build` | Type-check and build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint |

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

1. Fork the repo
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m 'Add my feature'`
4. Push to the branch: `git push origin feature/my-feature`
5. Open a pull request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<p align="center">Built with ❤️ using React + Chakra UI + Recharts</p>
