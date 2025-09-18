# 🌍 Awesome Open Data APIs

A **community-driven collection of free & open APIs** with examples.  
Perfect for developers, students, and hobbyists looking to build projects.  

👉 Goal: Make it easy for anyone to discover useful APIs and learn how to use them.  

---

## 📂 Categories

### 📈 Finance
- [Polygon.io](https://polygon.io) – Free stock & crypto data API (✅ Free tier, 🔑 Requires API Key)  
- [Frankfurter](https://www.frankfurter.app/) – Currency exchange rates, no auth required (✅ Free, 🚫 No Auth)

### 🌦️ Weather
- [Open-Meteo](https://open-meteo.com/) – Global weather forecasts (✅ Free, 🚫 No Auth)  
- [WeatherAPI](https://www.weatherapi.com/) – Weather and astronomy data (✅ Free tier, 🔑 API Key)

### 🛰️ Space
- [NASA Open APIs](https://api.nasa.gov/) – Space imagery, Mars Rover, and more (✅ Free, 🔑 API Key)  
- [Open Notify](http://open-notify.org/) – ISS location and astronaut data (✅ Free, 🚫 No Auth)

---

## 📖 Examples

We include code samples in `/examples` to help you get started quickly.  

Example in Python:
```python
import requests

response = requests.get("https://api.open-meteo.com/v1/forecast?latitude=35&longitude=139&hourly=temperature_2m")
data = response.json()
print(data["hourly"]["temperature_2m"][:5])
