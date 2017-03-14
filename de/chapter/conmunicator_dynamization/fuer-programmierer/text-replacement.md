# Text replacement

In der Datei **text_replacement.php** können eigene Textersetzungen definiert werden. Hierzu steht eine Funktion zur Verfügung:

```php
replace_text($search,$replace,$regex=false)
```

| Parameter: | Bedeutung: |
| -- | -- |
| $search |Text der gesucht werden soll. Ist **$regex=true**, so wird $search als RegEx interpretiert.|
| $replace |Text der als Ersetzung dienen soll.|
| $regex |Wahl ob die Ersetzung als str_replace (false) oder als preg_replace (true) ausgeführt wird.|