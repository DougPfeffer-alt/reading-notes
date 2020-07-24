# Lists (HTML - Chapter 3, pp. 62-73)

- Ordered lists
  - `<ol>` The ordered list is created with the `<ol>` element
  - Each itme in the list is placed between an opening `<li>` and a closing `</li>`.

- Unordered lists
  - The unordered list is created with the `<ul>` element.
  - Each itme in the list is placed between an opening `<li>` and a closing `</li>`.

- DefinitionLists
  - The Definition List is created using the `<dl>` element. Inside, you will see a series of terms (`<dt>`) and their definitions (`<dd>`).

- Nested lists
  - You can nest a secong list inside an `<li>` element. 

# Boxes (Chapter 13, pp. 300-329)

- Box Dimensions
  - By default, a bos is just big enough to hold what's inside the box
  - You can specify the size by:
    - Pixels
    - Percentages
    - ems
- Limiting width and height may be very helpful, so that the site is readable on all devices.
- Overflowing content
  - hidden: Hides extra content not in the box.
  - scroll: Creates a scroll bar.
- Every box has 3 available properties that can be adjusted to control its appearance"
  - Border.
    - The border-width property controls the width of the border. It can be given in pixels, or using the following:
      - thin 
      - medium 
      - thick 
    - Border style can take the following values: 
      - solid 
      - dotted 
      - dashed 
      - double
      - groove
      - ridge
      - Inset
      - outset
      - hidden/none
    - Border color
      - You can individually control all borders for color (top, bottom, left and right)
  - Margin.
  - You can individually control gaps for all margins (top, bottom, left and right)
  - Padding.
  - You can individually control all sides for padding (top, bottom, left and right)
- Padding and margin properties are helpful to control white space and vertical margin.
- You can center a box on a page, or center it inside an element, by setting the left-margin and the right-margin to auto.
- The display property allows you to turn an inline element into a block-level element, or vice verse. The values this property can take are:
  - inline
  - block 
  - inline-block
  - none
- Hiding boxes
  - Using the hidden value means that you can have a box on a page, which will take up the space, but it will be invisable.
- CSS3: 
  - Border-image: Takes an image and slices it into 9 pieces to make the background
  - Box-shadow: Creates a 3d effect 
  - border-radius: creates rounded corners as we;; as elliptical shapes

  # Decisions and Loop (Chapter 4, pp. 162-182)

  - if...else statements: Checks the condition. If it resolves true, the first code block is executed. If the condition resolves false, the second code block is executed instead.
  - Switch statements: Starts with a variable called the switch value. Each case indicates a possible value for this variable, and which code should run if the variable matches that value. (p. 164)
  - Loops: if it returns true, the code runs. If it returns true again, the code runs again...until it returns false.
  - Loop counter: Runs for a certain number of times.
  - 3 Types of loop:
    - FOR: For a specific number of times.
    - WHILE: It will run while the condition is met.
    - DO WHILE: Will run the statement at least once, even if the condition evaluates to false.
