# shad0w.x7 PWA

Files:
- index.html — upgraded app
- manifest.webmanifest — PWA identity/install configuration
- sw.js — offline app-shell caching
- icons/ — supplied shad0w.x7 artwork at PWA sizes
- index.original.html — original uploaded source

Important:
A service worker/PWA installation requires the app to be served from HTTPS or from localhost.
Opening index.html directly as file:// will still run the app, but browser PWA installation/offline service-worker registration will not activate.

For local testing:
1. Put this folder on the device.
2. Run a local web server from this folder, e.g. `python3 -m http.server 8000`
3. Open `http://localhost:8000/` on the device/browser.
4. Use the browser's Install app / Add to Home Screen option.

The existing localStorage-based app data is preserved; this upgrade adds the PWA shell around it.
