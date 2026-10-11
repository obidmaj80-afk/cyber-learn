CyberLearn - site files
=======================
index.html  - the page (open it in a browser, or upload the folder to any static host)
style.css   - all styling (TryHackMe-style dark theme, light theme too)
app.js      - all logic: lessons, tools directory (150+), games, lab, link checker, translation, admin

Host it on your own domain (free options): Cloudflare Pages, Netlify, GitHub Pages.
Upload these 3 files, then connect your domain in the host's settings.

What works anywhere: lessons, tools directory, practice lab, fake-link checker, games, points,
quiz, sounds, animations, progress (saved in the browser).
What needs claude.ai: Cipher AI chat, translation, Code Academy teacher, voice/image chat,
visitor counter, admin panel. Outside claude.ai these show a message instead.
To run the AI on your own domain you need a small server that calls the Claude API.

Admin passphrase check: search app.js for AS and AH (salt and PBKDF2 hash, no plain password).
Decoy password hash: search for DH.

Single-file version: cyber-learn.html (the same site in one file).
