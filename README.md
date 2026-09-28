# Mausam - Pakistan Weather App

A sample web development project. Pick or add any place in Pakistan and see live conditions,
a 24-hour outlook and a 7-day forecast. Data comes from [Open-Meteo](https://open-meteo.com) (free, no API key).

**Stack:** HTML, CSS, Tailwind CSS (CDN), vanilla JavaScript, Node.js + Express.

## Run it

```bash
npm install
npm start
```

Open http://localhost:3000 (needs Node 18 or newer).

## Structure

```
server.js            Express server, proxies Open-Meteo weather, air quality and geocoding
public/index.html    Page layout (Tailwind utility classes)
public/css/style.css Custom component styles
public/js/app.js     Locations, search, rendering
```

## Notes

- Default places: Bhakkar, Sargodha, Mianwali, Karachi, Multan, Nawan Jandanwala, Kalorkot.
  Coordinates for the smaller towns are approximate. Search for the exact place to add a precise one.
- Added locations are saved in the browser (localStorage).
- Tailwind loads from its CDN, which is fine for a sample. For production, install Tailwind
  and compile the CSS with the Tailwind CLI.
