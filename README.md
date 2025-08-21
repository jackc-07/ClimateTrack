ClimateTrack
===========

Problem Statement
------------
When monitoring indoor climate, most consumer smart home devices only provide a single measurement location and store data in closed ecosystems. This makes it difficult to:
* Compare conditions across multiple rooms or locations within a room
* See how temperature and humidity change over time in different spaces and room usage
* Export raw data for independent analysis, modeling, or integration with other tools
This project was designed to solve these problems by supporting additional remote sensors, providing detailed historical records, and offering easy exports for advanced analysis.


Project Overview
--------
This project is a self-hosted local web application that displays real-time and historical temperature and humidity data for an apartment. It features a clean dashboard for monitoring environmental conditions, spotting trends, and reviewing past changes. The system also includes API endpoints for retrieving stored data and for receiving readings from remote temperature/humidity sensors.

![Sample Dashboard Image](https://github.com/jackc-07/ClimateTrack/blob/main/dashboard.PNG?raw=true)

Key Features
--------
* Real-time data display for temperature and humidity
* Interactive historical charts for spotting trends over days, weeks, or months
* Local hosting - runs entirely on your own network
* REST API endpoints for
    * Retrieving stored temperature/humidity readings
    * Accepting incoming data from remote sensors
* Multi-room monitoring -- supports multiple remote sensors
* Automatic data logging for historical analysis
* Temperature and humidity change alerts
* Export historical data
* Customizable alert thresholds via API or UI
* Mobile-friendly responsive design


Technologies Used
-----------
* Backend: Python / Flask
* Frontend: HTML, CSS, JavaScript (with Chart.js for graphs)
* Database: MySQL for storing historical readings
* Sensors: remote temperature/humidity sensors using microcontrollers (Raspberry Pi Pico, Arduino)
* API: RESTful endpoints for both data retrieval and submission


Future Enhancements
---------
* Additional sensor types (C02, air quality, VOC, etc.) and presence detection for expanded environmental monitoring / modeling
* Weather API integration for comparison of indoor vs. outdoor conditions and additional external modeling of temperature change inside the apartment


