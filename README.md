# City Weather Time
---

#### Video demo: https://youtu.be/hGQJtK54Tt0
---
---

### **Description**:
- This web app is the final project for CS50.

- It shows Weather, Time and map (Google map) about a city (or a location) using flask and javascript in addition to html and css.

- it works by searching for a city or a location, which transferred into coordinates using google geolocation api which are restored into to variables lat and lon (in helpers.py get_geolocation) then exported to javascript files to be used by the two weather functions and the google map function.

- The Weather is fetched using OpenWeatherMap api for current weather and Open-Meteo api for daily forecast.

- The current data are from open weather map api https://openweathermap.org/current. it shows an icon for the state of the current weather from the api, the temperature, wind speed, humidity and pressure. and for the today's high and low temperature the used api is the next "open meteo".

- And the forecast data are from open meteo api https://open-meteo.com/. shows the high and low temperature for the rest of the week or the upcoming six days by using the aforementioned lat and lon variables and the city's time zone name which is requested (in helpers.py get_timezone function) by the time zone api using the latitude and longitude of the location (lat and lon).

- the Time in a location is calculated by adding the time difference, which calculated by using timezonedb api (in helpers.py get_timezone) to get the GMT offset then adding it to the time zone offset of the user, and then adding it to the current time from the built in epoch timestamp.
- and the date by extracting the year, the month and the day form the calculated timestamp.
- And the sunrise and sunset from openweathermap api.

- The Map is from google maps api in addition to google geolocation api to get the coordinates of the searched location.

- and the navigator tool to get the location of the user to measure the distance between the user's location and the searched location using google geometry library.

---
### Languages used:

-   python
-   javasctipt
-   html
-   css
---

### Folders:
---
- Static contains js files (index, weather, time, map) and the css file.
- Templates contains html files (layout, index, weather, time, map).
- in addition to flask files app.py and helpers.py.
---
---

# Thank you Professor David and all CS50 Team, Thank you very much.
