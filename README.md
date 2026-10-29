# Space Hopping

Ein-Tipp-Spiel nach dem Prinzip von Flappy Bird, im Weltraum: Tippen (oder Leertaste) gibt der Rakete Schub, die Schwerkraft zieht sie nach unten. Flieg durch die Lücken im Asteroidengürtel.

- Alle 5 Punkte steigt das Level, jedes Level ist ein Abschnitt des Sonnensystems (Merkur → Kuipergürtel).
- Tempo 140 → 265 px/s, Lücke 178 → 112 px, Abstand 235 → 160 px (Maximum ab Level 9).
- Eine Datei (`index.html`), läuft offline im Handy-Browser. Bestwert bleibt auf dem Gerät gespeichert.
- Android: Vollbild beim ersten Tipp, kein Zoom/Pull-to-Refresh, Pause beim App-Wechsel, Vibration bei Crash und Levelwechsel.

Stellschrauben stehen oben im Skript (`GRAVITY`, `FLAP`, `SPEED`, `GAP`, `SPACING`, `MAX_SHIFT`).
