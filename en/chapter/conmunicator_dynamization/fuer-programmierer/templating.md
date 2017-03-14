# Templating

Not everytime the mapping of pages using the page name is useful. Especially for more complex sites, this procedure is complicated, because for each Kirby page you need a matching Adobe Muse CC page.

In this case, it makes sense to use a different strategy. In Adobe Muse CC build only the sides, which are needed for the visualization of the site. By specifying "**templateFile**" in the file **default.php** with a direct file name the normal alias mapping is overridden. If a Kirby page uses this template all pages are generated with the specified Adobe Muse CC file.

If you duplicate **default.php** and change the file name in **[somthingelse].php**, the file can be used in other Kirby page as a template.

https://getkirby.com/docs/templates