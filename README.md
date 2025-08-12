# Weather App

This project is a simple and user-friendly command-line Weather App built with python using the PyQt5 tool.
It fetches real-time weather data using the OpenWeatherApp API and displays current weather descriptions for any city inputed by the user.

---

## 📜 Table of Contents
-[Features]
-[Demo]
-[Tech Stack]
-[Installation]
-[Usage]
-[Code Snippet]
-[Future Improvements]
-[Contribution]
-[License]
-[Author]


---

## #️⃣ Features

Get real-time weather data for any city worrldwide
Displays temperature and weather descriptions
Weather icons for visual context
Modular and clean codebases
Error handling for invalid cities, Invalid API calls, and Network Issues.

---

## 📈 Demo

Enter city name: Vilnius
Temperature: 22°C
weatherdescription: ☁️ broken clouds

##🔌 Techn Stack

-Python 3.11
-PyQt5 for GUI
-requests - to fetch data from OpenWeatherMap API
-OpenWeatherMap API - weather data provider

---

## 🚀 Installation

🔧 Prerequisites
- Python 3.x installed on your system
- pip(Python npackage manager)
- pip install PyQt5 requests
- Get OpenWeatherMap APIKey
    - Go to https://openweathermap.org/api
    - sign up and generate your free API key
    - save the API key to use in the application

## 👩‍💻 Usage [How it Works]

1. User enters a city name
2. App sends an HTTP request to the OpenWeatherMap API
3. JSON response is parsed for weather data
4. GUI displays:
     - Temperature
     - Weather description
     - Weather Icon
5. Handles Errors (e.g., invalid city, connection error or API errors)

## 👩‍💻 Code Snippet

import sys
import requests
from PyQt5.QtWidgets import (QApplication, QWidget, QLabel,
                             QLineEdit, QPushButton, QVBoxLayout)
from PyQt5.QtCore import Qt
 def get_weather(self):

        api_key = "your_api_key_here"
        city = self.city_input.text()
        url = f"https://api.openweathermap.org/data/2.5/weather?q={city}&appid={api_key}"
        response = requests.get(url)
        response.raise_for_status()
        return response.json()

## 🛠️ Future Improvements

- 5-day forecast feature'
- custom themes or dark mode
- multi-language support

## Contribution

Pull requests are welcome! 

## 📜 License

This project is licensed under MIT

## 👩‍💻 Author
Shammah Akosile
Email: olawunmi.lola15@gmail.com

