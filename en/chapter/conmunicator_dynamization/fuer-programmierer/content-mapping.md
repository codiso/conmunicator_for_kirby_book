# Content Mapping

To use this feature you can create device folders (desktop,tablet,phone) in the folder /conmunicator/devices/. Each device folder can contain a text file, which shall comply with the following notation.

```
content_mapping.php
```

If a device has no specific file, the "desktop" version will be tried to load. If this file does not exist, the "content mapping" does not take place.

## Functionality

To change content in the HTML document, Conmunicator provides several functions.

| Funktion | Bedeutung |
|-|-|
|get_lang()|The function returns the currently used language (de, en, …).|
|replace_content_by_id($id,$html)|The function replaces the content of an HTML element with the used **id**.|
|replace_element_by_id($id,$html)|The function replaces the complete HTML-Element with the used **id**.|
|replace_content_by_class($class,$html)|The function replaces the content of an HTML element with the used **class**.|
|replace_element_by_class($id,$html)|The function replaces the complete HTML-Element with the used **class**.|



