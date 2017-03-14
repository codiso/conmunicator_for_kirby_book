# File Mapping

Normally the mapping of Contao-pages to the corresponding MUSE-pages is done by the page alias.

In the '**file_mapping.php**' file you can specify the page alias corresponding to an Adobe Muse CC page.

```php
file_mapping("alias","fname");

```
For **fname** enter the filename of the Adobe Muse CC file without the suffix ".html".

| Alias: | Importance: |
| -- | -- |
| * |All pages are mapped to the defined Adobe-MUSE page.|
| alias |A single Contao page with the given alias is mapped to the defined Adobe Muse CC page.|