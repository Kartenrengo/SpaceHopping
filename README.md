# Trabant

Ein-Tipp-Spiel nach der Mechanik von Flappy Bird, im Druck-Look von Trabant: Ein Komet fliegt von der Sonne bis zum Neptun. Tippen (oder Leertaste) gibt Schub, die Schwerkraft zieht ihn nach unten. Flieg durch die Lücken im Gestein.

- **Jeder Planet ist ein Level.** Echte Namen und echte Abstände zur Sonne (NASA Planetary Fact Sheet).
- **Strecke nach echten Abständen.** Die Anzahl der Gesteinsfelder bis zum nächsten Planeten ist die echte Lücke in AE hoch 0,3: innen 3–4 Felder, Mars→Jupiter durch den Asteroidengürtel 7, außen 10. Aus 40:1 wird 3:1, die Reihenfolge bleibt.
- **Schwierigkeit wie beim Vogelspiel:** Tempo 140 → 265 px/s, Lücke 178 → 112 px, Abstand 235 → 160 px. Maximum ab Level 11 (Runde 2).
- Nach Neptun gibt es +5 und es geht in die nächste Runde ab der Sonne.
- Jede Runde neue Druckfarben, Bestwert bleibt auf dem Gerät gespeichert.
- Android: Vollbild beim ersten Tipp, kein Zoom/Pull-to-Refresh, Pause beim App-Wechsel, Vibration bei Crash und Planet.

Eine Datei (`index.html`), läuft offline im Handy-Browser. Stellschrauben oben im Skript: `GRAVITY`, `FLAP`, `SPEED`, `GAP`, `SPACING`, `LEVELS_TO_MAX`, `MAX_SHIFT`, `COLS_K`, `GAP_P`.
