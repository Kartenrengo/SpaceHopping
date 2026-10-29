# Trabant

Ein-Finger-Spiel nach der Mechanik von **Tiny Wings**, im Druck-Look von Trabant: Ein Komet surft über die Hügel der Raumzeit, von der Sonne bis zum Rand des beobachtbaren Universums.

## Steuerung
- **Halten:** Der Komet wird schwer und saust die Hügel hinab.
- **Loslassen** vor der Kuppe: Er hebt ab.
- **Flach auf einem Abhang landen** = Perfekt (+Tempo, +Punkte). Drei perfekte Landungen in Folge = **Fieber** (5 s doppelte Punkte, mehr Tempo).
- Steile Landung oder Landung bergauf = Holprig, das kostet Tempo.
- Das **Licht** läuft ab. Jedes erreichte Ziel bringt Licht dazu. Ist es aus, endet der Flug bei der nächsten Landung.

## Die Reise (echte Entfernungen)
| Ziel | Entfernung | Hügel |
|---|---|---|
| Merkur … Neptun | 58 Mio. km … 4,52 Mrd. km | 3–4 je Planet |
| Pluto (New Horizons 2015) | 5,9 Mrd. km | 3 |
| Heliopause (Voyager 1, 2012) | 18 Mrd. km | 4 |
| Proxima Centauri b | 4,2 Lichtjahre | 11 |
| TRAPPIST-1 | 41 Lichtjahre | 5 |
| Orionnebel | 1.344 Lichtjahre | 7 |
| Sagittarius A* | 27.000 Lichtjahre | 6 |
| Große Magellansche Wolke | 160.000 Lichtjahre | 5 |
| Andromeda | 2,5 Mio. Lichtjahre | 6 |
| JADES-GS-z14-0 (JWST 2024) | 13,4 Mrd. Lichtjahre Lichtweg | 12 |
| Kosmische Hintergrundstrahlung | 13,8 Mrd. Lichtjahre | 3 |

Maßstab logarithmisch: Jede Verzehnfachung der Entfernung bringt gut zwei Hügel mehr (`3 + 2,4 · log10(Entfernung / vorige Entfernung)`). Mit jedem Ziel werden die Hügel höher und länger.

## Technik
Eine Datei (`index.html`), läuft offline im Handy-Browser. Vollbild beim ersten Tipp, kein Zoom/Pull-to-Refresh, Pause beim App-Wechsel, Vibration, Bestwert bleibt auf dem Gerät.

Stellschrauben oben im Skript: `G`, `G_HOLD`, `PERFECT`, `FEVER_CHAIN`, `LIGHT_START`; pro Ziel `amp`, `len`, `bonus`.
