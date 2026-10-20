# picks-app.de: Liga-Einladungen

Kleinste mögliche Seite für Einladungslinks wie `https://picks-app.de/liga/K7M2QX`
(Gründer, 18.10.2026: Einladen soll einen Link teilen, am besten ohne Code).

- `.well-known/apple-app-site-association`: sagt iOS, dass `/liga/*` zur App
  `975DQY3RWN.app.picks.ios` gehört. Ist PICKS installiert, öffnet der Link die App direkt
  bei „Liga beitreten“ mit dem Code; die Seite selbst sieht man dann nicht.
- `liga.html`: für alle ohne App. Link zu TestFlight (später App Store) und der Code aus dem Pfad.
  Keine Cookies, keine fremden Skripte, Schriften oder Bilder.
- `404.html`: dieselbe Seite für GitHub Pages, das `/liga/K7M2QX` sonst nicht findet.
- `_redirects` und `_headers`: dasselbe für Cloudflare Pages oder Netlify.
- `.nojekyll`: damit GitHub Pages den Ordner `.well-known` ausliefert.
- `CNAME`: die eigene Domain für GitHub Pages.

**Veröffentlicht** am 20.10.2026 nach Freigabe des Gründers („ja warum nicht? dafür brauche ich
ja nicht das Impressum“), als GitHub-Pages-Repository `m8gd268kbn-art/picks-app.de`.
Änderungen hier machen und dort hochladen. Schritte und Stand: `release/LIGA-LINK.md`.
