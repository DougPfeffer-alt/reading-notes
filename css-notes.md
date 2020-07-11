# CSS notes

- CSS - Cascading Style Sheets 
- RGB - Red Green Blue - `  background-color: rgb(214, 233, 176);`
- HEX Codes.
- Opacity (transparancy)
- HSL Hue Saturation Light

## The How 

- CSS associates style withe the HTML element, as if it appears inside of its own box (ex: what kind of font associared with a paragraph, or the color of a heading)
- CSS can be applied internally through HTML, or externally through CSS.
- Rules are made up of selectors (specify the elements the rules apply to), and declerations (what elements should lok like).
- Different selectors target different elements.
- Declerations have two parts - the property of the element to change, and the value of the property (example: font-family property sets the choice of font, and the value of arial sets the preferred typeface)
- CSS Rules cascade. Whatever the last rule is, it will trump all previous rules.
- What you apply a particular rule to a body element, it will then apply to all child elements.
- 3 ways to express color (RGB, Hex, color names).
- The A of RGBA notes opacity.

## External versus Internal style

### External Style

- 1 Style sheet can be applied to several web pages.
- The HTML code will be mush easier to read, because it won't be clogged up by a bunch of CSS style.

### Internal Style

- Best if onkly working with 1 web page.
- Best if you have 1 webpage that you want to afect, but not the whole site.
