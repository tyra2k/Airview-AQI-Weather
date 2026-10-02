# Airview — AQI & Weather

React + TypeScript + Tailwind CSS, packaged with Next.js for local development.
Includes the AQI dashboard, city search, location access, current weather,
24-hour weather outlook, seven-day forecast and home-screen web app assets.
Weather and air-quality estimates come from Open-Meteo; no API key is required.

## Run on your computer

1. Install Node.js 22.13 or newer.
2. Extract the ZIP and open this folder in VS Code.
3. Open the terminal in this folder and run:

```sh
npm install
npm run dev
```

4. Open http://localhost:3000 in your browser.

On Windows PowerShell, if npm.ps1 is blocked, use `npm.cmd install` and
`npm.cmd run dev` instead.

## Production

```sh
npm run build
npm start
```

Deploy the folder with a hosting provider that supports Next.js.
Use HTTPS for location access and home-screen installation.
This is a mobile-friendly web app, not an Android APK or iOS app binary.

## Main files

- app/page.tsx — AQI dashboard, location search and page layout
- app/weather.tsx — weather data and forecast components
- app/globals.css — shared styling and Tailwind import
- public/ — icons, web manifest and service worker

## Data and verification

AQI uses the US scale, not Malaysia's official API. Data are model estimates.
Attribution links to Open-Meteo and Copernicus CAMS remain in the app.
Live forecasts need internet access. Offline navigation shows an offline message.
The hosted version passed its build and live API checks. This download retains
its UI source and uses standard Next.js scripts instead of the hosted build wrapper.
Mobile installation and visual browser testing have not been verified.
