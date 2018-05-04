---
post_title: No <code>Figure</code> tag in compatibility mode
author: Stefan Brechbühl
layout: tutorials
published: false
tags:
  - manual testing
  - Microsoft Word
categories:
  - 13. Graphics
---
## Issue

An image is placed with the “In Line with Text” layout option into Word in “Compatibility Mode” (<code>.doc</code> file). After exporting as PDF the image won't be within a `<Figure>` tag as expected, but within an `<InlineShape>`, to which the role `<Sect>` is assigned.

Issue detected in PDF made from:

*   Microsoft Word 2013 for Windows (in Compatibility Mode)

### PAC 2 warning

> Possibly inappropriate use of a Sect structure element

### Failure Conditions of the Matterhorn Protocol

> **13-001** Graphics objects other than text objects and artifacts are not tagged with a Figure tag. (→ [manual testing][1])

## Manual approach in Acrobat

1. The “Reading order” tool can be used to select the image and convert it to a figure.
2. `<InlineShape>` is going to be converted to `<Figure>`. 
3. The alternative text is copied automatically.

## Automatic approach in Word 2013

Since the problem only exists in compatibility mode (<code>.doc</code> files), the document can be converted to the newer <code>.docx</code> file format. The “Convert” command is located in the menu “File” → “Info”.

Attention: The conversion can cause (minor) layout changes!

 [1]: https://accessible-pdf.info/en/glossary/#manual-testing