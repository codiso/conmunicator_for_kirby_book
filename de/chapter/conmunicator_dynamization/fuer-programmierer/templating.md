# Templating

Nicht in jedem Fall ist das Mapping der Seiten über den Seitennamen sinnvoll. Vorallem bei komplexeren Websites wird dieses Vorgehen kompliziert, denn für jede Seite benötigt man eine passende Adobe Muse CC Seite.

In diesem Fall ist es sinnvoll eine andere Strategie zu nutzen. In Adobe Muse CC baut man nur noch die Seiten auf, die man für die Visualisierung der Website benötigt. Über die Angabe "**templateFile**" kann in der Datei **default.php** ein direkter Dateinamen angegeben werden.

Dies füht dazu, dass das normale Alias-Mapping außer Kraft gesetzt wird. Nutzt eine Kirby-Seite dieses Template, so werden alle Contao-Seiten unter Nuzung der angegebenen Adobe Muse CC Datei ausgegeben.

Dupliziert man die Datei **default.php** und ändert den Dateinahmen in **[etwasAnderes].php**, so kann die Datei in weiteren Kirby-Seiten als Template verwendet werden.

https://getkirby.com/docs/templates

