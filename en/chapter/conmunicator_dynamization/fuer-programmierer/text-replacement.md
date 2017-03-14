# Text replacement

In the file **text_replacement.php** own text replacements can be defined.

```php
replace_text($search,$replace,$regex=false)
```

| Parameter | Description |
| -- | -- |
| $search |Text to be searched. Is **$regex=true**, so $search is interpreted as RegEx.|
| $replace |Text to serve as a replacement.|
| $regex |Choice if the replacement is executed as str_replace (false) or preg_replace (true).|