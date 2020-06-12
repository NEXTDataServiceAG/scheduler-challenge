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

Gibt es eine Liste von Ärzte und den Skills die sie haben?

- Diese Informationen sind natürlich Teil des realen Problems, im Rahmen der Challenge sind sie allerdings nicht relevant.

Gibt eine Liste von Räumen und den Arten von OPs die dort stattfinden können? 

- Diese Informationen sind auch Teil des realen Problems, im Rahmen der Challenge allerdings nicht relevant.

Gibt es eine Liste an Operationen + Skills die benötigen + ist die Anzahl der Ärzte variabel?

- Geht von einem "1. Operateur" je OP aus. Im realen Problem es das natürlich komplexer.

Warum ist die duration mit Nachkommastellen? Ist die Einheit Sekunde? Kann man die Länge der OP auf Minuten Runden?

- Genau, die Einheit ist in Sekunden angegeben. Entscheidet für Eure Lösung selbst, ob eine Rundung sinnvoll ist oder nicht. Bitte macht Eure Entscheidung mindestens im Code-Kommentar kenntlich.

Was ist cleanessMapped?

- Umso höher die Kennzahl, desto höher ist die Anforderung an die Sauberkeit des Raumes.

Wird eine Pause zwischen den OPs benötigt? Wenn ja wie lange und wo steht das?

- Nehmt an, dass alle OPs im selben OP-Trakt stattfinden und normale Zeiten zwischen OPs zur Vorbereitung und Laufwege eingeplant werden müssen.

Von wann bis wann dürfen OPs durchgeführt werden? (Mo- Fr 8-18Uhr o.Ä.?) Ist das in jedem Raum gleich?

- Im Rahmen der Challenge kann Mo-Fr. 8 - 18 Uhr angenommen werden.

Wie sind die Arbeitszeiten und Pausenzeiten der Ärzte geregelt?

- Im Rahmen der Challenge kann Mo-Fr. 8 - 18 Uhr angenommen werden.

Wie soll was verdrängt werden? Gibt es nur „Notfälle“ die sofort stattfinden sollen und dann wird anhand der urgencyMapped die Dringlichkeit sortiert? Und was ist dringender 1 oder 10?

- Für die urgencyMapped gilt das gleiche wie bei der Sauberkeit: Umso Höher desto Dringender.

Wie soll mit den Planungen umgegangen werden? Man kann ja den Patienten, der zu einer Routine Handoperation ambulant kommen soll und heute in 2 Wochen geplant wird, schlecht jeden Tag oder jede Stunde einen neuen Termin nennen, da immer andere evtl. etwas dringlichere Termine dazu kommen.

- Der Plan sollte die drei folgenden Kriterien optimieren:

•	Robustheit: Weniger Verschiebungen = Besser

•	Raumauslastung: Höher = Besser

•	Überstunden: Weniger = Besser

Was bedeuten die Farben in den Beispielplänen?

- In den Beispielplänen sind die Farben nicht bedeutend, sie dienen lediglich zur besseren Lesbarkeit.

Kann es mehrere tobetimes geben? (Hab den Datensatz nur überflogen und nicht alles gecheckt)

- Nein

