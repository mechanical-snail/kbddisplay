Summary
====

Draws a picture of an XKB keyboard layout.
----

This program takes a description of an XKB keyboard layout, and outputs a pretty XML keyboard, styled so that it can be viewed in a web browser. The output XML could possibly be used by other programs.

Written because `xkbprint` sucks. In particular, `xkbprint`

* displays its internal character name (e.g. `Cyrillic_softsign`, `rightdoublequotemark`, `U0462`) rather than the actual character (e.g. `ь`, `”`, `Ѣ`)
* ’s output is sometimes upside-down
* outputs in black and white and uses an ugly font
* can only display 2 shift states (!)
* etc.

To configure it, edit the CSS file.

To do @@@@@
====
* Write the actual program that generates the XML.
* Replace the CSS with XSL, for more flexibility?
* Display the Unicode code number in small font underneath the caption (rather than only in the tooltip) so you can see it if you print it out

Caveats
====
* Currently it doesn’t actually work, since browsers don’t implement CSS 3’s `attr()` function.