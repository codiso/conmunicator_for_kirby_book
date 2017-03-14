# For Programmers
Looking at the side of design from the perspective of an Adobe-MUSE project, styles are the easiest and most straightforward way to connect dynamic content from the CMS to the static layout.

For complicated requirements, styles ar not enough to reach your target. You will need more control over the allocation of dynamic content to DOM elements of the HTML document.

With Conmunicator you have several ways to control the assignment or integrate own code.

| Mode: | File: | Importance: |
| -- | -- | -- |
| Content-Mapping |content_mapping.php| Content from Contao can be used by define CSS selectors.|
| File-Mapping |file_mapping.php| Adobe-MUSE pages can be matched by using the page alias from Contao.|
| Text replacement |text_replacement.php| Define own text replacements.|

## Adaptive Layout
With Adobe-MUSE a layout can be constructed adaptively. Three independent sites are created by Adobe-MUSE. These are organized into seperated folders.

| Device: | Importance: |
| -- | -- |
| Desktop | Site for a destktop computer ore laptop. It is placed in the root of the export folder.|
| Tablet |  Site for an tablet computer placed into an subfolder named **/tablet**.|
| Phone |  Site for an mobile phóne placed into an subfolder named **/phone**.|

For control of the different versions <.COMMUNICATOR> has three folders for the every exported site.

* /devices/desktop
* /devices/tablet
* /devices/phone

Each of these folders contain files for controlling the above-mentioned types.

## Responsive Layout
In the current version of Adobe-MUSE layouts can be complete responsive. With CSS media queries the look and feel of an site is set up visually for different devices.

In this case you can only use the folder **/desktop**.