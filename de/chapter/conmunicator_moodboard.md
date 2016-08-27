# Moodboard

Durch die Anlage einer Adobe Muse CC Seite, mit dem Titel "**cmu_moodboard**", kann eine automatische Konvertierung von Stilen erfolgen. Das Ziel ist, die in Adobe Muse CC definierten Stile in einen andern Kontext zu überführen.

In der Regel wird durch ein CMS, bei der Dynamisierung, ein differenter HTML-Code generiert. Dieser stimmt nicht mit dem HTML-Code von Adobe Muse CC überein. Aus diesem Grund werden Stile aus Adobe Muse CC nicht automatisch auf die Ausgabe vom CMS passen. Diesen Schritt soll das Moodboard erleichtern.

## Beispiel
In Adobe Muse CC ist ein Absatzstil für eine Hauptüberschrift angelegt. Diese soll in den Kontext eines Inhalselementes von Contao gebracht werden.


|Stilbenamung in Adobe Muse CC|Element-Selektor in Contao|
|-|-|
|h1|.ce_text h1|

Um dies in Adobe Muse CC zu definieren kann folgender Text in ein Textrahmen eingegeben werden:

```
{{css :: h1 | .ce_text h1}}
```
Besitzt der Text im Textrahmen schon den gewünschten Stil "**h1**", so ist alternativ folgende Schreibweise möglich. Das Schlüsselwort "**self**" verweist auf den verwendeten Stil "**h1**".

```
{{css :: self | .ce_text h1}}
```

Bei einem Export aus Adobe Muse CC werden automatisch alle Stile, aus der Moodboard-Seite, in ein eigenes CSS überführt und in die Contao-Seite eingesetzt.