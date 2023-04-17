---
title: Handreichung
layout: home
---

# Handreichung

### Vorbereitende Arbeiten zur Datenerfassung
Bevor im Herbst mit der Erfassung der Daten begonnen werden kann, empfehlen wir, bereits jetzt einige grundlegende Schritte durchzuführen. 

- **Sichern** sie ihre Dateien vor Verlust. Sie sollten mindestens zwei, besser drei Kopien ihrer (Medien-)Daten haben. Am besten auf unterschiedlichen Speichermedien, aufbewahrt an unterschiedlichen Orten.
- Wir empfehlen, eine **Inventarliste** der digitalen Inhalte und der aktuellen Speicherorte anzulegen, um einen Überblick zu gewinnen. Auf Windows kann dafür [abeMeda](https://www.abemeda.com/) benutzt werden. Für Mac OS empfiehlt sich [NeoFinder](https://cdfinder.de/). Diese Programme erstellen detaillierte Kataloge der Inhalte von Datenträgern, lesen technische Metadaten der Dateien aus und können die Ergebnisse in gebräuchliche Tabellenformate exportieren. Selbstverständlich können auch andere entsprechende Digital-Asset-Management-Lösungen benutzt werden.
- Sorgen sie bitte dafür, dass mindestens folgende beschreibende **Metadaten** vorhanden sind: 

### Pflichtfelder für Metadaten

|:--------|:--------|
| Titel | Jedes Werk oder Projekt muss mindestens einen Titel haben. |
| Projektkategorie | Zur Klassifikation wird im späteren Erfassungs-Formular eine Taxonomie aller Kunst-Gattungen und deren Unterkategorien bereitgestellt, aus der Einträge ausgewählt werden können. Beispiele: *Kunst/Videokunst/Videoinstallation*, oder *Musik/Tanzmusik*. Man muss mindestens eine und kann beliebig viele Kategorien zuweisen. Bis das Erfassungs-Formular verfügbar ist, bitten wir darum, auf anderem Weg diesbezügliche Informationen festzuhalten. | 
| Schlagwörter zu Genre und Inhalt | Es wird die Funktion geben, Projekte über die Projektkategorie hinaus durch Verweise auf ein externes kontrolliertes Vokabular wie Wikidata inhaltlich zu erschließen. Beispiel: Ein Projekt wurde bereits als *Musik/	Klassische Musik	/Bühnenmusik* klassifiziert und bekommt zur weiteren Beschreibung die Schlagwörter *[Oper](https://www.wikidata.org/wiki/Q1344)* und (aufgrund z.B. einer thematischen Ausrichtung) *[griechische Mythologie](https://www.wikidata.org/wiki/Q34726)* zugewiesen. Durch die Einbindung von Wikidata werden automatisch Synonyme und Definitionen ausgelesen und abgespeichert. |
| Inhaltliche Beschreibung im Freitext           | Bitte geben sie an dieser Stelle alle weiteren, ggf. unstrukturierten Informationen an, die benötigt werden, um ihre Archivalien Dritten zu erschließen.    | 
| Akteur:innen und deren Rollen | Jedem Werk oder Projekt muss mindestens ein:e Akteur:in zugeordnet sein. Das kann eine Person oder Körperschaft sein. Diese werden mindestens mit vollständigem Namen und ggf. Geburtsdatum beschrieben. Personen haben im Rahmen eines Projekts mindestens eine Rolle inne (z.B. *Künstler:in, Interpret:in, Regisseur:in, Instrumentalist:in*). Bis wir eine Auswahlliste von möglichen Rollen bereitstellen können, bitten wir darum, in ihren eigenen Worten diesbezügliche Informationen festzuhalten.  |
|Ereignisse| Projekte sind mit Ereignissen verbunden. Beispiele: *Aufführung, Ausstellung, Konzert, Bearbeitung.* Wenn nichts Genaueres bekannt ist, würde man einem Werk mindestens das Ereignis *Herstellung* zuweisen.|
|Datum | Zeitpunkt oder Zeitraum, in dem Ereignisse stattgefunden haben. |
| Rechteangaben |Liegt eine Einverständniserklärung der Rechteinhaber zur Übernahme in das Archiv, auf Wunsch auch zur Veröffentlichung im Netz vor? Wir stellen unter dem Punkt **Vorlagen** demnächst einen Entwurf für eine Erklärung bereit. |


Die obige Tabelle stellt dar, welche Informationen schon vor Beginn der formellen Erfasssung bereits jetzt gesammelt und  zusammengeführt werden können, besonders wenn diese bisher nicht (oder nicht alle) strukturiert erfasst wurden. Wenn an ihrer Hochschule noch kein System dafür vorhanden ist, können sie dafür dieses einfache tabellarische [Formular](./assets/2023-04-13-Datenaufbereitung-Digi-Kunst.xlsx) benutzen.

Selbstverständlich kann das Formular auch benutzt werden, über diese Mindestanforderungen hinaus alle weiteren relevanten Metadaten zu sammeln und festzuhalten.

Weitere Informationen zu den wichtigsten Feldern finden sich unten unter dem Punkt [Datenmodellierung](https://digi-kunst.github.io/Handreichung/#digi-kunst-datenmodellierung). Die volle Anzahl der im System angelegten Metadaten-Felder wird später an dieser Stelle dokumentiert werden. 

### Vorlagen (in Vorbereitung) 

Demnächst finden sich hier Vorlagen zur Klärung von Fragen zur Rechteinhaberschaft, Miturheber:innen und Rechten Dritter (Fremdmaterial), u.a.:
- Einverständnis- und Übernahmeerklärung
- Rechteklärung
- Hinweise zur Erstellung von Archivrichtlinen an den Partnerhochschulen


### Weiterführende Lektüre

- Nicht alle Dateitypen sind langzeitstabil. Hier findet sich eine [Übersicht von gängigen Dateiformaten und deren Langzeitstabilität](https://www.lzv.nrw/dateiformate/) (lzv.nrw). 
- Schritte zum Sichern digitaler Inhalte: NDSA [Levels of Digital Preservation Matrix](https://osf.io/3na96). Hier finden sie weiterführende Informationen zu den oben erwähnten grundlegenden Schritten.
	

### Digi-Kunst Datenmodellierung 

Dieses [Diagramm](./assets/2023-03-21_Skizze_Datenmodellierung.pdf) zeigt, wie im Digi-Kunst-Archiv die heterogenen Informationen der unterschiedlichen Einliefernden in ein logisches Verhältnis zueinander gebracht und integriert werden, und in welchen Entitäten (Tabellen) und Attributen (Feldern) die einzelnen Metadaten erfasst und verfügbar gemacht werden.

Im Zentrum steht das *Projekt*, meistens ein künstlerisches Werk. Das Projekt muss einen Titel haben, es lässt sich kategorisieren und inhaltlich beschreiben.  

Die mit dem Projekt verbundenen weiteren Informationen, wie z.B. Personen speichern wir in der Entität *Akteure* separat ab. Dadurch müssen wir diese Informationen nur einmal eingeben und später nur noch darauf verweisen. So vermeidet man Redundanzen und minimiert Fehler, z.B. leicht anders geschriebene Namen. 

Eine weitere wichtige Entität sind die *digitalen Objekte* oder Dateien. Diese sind entweder durch Retrodigitalisierung aus physischen Medien entstanden, oder sie sind *born digital*. Weitere Entitäten, teilweise noch in der Planung begriffen, lassen sich aus dem Diagramm ablesen.

Das Digi-Kunst-Archiv ist ereignisbasiert angelegt und kann, wie im [Bericht des Vorprojekts](https://www.dh.nrw/kooperationen/Digi-Kunst.nrw%20%28Vorprojekt%29-63) erwähnt, in Metadatenaustauschformaten wie LIDO und MARC21 abgerufen werden.

---
Diese Handreichung wird kontinuierlich erweitert. Ansprechpartner an den Konsortialhochschulen werden per E-Mail über Updates informiert. [René Bialik](https://www.folkwang-uni.de/home/hochschule/personen/mitarbeiterinnen-a-z/vollanzeige/personen-detail/adm/rene-bialik/) oder [Christian Sievers](https://www.khm.de/personen_hochschule/id.27806.christian-sievers/) freuen sich über Fragen und Anregungen. 

[Digi-Kunst.nrw](https://www.rsh-duesseldorf.de/musikhochschule/wir-ueber-uns/digi-kunstnrw/) | [Impressum](https://www.rsh-duesseldorf.de/service/datenschutz-impressum) | zuletzt aktualisiert: 2023-04-13