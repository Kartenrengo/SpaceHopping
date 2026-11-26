# Trabant

Planeten-Hopping mit der Schwung-Mechanik von **Tiny Wings**, im Druck-Look von Trabant: Ein Komet holt in der Umlaufbahn Anlauf und springt von der Sonne bis zum Rand des beobachtbaren Universums.

## Steuerung
- **Halten auf dem Weg nach innen:** Die Schwerkraft des Planeten wird stärker, der Komet stürzt in den Schwerkrafttrichter und wird schneller (wie bergab bei Tiny Wings).
- **Loslassen auf dem Weg nach außen:** Der Komet schwingt mit dem neuen Tempo hinaus. So holt man Runde für Runde mehr Schwung.
- **Schwung-Ring** um den Kometen: Ist er voll, reicht der Schwung zum Abflug. Dann hält man weiter, bis die gepunktete Vorschau ein Ziel trifft (es leuchtet auf, die Zeit läuft langsamer), und lässt los.
- **Mehr Anlauf = weiter fliegen:** Die Reichweite wächst mit dem Schwung. Bei viel Schwung fliegt der Komet zu schnell durch das nächste Schwerefeld und landet erst dahinter, das gibt 10 × k² Punkte (k = Anzahl Ziele).
- **Flach einfliegen** = Perfekt, der Schwung bleibt. Drei perfekte Einflüge in Folge = **Fieber** (8 s doppelte Punkte, das Licht steht still).
- **Zu tief gestürzt:** Der Komet streift den Planeten und verliert Tempo. **Ins Leere geflogen:** Er wird zum letzten Ziel zurückgeholt, das kostet 3 s Licht.
- Das **Licht** läuft ab, jedes neue Ziel bringt Licht dazu. Ist es aus, zählt nur noch der laufende Flug.

## Die Reise (echte Entfernungen)
| Ziel | Entfernung |
|---|---|
| Merkur … Neptun | 58 Mio. km … 4,52 Mrd. km |
| Pluto (New Horizons 2015) | 5,9 Mrd. km |
| Heliopause (Voyager 1, 2012) | 18 Mrd. km |
| Proxima Centauri b | 4,2 Lichtjahre |
| TRAPPIST-1 | 41 Lichtjahre |
| Orionnebel | 1.344 Lichtjahre |
| Sagittarius A* | 27.000 Lichtjahre |
| Große Magellansche Wolke | 160.000 Lichtjahre |
| Andromeda | 2,5 Mio. Lichtjahre |
| JADES-GS-z14-0 (JWST 2024) | 13,4 Mrd. Lichtjahre Lichtweg |
| Kosmische Hintergrundstrahlung | 13,8 Mrd. Lichtjahre |

Maßstab logarithmisch: Der Abstand zum nächsten Ziel wächst mit jeder Verzehnfachung der echten Entfernung um 70 Einheiten (mindestens so viel, dass sich die Schwerefelder nicht berühren). Spätere Ziele drehen schneller und fangen weniger großzügig ein.

## Technik
Eine Datei (`index.html`), läuft offline im Handy-Browser. Vollbild beim ersten Tipp, kein Zoom/Pull-to-Refresh, Pause beim App-Wechsel, Vibration, Bestwert bleibt auf dem Gerät.

Stellschrauben oben im Skript: `K_HOLD` (Schwerkraft beim Halten), `CAPF` (wie großzügig eingefangen wird), `V_LAUNCH`/`SW_MAX`/`DRAG` (Reichweite), `AIM_HELP` (Zielhilfe), `SLOWMO`, `PERFECT`, `FEVER_CHAIN`, `LIGHT_START`; Umlaufzeit und Feldgröße in `setupBody`.
