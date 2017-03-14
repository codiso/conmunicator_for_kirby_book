# File Mapping

Im Normalfall werden Seiten, aus dem Contao-CMS, über den Seitenalias mit der entsprechenden Seite, aus dem Adobe Muse CC Projekt, verbunden.

In der Datei '**file_mapping.php**' kann durch die Angabe des Seitenalias eine Seite, aus dem Contao-CMS, auf eine andere Datei, des Adobe Muse CC Projektes, verweisen.

```php
file_mapping("alias","fname");
```

Für **fname** tragen Sie den Dateinamen der Adobe Muse CC Datei ohne die Endung ".html" ein.

| Alias: | Bedeutung: |
| -- | -- |
| * |Alle Seiten werden mit der zugewiesenen Datei verknüpft.|
| alias |Eine Seite mit dem Seitenalias wird mit der zugewiesenen Datei verknüpft. Diese Angabe dominiert die Wildcard-Verknüpfung.|