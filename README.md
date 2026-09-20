# Online-Test: Anfänge afroamerikanischer Musik (Klasse 9)

Fertige statische Web-App für GitHub Pages + optional Supabase.

## Enthalten
- 20 Aufgaben / 30 Punkte
- Antwortmöglichkeiten bewusst ähnlich lang formuliert, damit die richtige Lösung nicht am Schriftbild erkennbar ist
- automatische Punkte-, Prozent- und Notenberechnung
- 50–51,9 % = 4−
- Erklärung zu jeder Aufgabe
- optionale Speicherung der Ergebnisse in Supabase
- keine öffentliche Leseberechtigung für Schüler-Ergebnisse

## GitHub Pages
1. Neuen GitHub-Repository anlegen.
2. `index.html`, `style.css`, `app.js` und `config.js` hochladen.
3. Repository: **Settings → Pages**.
4. Unter **Build and deployment**: `Deploy from a branch`, Branch `main`, Ordner `/ (root)`.
5. Speichern. GitHub zeigt danach die öffentliche Test-URL an.

## Supabase
1. Supabase-Projekt anlegen.
2. Im SQL Editor den Inhalt von `supabase.sql` ausführen.
3. In Supabase unter Project Settings/API die Project URL und den **anon/public key** kopieren.
4. In `config.js` eintragen.
5. Änderungen zu GitHub pushen.
6. Ergebnisse stehen in Supabase unter Table Editor → `test_results`.

Wichtig: Der anon/public key darf bei einer Browser-App öffentlich sein, **wenn Row Level Security korrekt eingerichtet ist**. Niemals den `service_role`-Key in `config.js` eintragen.

## Notenschlüssel
95–100: 1+  
90–94,9: 1  
85–89,9: 1−  
80–84,9: 2+  
75–79,9: 2  
70–74,9: 2−  
65–69,9: 3+  
60–64,9: 3  
55–59,9: 3−  
53–54,9: 4+  
52–52,9: 4  
50–51,9: 4−  
45–49,9: 5+  
40–44,9: 5  
30–39,9: 5−  
unter 30: 6

Der Schlüssel lässt sich in `app.js` in `getGrade()` leicht ändern.

## Fachlicher Hinweis
Der Test vermeidet die pauschale Aussage, es habe überall in den USA zu jeder Zeit dasselbe „Trommelverbot“ gegeben. Er unterscheidet außerdem Spirituals von der späteren Gospel-Tradition.

## Version 3
Die Positionen der richtigen Antworten sind gleichmäßig auf A, B, C und D verteilt (je 5-mal), ohne einfaches Rotationsmuster.
