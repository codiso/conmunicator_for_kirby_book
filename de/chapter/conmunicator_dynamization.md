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
| \{\{cmu\_content\_[NAME]\}\} | Inhalt eines Feldes aus Kirby. |


| Platzhalter: | Ersetzung: |
| --- | --- |
| NAME | Name des Elements aus Kirby. |

## Snippets
Snippets bieten die Möglichkeit dynamische Code-Elemente in einen Seite einfließen zu lassen. Diese sind im Ordner "**/site/snippets/**" abgelegt. Eine genaue Beschreibung findet man in der [Dokumentation](https://getkirby.com/docs/templates/snippets) von Kirby.

Durch die Definition eines Stils kann ein Snippet mit einem Adobe Muse CC Element verknüpft werden.

| Stil: | Bedeutung: |
| --- | --- |
  | cmu\_snippet\_[NAME] | Inhalt eines Snippets aus Kirby. |

| Insert-TAG: | Bedeutung: |
| --- | --- |
  | \{\{cmu\_content\_[NAME]\}\} | Inhalt eines Snippets aus Kirby. |

| Platzhalter: | Ersetzung: |
| --- | --- |
| NAME | Name des Elements aus Kirby. |

Zusätzlich werden diese folgend benamte Snippets automatisch in den HTML-Code integriert, sofern sie existieren:

| Snippet: | Bedeutung: |
| --- | --- |
| cmu_head.php | Der Inhalt des Snippets wird am Ende des <head> Tag eingesetzt. |
| cmu_body.php | Der Inhalt des Snippets wird am Ende des <body> Tag eingesetzt. |

## Templates
Durch Templates wird es möglich bestehenden HTML-Code aus dem Adobe Muse CC Design zu extrahieren.

Entsprechende Elemente mit einem Template-Stil, werden in eigenen Dateien abgelegt und stehen so als dynamische Grundlage zur Verfügung. Der Speicherort befindet sich unter **"/conmunicator/templates/[DEVICE]"**. 

Templates werden für adaptive Layouts, in den passenden Ordnern für das genutzte Device abgelegt!

| Stil: | Bedeutung: |
| --- | --- |
| cmu_template_NAME | Inhalt eines eigenen Code-Templates unter Nutzung der Benamung.|

| Platzhalter: | Ersetzung: |
| --- | --- |
| NAME | Name des zu erzeugenden Templates. |


