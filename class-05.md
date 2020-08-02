# Images (HTML - Chapter 5, pp. 94 - 125)

- Choosing images for your site:
  - istockphoto.com
  - gettyimages.com
  - veer.com
  - sxc.hu
  - fotolia.com
- When creating a site from scratch, it's best to store pictures in a local file on your machine.
- Adding images
  - Use `<img>` element
    - src tells the where to find the images
    - alt is used for the text describing the pictures
    - title to title it
  - Height and width should be specified 
- Where to place in the code: 
  - Before a paragraph 
  - Inside the start of a paragraph 
  - In the middle of a paragraph 
- 3 Rules for creating images: 
  1. Save images in the right format 
  1. Save images at the right size
  1. Measure images in pixels
- Some tools to edit images:
  - Adobe fireworks 
  - pixelmator
  - PaintShop Pro
  - Paint.net
- Online editors: 
  - photoshop.com
  - pixlr.com
  - splashup.com
  - ipiccy.com
- Figure and Figure Caption
  - The `<figure>` was introduced so that a caption could be added to an image, and appear as one.
    - `<figcaption>` adds the caption

# Color (HTML - Chapter 11, pp 246 - 263)

- Foreground Color - You can specify the color of text inside of an element
  - RGB values
  - HEX Codes
  - Color names
- Background colors - background-color: If CSS treats HTML like boxes, background-color afffects the background of the boxes
- Understanding color:
  - RGB Values: rgb(102.205.170)
  - HEX Codes: `#66cdaa`
  - Color names: red, green, blue
- Opacity to determine how transparent it is.
  - ex: opacity: 0.5;
- HSLA Colors:
  - Hue, saturation and lightness and Alpha (0.5 = 50% transparency).

# Text (HTML - Chapter 12, pp. 264 - 299)

- When choosing a typeface for your site, it's important to understand that a browser will only display what's installed on the user's computer. 
- Specifying typefaces: font-family
- Specifying size of type: font-size
- @font-face will allow you to use a font, even if it's not installed on the computer of the person browsing.
- Bold: font-weight 
- Italic: font-style 
- Upper and lowercase: text-transform
- Underline and strike: text-decoration
- Leading: line-height
- Letter and word spacing: letter-spacing, word-spacing
- Alignment: text-align
- Vertical alignment: vertical-align
- Indent Text: text-indent
- Drop Shadow: text-shadow
- First Letter or Line: :first-letter, `:first-line`
- Styling links: :link, :visited
- Responding to users: `:hover`, :active, `:focus`
- Attribute Selectors: These allow you to create specific rules:
  - existence
  - equality
  - space
  - prefix
  - substring
  - suffix

