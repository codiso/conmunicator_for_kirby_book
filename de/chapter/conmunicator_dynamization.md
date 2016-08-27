# Dynamisierung

## Inhalte
Inhalte werden in Kirby über Dateien, im Ordner "**content**", definiert. Diese befinden sich in den Seiten-Ordnern und tragen deren Namen. Welche genauen Möglichkeiten der Definition von Inhalten zur Verfügung stehen, kann man aus der [Dokumentation](https://getkirby.com/docs/content) von Kirby entnehmen.

Hier ein typisches Beispiel:
```
Title: About
----
Text: Lorem ipsum dolor sit amet,
consectetuer adipiscing elit.
Aenean commodo ligula eget dolor.
```
In dieser Textdatei sind zwei Felder definiert, die als Inhalte genutzt werden können.

Damit entsprechende Feldinhalte mit Adobe Muse CC Elementen korrespondieren, muss ein Stil an dem betroffenen Adobe Muse CC Element definiert werden. In der Regel ist ein Grafikstil unter Adobe Muse CC der richtige Ansatzpunkt.

| Stil: | Bedeutung: |
| --- | --- |
  | cmu\_content\_[NAME] | Inhalt eines Feldes aus Kirby. |
  
| Insert-TAG: | Bedeutung: |
| --- | --- |
  | {{cmu\_section\_[NAME]}} | Inhalt eines Feldes aus Kirby. |
  

| Platzhalter: | Ersetzung: |
| --- | --- |
| NAME | Name des Inhaltsfeldes aus Kirby. |

## Snippets
Snippets bieten die Möglichkeit Code-Elemente in einen Seite einfließen zu lassen. Diese sind im Ordner "**/site/snippets/**" abgelegt.

Durch die Definition eines Stils kann ein Snippet mit einem Adobe Muse CC Element verknüpft werden.

| Stil: | Bedeutung: |
| --- | --- |
  | cmu\_snippet\_[NAME] | Inhalt eines Feldes aus Kirby. |

| Platzhalter: | Ersetzung: |
| --- | --- |
| NAME | Name des Inhaltsfeldes aus Kirby. |