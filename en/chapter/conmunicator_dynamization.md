# Dynamization

## Content
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
| cmu\_page\_[NAME] | Inhalt eines Feldes aus dem $page Kontext. |
| cmu\_site\_[NAME] | Inhalt eines Feldes aus dem $site Kontext. |
  
| Insert-TAG: | Bedeutung: |
| --- | --- |
| \{\{cmu\_page\_[NAME]\}\} | Inhalt eines Feldes aus dem $page Kontext. |
| \{\{cmu\_site\_[NAME]\}\} | Inhalt eines Feldes aus dem $site Kontext. |

| Platzhalter: | Ersetzung: |
| --- | --- |
| NAME | Name des Elements aus Kirby. |

## Snippets
Snippets bieten die Möglichkeit dynamische Code-Elemente in einen Seite einfließen zu lassen. Diese sind im Ordner "**/site/snippets/**" abgelegt. Eine genaue Beschreibung findet man in der [Dokumentation](https://getkirby.com/docs/templates/snippets) von Kirby.

Durch die Definition eines Stils kann ein Snippet mit einem Adobe Muse CC Element verknüpft werden.

| Style: | Bedeutung: |
| --- | --- |
  | cmu\_snippet\_[NAME] | Inhalt eines Snippets aus Kirby. |

| Insert-TAG: | Bedeutung: |
| --- | --- |
  | \{\{cmu\_content\_[NAME]\}\} | Inhalt eines Snippets aus Kirby. |

| Placeholder: | Ersetzung: |
| --- | --- |
| NAME | Name des Snippets aus Kirby. |

## Templates
Through templates, it is possible to extract existing HTML code from the Adobe Muse CC design.

Corresponding elements with a template style are stored in their own files and are thus available as a dynamic basis. They are located at **"/conmunicator/templates/[DEVICE]"**.

Templates are stored for adaptive layouts, in the appropriate folders for the used device!

| Style: | Bedeutung: |
| --- | --- |
| cmu_template_NAME | Content of a separate code template using the desired name.|

| Placeholder: | Ersetzung: |
| --- | --- |
| NAME | Name of the template. |