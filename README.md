# WG1 Lern-Quiz (PWA)

Installierbare Lern-App: 100 Fragen, Lern- und Prüfungsmodus mit Timer, Statistik, eigene Fragen.
Alle Daten bleiben lokal im Browser des Geräts.

## Veröffentlichen (einmalig, kostenlos) – GitHub Pages
1. Auf github.com ein neues Repository anlegen (z. B. `wg1-quiz`), alle Dateien dieses Ordners hochladen.
2. Repository → Settings → Pages → Branch `main`, Ordner `/ (root)` → Save.
3. Nach ca. 1 Minute ist die App unter `https://<dein-name>.github.io/wg1-quiz/` erreichbar.

(Alternativ: Netlify Drop – den Ordner auf app.netlify.com/drop ziehen.)

## Installieren
- Android/Chrome: Seite öffnen → Menü ⋮ → „App installieren“ / „Zum Startbildschirm“.
- iPhone/Safari: Teilen-Symbol → „Zum Home-Bildschirm“.
- PC (Chrome/Edge): Installations-Symbol in der Adressleiste.
Danach läuft sie auch offline.

## Lokal testen
`python3 -m http.server 8000` im Ordner, dann http://localhost:8000 öffnen.
(Offline-Modus braucht http://localhost oder https.)

## Nach Änderungen an data.js oder index.html
In `sw.js` die Zahl in `CACHE = "wg1quiz-v1"` erhöhen (v2, v3 …), sonst zeigen installierte Apps die alte Version.
