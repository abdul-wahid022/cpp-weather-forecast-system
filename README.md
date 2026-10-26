<p align="center">
  <img src="./images/banner.png" alt="Sky Cast" width="800"/>
</p>

<h1 align="center">Sky Cast</h1>

<h3 align="center">Console weather forecast system in C++ for Pakistani cities</h3>

<p align="center">
  <img src="https://img.shields.io/badge/LANGUAGE-C%2B%2B-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" alt="Language"/>
  <img src="https://img.shields.io/badge/PARADIGM-OOP-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" alt="Paradigm"/>
  <img src="https://img.shields.io/badge/API-OPENWEATHERMAP-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" alt="API"/>
  <img src="https://img.shields.io/badge/STATUS-COMPLETE-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" alt="Status"/>
</p>

<p align="center">
  <a href="#overview"><b>Overview</b></a> ·
  <a href="#features"><b>Features</b></a> ·
  <a href="#screenshots"><b>Screenshots</b></a> ·
  <a href="#tech-stack"><b>Tech Stack</b></a> ·
  <a href="#build--run"><b>Build</b></a> ·
  <a href="#repository-structure"><b>Structure</b></a>
</p>

---

## Overview

Sky Cast is a console weather application written in C++. It fetches live data from the OpenWeatherMap API for Pakistani cities and lets the user check current weather, view a 5-day forecast, search cities by weather condition or temperature, and read weather history, safety alerts and educational content. It applies object-oriented programming, external API integration, JSON parsing and file handling in one program.

| | |
| --- | --- |
| **Language** | C++ |
| **Interface** | Console menu with 8 options |
| **Data source** | OpenWeatherMap API |
| **Libraries** | libcurl (HTTP requests), RapidJSON (JSON parsing) |
| **Storage** | Weather history saved to files (`fstream`) |
| **Coverage** | Major Pakistani cities |

## Features

| Menu | Feature | Description |
| ---- | ------- | ----------- |
| 1 | Weather by city | Current temperature, humidity and conditions for a city |
| 2 | Search by condition | List cities with a given condition such as clear, rain or clouds |
| 3 | Search by temperature | List cities within 1°C of a target temperature |
| 4 | 5-day forecast | Forecast for the next five days |
| 5 | Weather history | View past records stored in files |
| 6 | Alerts and precautions | Weather alerts and emergency preparation guidelines |
| 7 | Learn about weather | Weather types, terminology and facts |
| 8 | Exit | Close the program |

## Screenshots

Captured on Ubuntu while the program was running.

| | |
| --- | --- |
| <img src="./images/weather-multan.png" alt="Weather by city, Multan" width="420"/> | <img src="./images/weather-lahore.png" alt="Weather by city, Lahore" width="420"/> |
| <sub>Option 1: weather by city (Multan)</sub> | <sub>Option 1: weather by city (Lahore)</sub> |
| <img src="./images/search-by-condition.png" alt="Search by weather condition" width="420"/> | <img src="./images/search-by-temperature.png" alt="Search by temperature" width="420"/> |
| <sub>Option 2: search by weather condition</sub> | <sub>Option 3: search by temperature</sub> |

## Tech Stack

| Component | Technology |
| --------- | ---------- |
| Programming | C++ |
| API | OpenWeatherMap |
| HTTP requests | libcurl |
| JSON parsing | RapidJSON |
| File handling | C++ `fstream` |

## Build & Run

A free [OpenWeatherMap API key](https://openweathermap.org/api) is required.

Install the dependencies on Debian, Ubuntu or Kali:

```bash
sudo apt update
sudo apt install g++ libcurl4-openssl-dev pkg-config rapidjson-dev git
```

Clone this repository and RapidJSON, then compile and run:

```bash
git clone https://github.com/abdul-wahid022/cpp-weather-forecast-system.git
cd cpp-weather-forecast-system/"Sky Cast"
git clone https://github.com/Tencent/rapidjson.git
g++ Q1.cpp -o SkyCast -I./rapidjson/include $(pkg-config --cflags --libs libcurl)
./SkyCast
```

## Repository Structure

```
cpp-weather-forecast-system/
├── README.md
├── Sky Cast/                 # source code
│   └── Q1.cpp
├── screenshots/              # program screenshots
└── images/                   # banner
```

## License

Shared for educational reference.

## Contact

<p align="center">
  <b>Abdul Wahid</b>
</p>

<p align="center">
  <a href="mailto:a.wahid7860668@gmail.com"><img src="https://img.shields.io/badge/EMAIL-0d1117?style=for-the-badge&logo=gmail&logoColor=white&color=00b4d8" alt="Email"/></a>
  <a href="https://www.linkedin.com/in/abdul-wahid022"><img src="https://img.shields.io/badge/LINKEDIN-0d1117?style=for-the-badge&logo=linkedin&logoColor=white&color=00b4d8" alt="LinkedIn"/></a>
  <a href="https://github.com/abdul-wahid022"><img src="https://img.shields.io/badge/GITHUB-0d1117?style=for-the-badge&logo=github&logoColor=white&color=00b4d8" alt="GitHub"/></a>
</p>
