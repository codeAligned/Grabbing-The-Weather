# Grabbing-The-Weather
[![Build Status](https://travis-ci.org/Acesonnall/Grabbing-The-Weather.svg?branch=master)](https://travis-ci.org/Acesonnall/Grabbing-The-Weather) [![dependencies Status](https://david-dm.org/Acesonnall/Grabbing-The-Weather/status.svg)](https://david-dm.org/Acesonnall/Grabbing-The-Weather) [![devDependency Status](https://david-dm.org/Acesonnall/Grabbing-The-Weather/dev-status.svg)](https://david-dm.org/Acesonnall/Grabbing-The-Weather#info=devDependencies)
<br />
A program that prompts for a city name and returns the current temperature for the city using OpenWeatherMap API <br />
## How to run
1. Verify you are running latest stable version of node
2. Clone repository and "cd" into folder
3. Set environment variable "APIKEY" to api key value retrieved from openweatherapi.org
   1. Add .env file to root folder
   2. Add line "APIKEY=*< YOUR API KEY >*"
4. Type **npm start** into the terminal
## How to test
1. Follow steps 1 to 3 of "How to run"
2. Type **npm test** into the terminal
## Folder Structure
- app.js (Application entry point/Server configuration)
- /app (App core)
  - /routes (App routes)
    - routes.js (Server handle for weather related client requests)
- /public (statically served files for client use)
  - /css (local CSS)
    - basic.css (Basic HTML stylesheet for views)
  - /files (local files)
    - city.list.json (City ID lookup database) **[doesn't need to be public]**
  - /js (local JS)
    - curr_weather.js (Scripting for HTML)
- /views (Client user interface)
  - curr_weather.html (Domain page)
- /test (software testing folder)
  - tests.js (BDD style testing with Chai)
  
## Technologies Used
### Front-End
#### Languages
- HTML/CSS
- JavaScript
#### Frameworks
- Bootstrap (CSS/JS)
- JQuery (JS)
- Materialize (CSS/JS)
### Back-End
#### Languages
- Node.js (JavaScript)
#### Frameworks
- Babel (Next-gen JS compiler)
- Express.js (Web framework)
- Morgan (HTTP request debug logging)
- Request (HTTP request client)
- Body-parser (Body parsing)
- Compression (Gzip compression)
- Express-minify (Minification)
- Countrynames (Country name/code mapper)
#### Test Frameworks
- Chai (BDD / TDD assertion framework)
- Mocha (JS testing)
- SuperTest (HTTP server testing)
### Continuous Integration
- Travis CI
## Demo
![Grabbing The Weather Demo](https://github.com/Acesonnall/Grabbing-The-Weather/blob/master/Project_Resources/Grabbing%20The%20Weather%20Demo.gif?raw=true)
