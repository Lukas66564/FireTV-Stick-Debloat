# FireTV-Stick-Debloat

Debloating und Anpassung meines Fire TV Sticks über ADB und Pi-hole.

## Hintergrund und Umsetzung

Ich habe meinen Fire TV Stick schon seit längerer Zeit. Mit der Zeit ist er allerdings immer langsamer geworden. Jede Animation hat geruckelt und Apps haben ewig zum Starten gebraucht. Anstatt mir direkt einen neuen Fire TV Stick zu kaufen, habe ich mich dazu entschieden, meinen vorhandenen selbst zu modifizieren.

Zuerst habe ich die Entwickleroptionen meines Fire TV Sticks aktiviert. Dort konnte ich anschließend ADB einschalten und meinen PC mit dem Gerät verbinden.

Als Erstes habe ich die vorinstallierten Apps entfernt, die sich normalerweise nicht deinstallieren lassen, darunter Amazon Music, Prime Video und der Silk Browser.

Anschließend habe ich weitere Hintergrund- und Telemetriedienste deaktiviert, sofern das möglich war. Da sich allerdings nicht alle Dienste deaktivieren ließen, habe ich zusätzliche Telemetrie-Dienste auf DNS-Ebene über Pi-hole blockiert.

Damit bestimmte Änderungen nicht durch automatische Updates rückgängig gemacht werden, habe ich zusätzlich die Update-Server blockiert.

Außerdem habe ich weitere Sprachsteuerungsfunktionen hinzugefügt, um meinen Fire TV Stick besser über Alexa steuern zu können. Mehr dazu findet ihr in meinem [Home-Assistant-Projekt](https://github.com/Lukas66564/Home-Assistant).

## Ergebnis

Nach den Änderungen läuft mein Fire TV Stick wieder so flüssig wie damals, als ich ihn neu bekommen habe – und gefühlt sogar noch schneller.
