# 🌍 Global Earthquake Monitoring Dashboard

An interactive earthquake map built using HTML, JavaScript, and Leaflet, designed to integrate seamlessly with Microsoft Power BI.

---

## 📌 Overview

This project visualizes earthquake data on a world map. It dynamically updates based on input parameters such as latitude, longitude, and magnitude — making it ideal for embedding inside Power BI dashboards.

---

## 🚀 Features

* 🌍 Interactive world map
* 📍 Dynamic earthquake marker based on input
* 🎨 Color-coded magnitude visualization
* 📊 Clean dashboard-style UI
* 📦 Lightweight and fast (no backend required)
* 🔗 Works with Power BI via URL parameters

---

## 🛠️ Technologies Used

* HTML5
* CSS3
* JavaScript
* Leaflet.js (for maps)

---

## 📥 How It Works

The map reads parameters from the URL:

```
?lat=VALUE&lon=VALUE&mag=VALUE&place=NAME
```

### Example:

```
https://yourusername.github.io/earthquake-map/?lat=34&lon=-118&mag=5.6&place=California
```

---

## 📊 Power BI Integration

1. Upload the HTML file to GitHub
2. Enable GitHub Pages
3. Use the generated URL in Power BI

### DAX Example:

```DAX
Map URL =
VAR lat = SELECTEDVALUE(Earthquake[Latitude])
VAR lon = SELECTEDVALUE(Earthquake[Longitude])
VAR mag = SELECTEDVALUE(Earthquake[Magnitude])
VAR place = SELECTEDVALUE(Earthquake[Location])

RETURN
"https://yourusername.github.io/earthquake-map/?lat="
& lat & "&lon=" & lon & "&mag=" & mag & "&place=" & place
```

4. Use **HTML Content visual** in Power BI to display the map

---

## 🎨 Legend

* 🔴 > 7 → Very High
* 🟠 6 – 7 → High
* 🟡 5 – 6 → Moderate
* 🔵 < 5 → Low

---

## 📂 Project Structure

```
earthquake-map/
│── earthquake-map.html
│── README.md
```

---

## ⚡ Setup Instructions

1. Download the HTML file
2. Upload it to GitHub
3. Enable GitHub Pages
4. Open the generated URL
5. Integrate with Power BI

---

## 🎯 Use Cases

* Data visualization projects
* Power BI dashboards
* Academic assignments
* Real-time monitoring systems (with API upgrade)

---

## 📌 Future Enhancements

* Multiple earthquake markers
* Live data integration (USGS API)
* Filtering by magnitude
* Time-based animation

---

## 👨‍💻 Author

Your Name

---

## ⭐ If you like this project

Give it a star on GitHub ⭐
