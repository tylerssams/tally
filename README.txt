TALLY — how to install it as a real app (and stop losing data)

WHY THE LOCAL FILE FAILED
Opening the .html straight from your phone uses a "file://" address.
Phones treat those as temporary: they won't save data between sessions
and won't show an install option. You need a real web link (https://).
Hosting it (free, 2 minutes) fixes BOTH problems at once.

EASIEST HOST — NETLIFY DROP (no account needed)
1. On a computer, go to:  https://app.netlify.com/drop
2. Drag this WHOLE "tally-app" folder onto the page.
3. It gives you a link like  https://something.netlify.app
4. Open that link on your phone.

INSTALL IT ON YOUR PHONE
- Android (Chrome): open the link -> menu (3 dots) -> "Install app"
  (or "Add to Home screen"). It becomes a real app icon, full screen,
  and your data is saved permanently.
- iPhone (Safari): open the link -> Share -> "Add to Home Screen".

YOUR DATA
Saved on the device, in the app, automatically. Nothing is uploaded.
Close it, reopen it — it's all still there.

WANT AN ACTUAL .APK FILE?
Once it's hosted (step 3 above), go to https://www.pwabuilder.com,
paste your netlify link, and it generates a signed Android APK you can
install or put on the Play Store. This folder already has everything
PWABuilder needs (manifest + service worker + icons).

FILES IN THIS FOLDER (keep them together)
  index.html              the app
  manifest.webmanifest    makes it installable
  sw.js                   makes it work offline
  icon-192 / 512 / maskable.png   app icons
