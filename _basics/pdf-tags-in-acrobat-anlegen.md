---
ID: 21938
post_title: '<em>PDF-Tags</em> in Acrobat anlegen'
author: Stefan Brechbühl
post_excerpt: >
  Das vollständige Taggen eines PDFs in
  Acrobat ist nur empfohlen wenn die
  Autorensoftware keinen PDF-Export mit
  Tags (Tagged PDF) erlaubt oder das
  Quelldokument nicht vorhanden ist. Für
  Word und InDesign werden folgende
  Anleitungen empfohlen.
layout: basics
permalink: >
  https://accessible-pdf.info/de/basics/pdf-tags-in-acrobat-anlegen/
published: true
post_date: 2018-09-06 20:16:51
tags: [ ]
categories: [ ]
---
Das vollständige *Taggen* eines PDFs in Acrobat ist nur empfohlen wenn die Autorensoftware keinen PDF-Export mit *Tags* *(Tagged PDF)* erlaubt oder das Quelldokument nicht vorhanden ist. Für Word und InDesign werden folgende Anleitungen empfohlen:

*   [*PDF-Tags* in Word festlegen][1]
*   [*PDF-Tags* in InDesign festlegen][2]

Da die Möglichkeiten, welche Word oder InDesign anbieten, beschränkt sind, ist es häufig nötig die *Tagstruktur* in Acrobat noch anzupassen. In dieser und den folgenden Anleitungen siehst du wie das geht:

*   [*PDF-Tags* in Acrobat ändern][3]
*   [Unwichtige und dekorative Inhalte als Artefakt][4]

Hinweis: Mit dem kostenlosen [Adobe Acrobat Reader][5] können keine Anpassungen der *Tagstruktur* vorgenommen werden. Dafür wird der kostenpflichtige [Adobe Acrobat][6] benötigt.

## Erste Schritte {#ersteSchritte}

Zuerst muss das Dokument als „Tagged PDF“ markiert werden.

1.  Zeige dir hierzu das Navigationsfenster „Tags“ an. 
2.  Wähle „Tag-Stamm erstellen“ unter Optionen (kleines rechteckiges *Icon* mit zwei Listenpunkten).
3.  Der Text „Keine Tags verfügbar“ hat sich in „Tags“ geändert.
4.  Ein erneuter Klick auf das Icon „Optionen“ zeigt neu den Befehl „Dokument ist PDF (mit Tags)„. Klicke diesen an.
5.  In den „Dokumenteigenschaften“ wird nun unter „Beschreibung“ der Eintrag „PDF mit Tags“ → „Ja“ angezeigt.

![Erste Schritte um ein Tagged PDF aus Acrobat zu erstellen. Gif-Animation.][7]

## Semantik

Jetzt kannst du mit dem *Taggen* beginnen. Als oberstes *Tag* wird `<Document>` benötigt.

Eine Übersicht der möglichen Tags, welche innerhalb dieses `<Document>` *Tags* angewendet werden können, findest du in der [„Übersicht der *PDF-Tags*“][8].

Gemäss [Matterhorn Protokoll][9], Fehlerbedingung 01-006, muss immer der semantisch korrekte *Tag* verwendet werden.

## *Tags* automatisch zuweisen {#automatischesTaggen}

In Acrobat können *Tags* automatisch zugewiesen werden. Die Erkennung semantischer Auszeichnungen wurde in Acrobat stets verbessert. Trotzdem wird es einem Computerprogramm nie zu 100 % gelingen, jegliche Gestaltungslogik zu erkennen. **Daher bedingt das automatische *Taggen*, dass zwingend eine manuelle Prüfung und Optimierung des *Tagbaums* gemacht werden muss.** Wie bestehende *Tags* geändert werden, kannst du in [„PDF-Tags in Acrobat ändern“][3] nachlesen.

### Lösungsweg 1

Gleiches Vorgehen wie unter [Erste Schritte][10], nur wird bei Punkt 2 anstatt „Tag-Stamm erstellen“, „Tags zu Dokument hinzufügen“ gewählt.

### Lösungsweg 2

Wähle „Dokument automatisch taggen“ in den Werkzeugen „Barrierefreiheit“.

## Einzelner *Tag* manuell zuweisen {#manuellesTaggen}

Das manuelle Vorgehen wird in der Regel benötigt um einzelne, fehlende *Tags* der bestehenden Struktur hinzufügen.

### Lösungsweg 1

1.  Füge einen neuen *Tag* hinzu indem du im Navigationsfenster „Tags“ die Optionen öffnest (kleines rechteckiges *Icon* mit zwei Listenpunkten) und „Neuer Tag“ auswählst. 
2.  Im angezeigten Fenster kannst du den korrekten *Tag* auswählen und mit „OK“ bestätigen.
3.  Klicke auf den neu erstellten *Tag* und wähle den dafür vorgesehene Text mit dem Auswahlwerkzeug aus.
4.  Öffne nun das Optionen-Menü des Navigationsfensters *Tags* erneut und wähle „Tag aus Auswahl erstellen“.

![Lösungsweg 1 um in Acrobat manuell ein neuer Tag hinzuzufügen. Gif-Animation.][11]

### Lösungsweg 2

1.  Klicke auf das *Root*-Element *Tags* im Navigationsfenster *Tags*.
2.  Wähle den gewünschten Text mit dem Auswahlwerkzeug aus.
3.  Öffne das Optionen-Menü (kleines rechteckiges *Icon* mit zwei Listenpunkten) des Navigationsfensters *Tags* und wähle „Tag aus Auswahl erstellen“
4.  Im angezeigten Fenster kannst du den korrekten *Tag* auswählen und mit „OK“ bestätigen.

![Lösungsweg 2 um in Acrobat manuell ein neuer Tag hinzuzufügen. Gif-Animation.][12]

### Lösungsweg 3

Eine weitere Möglichkeit ist die Verwendung des „Leserichtung“-Werkzeugs. Die Handhabung dieses Werkzeugs ist etwas gewöhnungsbedürftig und es stehen nicht alle möglichen *Tags* zur Verfügung.

1.  Klicke auf „Leserichtung“ innerhalb der „Barrierefreiheit“-Werkzeuge.
2.  Es öffnet sich ein neues Fenster und der *Cursor* ändert sich in ein Kreuz.
3.  Wähle damit den Inhalt aus, welcher *getaggt* werden muss. 
4.  Im Fenster „Leserichtung“ kann nun der entsprechende *Tag* ausgewählt werden.

![Lösungsweg 3 um in Acrobat manuell ein neuer Tag hinzuzufügen. Gif-Animation.][13]

 [1]: https://accessible-pdf.info/de/basics/pdf-tags-in-word-festlegen/
 [2]: https://accessible-pdf.info/de/basics/pdf-tags-in-indesign-festlegen/
 [3]: https://accessible-pdf.info/de/basics/pdf-tags-in-acrobat-aendern/
 [4]: https://accessible-pdf.info/de/basics/unwichtige-und-dekorative-inhalte-als-artefakt/
 [5]: https://get.adobe.com/de/reader/
 [6]: https://acrobat.adobe.com/ch/de/acrobat.html
 [7]: https://accessible-pdf.info/wp/wp-content/uploads/acrobat_taggen_erste_schritte.gif
 [8]: https://accessible-pdf.info/de/basics/uebersicht-der-pdf-tags/
 [9]: https://accessible-pdf.info/de/glossar/#matterhorn-protokoll
 [10]: #ersteSchritte
 [11]: https://accessible-pdf.info/wp/wp-content/uploads/acrobat_manuelles_taggen1.gif
 [12]: https://accessible-pdf.info/wp/wp-content/uploads/acrobat_manuelles_taggen2.gif
 [13]: https://accessible-pdf.info/wp/wp-content/uploads/acrobat_manuelles_taggen3.gif