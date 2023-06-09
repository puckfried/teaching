# HTML Basics

HTML steht für Hypertext Markup Language und ist die Grundlage für die Erstellung von Webseiten. HTML besteht aus einer Reihe von Tags und Attributen, die zur Strukturierung von Inhalten verwendet werden. Hier sind die grundlegenden Konzepte von HTML:

## Tags

HTML-Tags sind Elemente, die zur Strukturierung von Inhalten auf einer Webseite verwendet werden. Tags sind in spitzen Klammern geschrieben und können geöffnet und geschlossen werden, um den Inhalt zu umschließen. Hier sind einige grundlegende HTML-Tags:

- `<html>`: Definiert den Anfang des HTML-Dokuments.
- `<head>`: Enthält Metadaten über das Dokument, einschließlich Titel und Stilinformationen.
- `<body>`: Enthält den sichtbaren Inhalt der Webseite.
- `<h1>` bis `<h6>`: Definiert die Überschriften auf der Seite, wobei `<h1>` die höchste und `<h6>` die niedrigste Ebene hat.
- `<p>`: Definiert einen Absatz.
- `<img>`: Definiert ein Bild.
- `<a>`: Definiert einen Link.
- `<ul>`: Definiert eine unsortierte Liste.
- `<ol>`: Definiert eine sortierte/nummerierte Liste.
- `<li>`: Definiert ein einzelnes Listenelement innerhalb einer Liste.

## Attribute

HTML-Attribute werden verwendet, um zusätzliche Informationen zu Tags hinzuzufügen. Attribute werden innerhalb des Starttags des Tags geschrieben und haben einen Namen und einen Wert. Hier sind einige grundlegende HTML-Attribute:

- `class`: Wird verwendet, um ein Tag mit einer Klasse zu kennzeichnen, um es zu formatieren oder mit CSS zu stylen.
- `id`: Wird verwendet, um ein Tag mit einer eindeutigen ID zu kennzeichnen, um es per CSS oder JavaScript zu manipulieren.

#### `<img>` 
- `src`: Wird verwendet, um die Quelle des Bildes für das `<img>`-Tag anzugeben.
- `alt`: Wird verwendet, um den Alternativtext eines Bildes (`<img>`-Tag) zu definieren, für Screenreader und wenn das Bild nicht angezeigt werden kann.
- `width`: Definiert die Breite des Bildes in Pixel
#### `<a>`
- `href`: Wird verwendet, um den Ziel-URL für das `<a>`-Tag anzugeben.
- `target="_blank"`: Wird verwendet, um bei Klicken des Links, ein neues Browser-Tab zu öffnen

## Beispiel

Hier ist ein Beispiel für eine HTML-Seite, die aus einem `<head>`-Bereich und einem `<body>`-Bereich besteht:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Meine Webseite</title>
  </head>
  <body>
    <h1>Willkommen auf meiner Webseite</h1>
    <p>Hier ist ein Absatz mit ein paar Informationen.</p>
    <img src="mein-bild.jpg" alt="Mein Bild" />
    <a href="https://www.meinlink.de">Hier ist ein Link</a>
  </body>
</html>
```

