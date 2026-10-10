# Quranic AR – Hiro marker AR demo (AR.js + A-Frame)

STATUS: CREATED — REQUIRES REAL-PHONE TESTING. Camera tracking has not been tested.

Files (keep all three in the SAME folder):
- index.html – AR demo (Malay/English instruction screen, AR scene, button to learning module)
- quranic-ar-prototype.html – existing non-AR learning module
- hiro-marker-print.html – print page for the official Hiro marker image

Libraries (loaded from the internet, free, no key): A-Frame 1.3.0 (aframe.io) and AR.js 3.4.5 marker build (raw.githack.com, tag 3.4.5).
AR.js also fetches its own Hiro pattern and camera data from its official repository at run time, so the phone needs internet.

## Free HTTPS hosting (GitHub Pages) – YOU must do this
1. Create a free account at github.com.
2. New repository -> name it e.g. quranic-ar -> Public -> Create.
3. "uploading an existing file" -> drag the three files in -> Commit changes.
4. Settings -> Pages -> Source: Deploy from a branch -> Branch: main, folder: / (root) -> Save.
5. Wait 1-3 minutes. Your address: https://YOUR-USERNAME.github.io/quranic-ar/
(Alternative: Netlify Drop or Cloudflare Pages free tiers; check their current terms yourself.)

## Test on Android with Chrome
1. On a laptop, open https://YOUR-USERNAME.github.io/quranic-ar/hiro-marker-print.html and print on matte A4 (or show the marker on the laptop screen).
2. On the phone, open the main address in Chrome (not inside WhatsApp/Facebook).
3. Check the Malay instructions appear, then press Mula AR and tap Allow for the camera.
4. Point at the marker (whole black frame visible, good light). Expect: rotating ring and book above the marker, text panel, and a text description at the bottom.
5. Move the marker; cover it; expect the description to disappear when tracking is lost.
6. Press Modul pembelajaran: the learning module should open.
7. Record phone model, Android and Chrome versions, and pass/fail for each step.
Local laptop testing: http://localhost is treated as secure by Chrome; a phone needs HTTPS.

## If the libraries do not load
Open each script URL from index.html directly in a browser. If one is missing, replace it with the URL from the AR.js docs and re-test.
