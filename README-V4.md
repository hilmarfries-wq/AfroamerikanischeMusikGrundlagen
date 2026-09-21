# Version 4 – Lehrerbereich

1. Dateien auf GitHub hochladen/ersetzen.
2. In `config.js` Project URL und den publishable/anon key eintragen. Niemals service_role/Secret-Key verwenden.
3. Zuerst die bisherige `supabase.sql`, danach `supabase-v4.sql` im Supabase SQL Editor ausführen.
4. Unter Authentication → Users einen Lehrer-Benutzer mit E-Mail und sicherem Passwort anlegen.
5. Dessen UUID kopieren und im SQL Editor ausführen:

    insert into public.teacher_users (user_id) values ('DEINE-USER-UUID');

Danach kann nur dieser freigegebene, angemeldete Benutzer die Testergebnisse lesen. Schüler können weiterhin Ergebnisse speichern, aber nicht die Ergebnisliste auslesen.
