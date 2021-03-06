---
ID: 21942
post_title: >
  Unwichtige und dekorative Inhalte als
  Artefakt
author: Stefan Brechbühl
post_excerpt: >
  BenutzerInnen von AT sind nicht nur auf
  semantisch korrekte Tags angewiesen. Es
  ist auch wichtig dekorative, nicht
  relevante Objekte von der Ausgabe
  auszuschliessen. Dies wird erreicht
  indem solche unwichtige Elemente als
  Artefakt gekennzeichnet werden.
layout: basics
permalink: >
  https://accessible-pdf.info/de/basics/unwichtige-und-dekorative-inhalte-als-artefakt/
published: true
post_date: 2018-03-28 14:53:24
tags:
  - InDesign
  - Word
categories: [ ]
---
BenutzerInnen von [AT](https://accessible-pdf.info/de/glossar/#assistive-technologie) sind nicht nur auf semantisch korrekte *Tags* angewiesen. Es ist auch wichtig dekorative, nicht relevante Objekte von der Ausgabe auszuschliessen. Dies wird erreicht indem solche unwichtige Elemente als Artefakt gekennzeichnet werden.

Unwichtig sind Informationen, welche für die gedruckte jedoch nicht die digitale Ausgabe nützlich sind. Hierzu zählen beispielsweise:

- Seitennummerierung
- Wiederholende Informationen in Kopf- und Fusszeilen

Weiter unwichtig sind dekorative Objekte, wie zum Beispiel:

- Hintergrundbilder
- Symbolbilder
- diverse Formen von Linien 
	- zur Dekoration
	- zur Trennung von Textspalten 
	- Tabellenlinien 

## Artefakte in Microsoft Word

Mit Boardmitteln können in Word aktuell keine Artefakte definiert werden. Abhilfe bringt hier das Plugin [axesPDF for Word](https://www.axes4.com/axespdf-for-word-ueberblick.html).

Inhalte, die sich in der Kopf- oder Fusszeile befinden, werden jedoch automatisch als Artefakt ausgezeichnet.

## Artefakte in InDesign festlegen

### Text (innerhalb eines Absatzes)

Texte werden mittels Absatzformatoptionen als Artefakt definiert. Das Vorgehen ist gleich wie in [*Tags* in InDesign festlegen](https://accessible-pdf.info/de/basics/pdf-tags-in-indesign-festlegen/) beschrieben.

Texte, welche auf der Musterseite positioniert sind, werden automatisch als Artefakte ausgezeichnet.

### Objekte

Dekorative Objekte können mit „Objekt“ → „Objektexportoptionen“ als Artefakt gekennzeichnet werden. Wechsle dazu im Fenster auf den Tab „PDF mit *Tags*“ und wähle „*Tag* anwenden: Aussertextliches Element“.

Wer das InDesign Plugin [MadeToTag](https://www.axaio.com/doku.php/de:products:madetotag) besitzt, braucht den oberen Schritt nicht zu tun. Alle Objekte, welche ausserhalb eines Artikels sind, werden automatisch als Artefakt markiert.

## Artefakte in Acrobat festlegen

Artefakte können entweder im *Tagbaum* oder mit dem Leserichtung-Werkzeug definiert werden. Welche Elemente als Artefakte markiert wurden, kann im Navigationsfenster „Inhalt“ geprüft werden.

### Navigationsfenster *Tags*

1. Suche dir den dekorativen Inhalt innerhalb der Tags. Am schnellsten bist du wenn du den Inhalt mit dem Auswahlwerkzeug auswählst und in den Optionen des Navigationsfensters *Tags* auf „*Tag* in Auswahl suchen“ klickst.
2. Mache einen Rechtsklick auf den Inhalt (mit dem kleinen Kistensymbol) und wähle „*Tag* in aussertextliches Element ändern“.
3. Der öffnende Dialog erlaubt dir noch die Art des Artefakts zu bestimmen.
4. Falls dieses Artefakt alleine innerhalb eines *Tags* platziert war, sollte das leere Tag noch gelöscht werden.

![Wie wird ein Artefakt mithilfe des Navigationsfensters *Tags* angelegt? Gif-Animation.](https://accessible-pdf.info/wp/wp-content/uploads/acrobat_artifact.gif)

### Leserichtung-Werkzeug

Mit dem Leserichtung-Werkzeug geht es schneller. Im Gegenzug kann man weniger präzise arbeiten und nicht genau sehen wo was passiert.

1. Wähle das Leserichtung-Werkzeug aus. Falls du es nicht in deinen Schnellwerkzeugen hast, findest du es innerhalb der Werkzeuggruppe „Barrierefreiheit“.
2. Nun verändert sich deine Maus und ein Fenster wird geöffnet.
3. Wähle den Bereich aus, den du als Artefakt kennzeichnen möchtest. Dazu kannst in die linke obere Ecke klicken oder die Maus geklickt halten und ein Auswahlfeld aufziehen.
4. Klicke nun im Fenster auf den Knopf „Hintergrund/Artefakt“.

![Wie wird ein Artefakt mithilfe des „Leserichtung-Werkzeugs“ angelegt? Gif-Animation.](https://accessible-pdf.info/wp/wp-content/uploads/acrobat_artifact2.gif)