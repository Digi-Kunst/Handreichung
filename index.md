---
title: Handreichung
layout: home
---

# Handreichung

### Vorbereitende Arbeiten zur Datenerfassung
Bevor im Herbst mit der Erfassung der Daten begonnen werden kann, empfehlen wir, bereits jetzt einige grundlegende Schritte durchzuführen. 

- **Sichern** sie ihre Dateien vor Verlust. Sie sollten mindestens zwei, besser drei Kopien ihrer (Medien-)Daten haben. Am besten auf unterschiedlichen Speichermedien, aufbewahrt an unterschiedlichen Orten.
- Wir empfehlen, eine **Inventarliste** der digitalen Inhalte und der aktuellen Speicherorte anzulegen, um einen Überblick zu gewinnen. Auf Windows kann dafür [abeMeda](https://www.abemeda.com/) benutzt werden. Für Mac OS empfiehlt sich [NeoFinder](https://cdfinder.de/). Diese Programme erstellen detaillierte Kataloge der Inhalte von Datenträgern und lesen zusätzlich deren technische Metadaten aus. Selbstverständlich können auch andere entsprechende Digital-Asset-Management-Lösungen benutzt werden.
- Sorgen sie bitte dafür, dass mindestens folgende beschreibende **Metadaten** vorhanden sind: 

### Pflichtfelder für Metadaten

|:--------|:--------|
| Titel | Jedes Werk oder Projekt muss mindestens einen Titel haben. |
| Projektkategorie | Zur Klassifikation wird im späteren Erfassungs-Formular eine Taxonomie aller Kunst-Gattungen und deren Unterkategorien bereitgestellt, aus der Einträge ausgewählt werden können. Beispiele: *Kunst/Videokunst/Videoinstallation*, oder *Musik/Tanzmusik*. Man muss mindestens eine und kann beliebig viele Kategorien zuweisen. Bis das Erfassungs-Formular verfügbar ist, bitten wir darum, auf anderem Weg diesbezügliche Informationen festzuhalten. | 
| Schlagwörter zu Genre und Inhalt | Es wird die Funktion geben, Projekte über die Projektkategorie hinaus durch Verweise auf ein externes kontrolliertes Vokabular wie Wikidata inhaltlich zu erschließen. Beispiel: Ein Projekt wurde bereits als *Musik/	Klassische Musik	/Bühnenmusik* klassifiziert und bekommt zur weiteren Beschreibung die Schlagwörter *[Oper](https://www.wikidata.org/wiki/Q1344)* und (aufgrund z.B. einer thematischen Ausrichtung) *[Migration](https://www.wikidata.org/wiki/Q177626)* zugewiesen. Durch die Einbindung von Wikidata werden automatisch Synonyme und Definitionen ausgelesen und abgespeichert. |
| Inhaltliche Beschreibung im Freitext           | Bitte geben sie an dieser Stelle alle weiteren, ggf. unstruktierten Informationen an, die benötigt werden, um ihre Archivalien Dritten zu erschließen.    | 
| Personen und deren Rollen | Jedem Werk oder Projekt muss mindestens ein:e Akteur:in (meistens eine Person) zugeordnet sein. Personen werden mindestens mit vollständigem Namen und Geburtsdatum beschrieben. Personen haben im Rahmen eines Projekts mindestens eine Rolle inne (z.B. *Künstler:in, Interpret:in, Regisseur:in, Instrumentalist:in*). Bis wir eine Auswahlliste von möglichen Rollen bereitstellen können, bitten wir darum, auf anderem Weg diesbezügliche Informationen festzuhalten.  |
|Datum und dazugehöriges Ereignis |Zeitangaben sind immer verbunden mit Ereignissen. Beispiele: *Aufführung, Ausstellung, Konzert.* Wenn nichts Genaueres bekannt ist, würde man einem Werk mindestens das Ereignis *Herstellung* zuweisen.|
| Rechteangaben |Einverständniserklärung der Rechteinhaber zur Übernahme in das Archiv, auf Wunsch auch zur Veröffentlichung im Netz. Siehe Entwurf weiter unten. |


Dies sind die absoluten Mindestanforderungen. Diese Daten sollten möglichst strukturiert und zentralisiert abgelegt werden. Wenn noch kein System dafür vorhanden ist, bietet sich an, ein einfaches tabellarisches Formular zu benutzen.

Weitere Informationen zu den wichtigsten Feldern finden sich unten unter dem Punkt [Datenmodellierung](https://digi-kunst.github.io/Handreichung/#digi-kunst-datenmodellierung). Die volle Anzahl der im System angelegten Metadaten-Felder wird später an dieser Stelle dokumentiert werden. 

### Entwürfe zu 
- Einverständnis- und Übernahmeerklärung
- Rechteklärung
- Archivrichtlinie der Hochschule


### Weiterführende Lektüre

- Nicht alle Dateitypen sind archivtauglich. Gegebenenfalls sollte erwogen werden, Dateien zu konvertieren. Hier findet sich eine [Übersicht von gängigen Dateiformaten und deren Langzeitstabilität](https://www.lzv.nrw/dateiformate/) (lzv.nrw). 
- Schritte zum Sichern digitaler Inhalte: NDSA [Levels of Digital Preservation Matrix](https://osf.io/3na96). Hier finden sie weiterführende Informationen zu den oben erwähnten grundlegenden Schritten.
	

### Digi-Kunst Datenmodellierung 

Dieses [Diagramm](./assets/2023-03-21_Skizze_Datenmodellierung.pdf) zeigt, wie im Digi-Kunst Archiv die heterogenen Informationen der unterschiedlichen Einliefernden in ein logisches Verhältnis zueinander gebracht und integriert werden, und in welchen Entitäten (Tabellen) und Attributen (Feldern) die einzelnen Metadaten erfasst und verfügbar gemacht werden.

Im Zentrum steht das *Projekt*, meistens ein künstlerisches Werk. Das Projekt muss einen Titel haben, es lässt sich kategorisieren und inhaltlich beschreiben.  

Die mit dem Projekt verbundenen weiteren Informationen, wie z.B. Personen speichern wir in der Entität *Akteure* separat ab. Dadurch müssen wir diese Informationen nur einmal eingeben und später nur noch darauf verweisen. Dadurch vermeidet man Redundanzen und minimiert Fehler, z.B. leicht anders geschriebene Namen. 

Eine weitere wichtige Entität sind die *digitalen Objekte* oder Dateien. Diese sind entweder durch Retrodigitalisierung aus physischen Medien entstanden, oder sie sind *born digital*. Weitere Entitäten, teilweise noch in der Planung begriffen, lassen sich aus dem Diagramm ablesen.

Das Digi-Kunst Archiv ist ereignisbasiert strukturiert und wird wie im [Bericht des Vorprojekts](https://www.dh.nrw/kooperationen/Digi-Kunst.nrw%20%28Vorprojekt%29-63) erwähnt über Harvestingformate wie LIDO und MARC21 abfragbar sein.

Später werden wir an dieser Stelle Informationen zu den von uns entwickelten Taxonomien und kontrollierten Vokabularen bereitstellen.

---
Diese Handreichung wird kontinuierlich erweitert. Ansprechpartner an den Konsortialhochschulen werden per E-Mail über Updates informiert. Wir freuen uns über Fragen und Anregungen. Kontakt: [Digi-Kunst.nrw](https://www.rsh-duesseldorf.de/musikhochschule/wir-ueber-uns/digi-kunstnrw/) | zuletzt aktualisiert: 2023-04-12