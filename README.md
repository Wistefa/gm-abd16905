# Gesundheitsmappe

Einzel-HTML-App (`index.html`) für **Medikamenten-Einnahme** und **Arzttermine**, für zwei Personen (Joper und Partnerin).

- **Daten nur auf dem Gerät** (localStorage, Schlüssel `gesundheitsmappe.v1`). Kein Server, keine Cloud, keine externen Schriften/Skripte.
- **Sicherung:** Einstellungen → „Sichern (Datei)“ erzeugt `gesundheitsmappe-sicherung-DATUM.json`; „Datei einlesen“ stellt wieder her (auch für Gerätewechsel).
- **Erinnerungen:** die App klingelt nicht selbst. Je Einnahmezeit „In Erinnerungen anlegen“ (iOS-Teilen-Fenster → Erinnerungen, dort Uhrzeit + „Täglich“ einmalig setzen). Arzttermine: „In Kalender“ erzeugt eine `.ics`-Datei mit Warnung am Vortag und 2 Stunden vorher.
- **Funktionen:** Heute (abhaken, überspringen, überfällig), Medikamente (Uhrzeiten, Wochentage, Vorrat zählt herunter, Rezept-Warnung), Termine (Fragen, Mitbringliste, Ergebnis), Verlauf (14 Tage, Einnahmetreue), Übersicht für den Arzt (Teilen/Drucken), zwei Personen.
- **iPhone:** in Safari „Teilen → Zum Home-Bildschirm“, dann behält iOS die Daten zuverlässiger.

Getestet (Chromium, Handy-Format): Einrichtung, Medikament anlegen, Einnahme/Rücknahme mit Vorrat, Überspringen, Wochentage, Termin, .ics (VALARM), Personenwechsel, Verlauf, Arzt-Übersicht, Sicherung/Einlesen, Löschen, Neuladen. Nicht getestet: iPhone-Safari (Teilen → Erinnerungen, .ics → Kalender).

Kein medizinischer Rat; keine Prüfung von Wechselwirkungen.
