RAHUL WATCH MOBILE PWA

Files
- index.html
- manifest.webmanifest
- sw.js
- icons/icon-192.png
- icons/icon-512.png

Deployment
1. Upload the entire watchlist-mobile-app folder to an HTTPS location on the same site as your admin pages.
2. Keep all filenames and the icons folder unchanged.
3. Open index.html on your phone.
4. Android/Chrome: use Install app when offered, or the browser menu.
5. iPhone/Safari: tap Share, then Add to Home Screen.

Recommended location
Admin/mobile-watch/index.html

If deployed there, change the full-admin link in index.html from:
  href="watchlist-admin.html"
to:
  href="../watchlist-admin.html"

Notes
- The app uses the same Google Apps Script endpoint and watchlist.json as the desktop admin.
- Search requires an internet connection because it uses TMDB.
- If the server write fails, the entry is kept in a phone-local pending queue and retried when the app is online.
- Detailed collections and season editing stay in the full admin page.
- The current Google Apps Script write endpoint should be protected before publishing this URL broadly.
