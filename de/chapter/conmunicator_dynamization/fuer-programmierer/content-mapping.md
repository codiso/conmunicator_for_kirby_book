# Content Mapping

Um diese Funktion zu nutzen, können unter dem Ordner /conmunicator/devices/ Unterordner (desktop,tablet,phone) angelegt werden. In den Ordnern kann dann die entsprechende Textdatei angelegt werden.

```
content_mapping.php
```

Sollte für ein Endgerät keine spezifische Datei vorhanden sein, so wird automatisch auf "desktop" zurückgeschaltet. Sollte auch hier keine Datei vorhanden sein, findet das "Content Mapping" nicht statt.

## Funktionalitäten

Um Inhalte im HTML-Dokument zu verändern, stellt Conmunicator einige Funktionen zur Verfügung.

| Funktion | Bedeutung |
|-|-|
|get_lang()|Die Funktion gibt die aktuell genutzte Sprache zurück (de, en, …).|
|replace_content_by_id($id,$html)|Die Funktion ersetzt den Inhalt eines durch die **id** gekennzeichneten HTML-Elementes.|
|replace_element_by_id($id,$html)|Die Funktion ersetzt das komplette, durch die **id** gekennzeichnete, HTML-Element.|
|replace_content_by_class($class,$html)|Die Funktion ersetzt den Inhalt eines durch die **class** gekennzeichneten HTML-Elementes.|
|replace_element_by_class($id,$html)|Die Funktion ersetzt das komplette, durch die **class** gekennzeichnete, HTML-Element.|