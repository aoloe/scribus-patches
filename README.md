# scribus-patches

A set of patches to make Scribus "usable"

There are a few very sane request that the Scribus has refused to implement and some important patches/request that have been laying around for years without having been applied.

Most of them are rather trivial to implement.

This repository contains a set of patches that implements those features and can be applied to the Scribus source code and produce a better Scribus.

## The existing patches

- Remove the hack that enables the single click on Fedora and breaks all other Linux systems.  
  `file-open-shortcuts.patch`

## Patch that exist but are not complete / enabled by default

- Activate the new Scripter

## Patches that should be created

### User interface

- toolbars
  - by default place the tools toolbar on the left and hide the other toolbars
  - remove rarely used and unstable tools from the tools toolbar:
    - table (unstable)
    - spirals,
    - caligraphy,
    - freehand line (that should not be a tool)
    - barcode,
    - polygon (not 100% sure...)
- by default show the properties palette and dock it to the right side
- by default do not show the multiple actions open / new / template dialog

### Text frames

- remove the "Unlik with copy" and rename "Unlink with cut" as "Item > Text frames > Unlink and cut Text" (or better name)  
  https://bugs.scribus.net/view.php?id=14327
- remove the confirmation dialog when adding a text frame in the middle of a text frames chain:  
  https://bugs.scribus.net/view.php?id=14325
- add a "chain before" entry in the "Item > Text frames" dialog  
  https://bugs.scribus.net/view.php?id=14326
- remove the "Automatic creation of text frames" from the new dialog (eventually put it in the document settings)

### Frames

- unify the shortcut commands for "Fit frame to text" and "Ajust frame to image" into "Fit frame to content" and assigne the `ctrl-=` shortcut.


### Others

- Remove all templates
