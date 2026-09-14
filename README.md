# The Portugues Way V24.1a

V24.1a is the GitHub Pages-ready installation build for the October 2026 Camino Português trip.

## Public app name
**The Portugues Way**

This name is used for the PWA manifest and iPhone Home Screen so it is not confused with third-party apps named “Buen Camino”.

## GitHub Pages deployment
1. On Windows, create a public GitHub repository, for example `the-portugues-way`.
2. Upload the **contents of this `camino-app` folder**, including the `routes/` folder and all seven GPX files.
3. Enable GitHub Pages for the repository, publishing the `main` branch from `/`.
4. GitHub will publish an HTTPS address such as `https://YOUR-NAME.github.io/the-portugues-way/`.
5. Open that address in Safari on the iPhone.
6. Choose **Share → Add to Home Screen → Open as Web App → Add**.

## Seven bundled route files
The PWA is prepared to automatically retrieve these files from the GitHub Pages `routes/` directory and cache valid GPX files locally:

1. `day-01-tui-o-porrino.gpx`
2. `day-02-o-porrino-redondela.gpx`
3. `day-03-redondela-pontevedra.gpx`
4. `day-04-pontevedra-armenteira.gpx`
5. `day-05-armenteira-vilanova.gpx`
6. `day-06-pontecesures-o-milladoiro.gpx`
7. `day-07-o-milladoiro-santiago.gpx`

**Important:** V24.1a bundles the seven validated GPX tracks supplied by the user. The app automatically loads them from GitHub Pages on first use and retains them locally for offline navigation. Manual GPX import remains available as a fallback.

## Offline behavior
After the app and valid route files have been cached on the phone, GPS route tracking can work without cellular/Wi-Fi. A detailed offline basemap is still a separate dataset and must be supplied as a properly licensed GeoJSON package.

## Safety rule
**No real GPX = no live route guidance.** The app deliberately locks navigation for any stage that has not loaded a valid track.
