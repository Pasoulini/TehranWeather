# TehranWeather

A sleek Rainmeter weather widget for Tehran powered by the **Open-Meteo API** — free, no API key required.

![Rainmeter](https://img.shields.io/badge/Rainmeter-Skin-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey)
![Author](https://img.shields.io/badge/Author-Parsa%20Rasouli-orange)

## Features

- Current temperature with "feels like" display
- Weather condition with dynamic icons
- High/Low daily temperatures
- Humidity, wind speed, and precipitation
- Auto-refresh every 4 hours
- Hover effects with smooth transitions
- Clean dark UI with blur effect
- Tooltips with detailed information

## Screenshot

```
┌─────────────────────────────┐
│  Tehran                     │
│  32°C         ☀️ Clear      │
│         Feels like 30°C     │
│─────────────────────────────│
│  H 35°C / L 22°C  Wind 14  │
│  Humidity 13%     Rain 0mm  │
└─────────────────────────────┘
```

## Installation

1. Download or clone this repository
2. Copy the `TehranWeather` folder to your Rainmeter skins directory:
   ```
   %USERPROFILE%\Documents\Rainmeter\Skins\
   ```
3. Right-click the Rainmeter tray icon → **Refresh all**
4. Right-click Rainmeter tray → **Skins** → **TehranWeather** → **TehranWeather.ini**

## Data Source

- **Weather**: [Open-Meteo API](https://open-meteo.com/) (Free, no API key)
- **Location**: Tehran, Iran (35.6892°N, 51.3890°E)

## Weather Icons

The widget includes dynamic weather icons for various conditions:
- ☀️ Clear / Mainly clear
- ⛅ Partly cloudy
- ☁️ Overcast
- 🌫️ Fog / Rime fog
- 🌧️ Rain / Drizzle
- ❄️ Snow
- ⛈️ Thunderstorm

## Requirements

- [Rainmeter](https://www.rainmeter.net/) 4.0+
- Windows 10/11
- Internet connection

## API Reference

This widget uses the Open-Meteo Forecast API:

```
https://api.open-meteo.com/v1/forecast
  ?latitude=35.6892
  &longitude=51.3890
  &current=temperature_2m,relative_humidity_2m,apparent_temperature,
           precipitation,weather_code,wind_speed_10m
  &daily=temperature_2m_max,temperature_2m_min,weather_code
  &timezone=Asia/Tehran
```

**No API key required!** Open-Meteo is free for non-commercial use.

## Configuration

Edit `TehranWeather.ini` to customize:

| Variable | Description | Default |
|----------|-------------|---------|
| `FontMain` | Main font family | Segoe UI |
| `FontBold` | Bold font family | Segoe UI Semibold |
| `UpdateRate` | Data refresh interval (seconds) | 14400 |
| `WeatherUrl` | API endpoint | Open-Meteo Tehran |

To change location, update the `latitude` and `longitude` in `WeatherUrl`.

## License

MIT License - feel free to use and modify.

## Author

Made by **Parsa Rasouli** with [Rainmeter](https://www.rainmeter.net/) and good vibes.
