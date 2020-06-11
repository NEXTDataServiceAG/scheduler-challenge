# scheduler-challenge

## Problem

In der Chirurgie kann der kleinste Fehler über Leben und Tod entscheiden. Bevor ein Arzt aber das Skalpell anlegt, muss jede OP erst intern geplant werden. Neben einem freien Zeits-lot, muss auch ein passender Arzt und Raum gefunden werten, die den Anforderungen der Operation gerecht werden. Dabei kann jede OP, die zusätzlich eingeplant wird potentiell Leben retten oder Anstrengungen und Leiden von Arzt und Patienten drastisch verringern. Lastet man Chirurgen aber mit unnötigen Überstunden und Sonderschichten zu sehr aus, können die Konsequenzen dramatisch sein. Wenn ein Notfall auftritt, muss der Plan möglichst schnell aktualisiert werden, um direkt zu sehen, wo die OP eingeplant werden kann.

Für diese Herausforderung  sollt Ihr eine Lösung entwickeln: ein  Programm, das aus allen zur Verfügung stehenden Parametern und bereits stattgefundenen Operationen die Daten analy-siert und die OP-Planung optimal erstellt.


## Datensatz

Wir haben für euch aus einem unserer Produkte einen Teildatensatz extrahiert. Es sind reale Daten die wir für diese challenge anonymisiert haben. Auf Github <link> könnt ihr euch die Repo klonen. Hier eine Übersicht einiger Parameter:
- empId: Operiender Arzt
- personId: Patient
- regDate: Wann die Op ins system eingetragen wurde
- opRoom: Raumkennzeichnung
- disciplin: Art der Op, Je nach Disziplin wurden passende Ärzte und Räume ausge-wählt. 
- urgencyMapped: Wie dringlich ist die Op
- Duration: Wie lange dauert die op (in Sekunden)


## Fragen, die ihr euch beim Coden stellen solltet:

- Wie verteilen wir Ärzte auf Räume?
- Wie verteilen wir Ops auf Räume?
- Wie berechnen wir einen guten Schedule?


## Eine gute Lösung sollte:

- Bestmögliche Auslastung der Ärzte und Räume ermöglichen
- Leerlaufzeiten der Räume und Ärzte minimieren, Anzahl und Pace maximieren
- Berechnungszeit minimieren:

-1 Stunde? Cool und reiche deine Lösung an die Mail unten ein

-10 Minuten? Schick deine Mail direkt an unseren Projektleiter René (rene@next-data-service.com) 

-20 Sekunden? Schick deine Mail bitte direkt an unseren CTO (stephan@next-data-service.com)


## Rahmenbedingungen

Laufzeitumgebung, Programmiersprache, Datenbank? Was auch immer Ihr braucht um Eure Lösung zu schaffen. Wir sollten Euer Ergebnis aber reproduzieren können. Euer Code sollte also bei uns laufen. Wenn Ihr dafür einen Quantencompu-ter braucht, wäre es super, wenn ihr ihn uns für das Testen eures Codes zur Verfü-gung stellt.

## Teilnahme

Ihr dürft in Zweierteams arbeiten oder eure Lösung alleine einreichen.
Bitte stellt eure Lösung in einem Github zur Verfügung und Schickt uns den Link per Mail. Das Repo sollte

- Eure Ergebnisse und 
- den Source Code mit ausführlicher Dokumentation (inkl. Liste der Depen-dencies) enthalten. 

Fügt eurer Mail bitte außerdem den ausgefüllten Steckbrief (ein Beispiel findet ihr im challenge repo) und wenn ihr möchtet einen Lebenslauf hinzu.

Einreichungsfrist: 22. Juni 2020, 23.59 Uhr
Einreichen an: challenge@next-data-service.com

## FAQ

Hier beantworten wir Eure Fragen, die ihr uns per Mail an challenge@next-data-service.com stellt.
