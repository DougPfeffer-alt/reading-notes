# Links (HTML - Chapter 4, pp.74-93)

- Writing Links: Links are created using the `<a>` elemment. Users can click on anything between the opening and closing tag. You specify which page you want to link to using the "href" attribute.
  - Linking tp other pages on the same site: You can use a shorthand called a relative URL. But all pages must be within the same folder.
- Directory Structure:
  - Structure: The top level folder is know as the root folder. Everything builds off of that.
  - Relationships: Like a family tree
  - Homepages: Teh main homepage to a website written in HTML.
- Relative URLs: Can be used when linking pages within your own website.
- For email links, use "mailto:"
- target: Open links ina new window.
- Use id elements to link to a specifi point on the same webpage, or another page on the site.

# [Layout](http://htmlandcssbook.com/code-samples/chapter-15/) (HTML - Chapter 15, pp. 358-404)

- Key concepts in positining elements: 
  - Building Blocks (In CSS, boxes will either be inline or block'level)
  - Containing blocks (One block elemenst sitting inside another. Known as containing or parent element)
  - Controlling the position of elements. 
    - Normal Flow.
    - Relative Positioning.
    - Absolute Positioning.
    - Fixed Positioning.
    - Floating elements.
- Screen Sizes: Different visitors will have different size screens. You will need to design pages that will work on a variety of screens.
- Screen resolution: You'll need to account for this too.
- Page Sizes: Because screen sizes and displays vary so much, most web designers create pages around 960-1000 pixels.
- Fixed Width Layouts: These do not change as the user increases or decreases the size of their browser window.
  - The width of the main bozes will be spelled out in pixels.
- Liquid Layouts: These stratch and contract as the user increases or decreases the size of their screen.
  - We use percentages to specify the width. 
Layout Grids: Many wed designers use grid structure to position items on the page. 
- CSS Frameworks make life easier by providing the code for common tasks, such as creating:
  - Layout Grids 
  - Styling Forms
  - Printer-friendly versions of pages
  - And more....
- Use "@import" or "link" for multiple style sheets

# Functions, Methods, and Objects (JS - Chapter 3, pp. 86-99)

- What is a function: A grouping of statements that together, will perform a specific task.
- Declaring a function: Give it a name, and thenin curly braces, you note what you want it to do when called.
  `function sayHello(){ document.write('Hello!'); }`
- Calling a function: Once declared, you can execute it with one line of code.
  `sayHello();`
- Declaring the functions that need information: Sometimes a function needs information to perform a task. If this is necessary, when you declare a function, you'll need to give it parameters.
  `function geArea(width, height){ return width * height; }`
  - Calling functions that need information: When you call a function that has parameters, you specify the values that it should use in the parantheses that folow its name. The values are called arguments.
    - Arguments as values: `getArea(3, 5);`
    - Arguments as variables: `wallWidth = 3; wallHeight = 5; getArea(wallWidth, wallHeight);`
- Getting a single value our of a function: Soem functions perform a calculation and return a single value.
- Getting multiple values out of a function: Functions can return more than one value, using an array.
- Anonymous functions and function expressions: Expressions produce a value. If the browser expects to see an expression (like an argument to a function), then it will get treated as an expression.
  - Function decleration: Creates a function that you can call later in the code.
  - Function Expression: If it expects to see an expression, then it will treat it as one.
Immediately invoked Function Expressions (IIFE):
  - Pronounced IFFY, these functions are not given a name, they are executed when the intepreter comes across them.
  - When to use anonymous functions: 
    - As an argument when a function is called
    - To assign the value of a property to an object
    - In event handlers and listeners
    - To prevent conflicts between two Scripts
  - Variable scope:
    - Local variables: Whan a variable is created inside a functio using the `var` keyword, it can only be used in that function. It is claaed a local variable.
    - Global variables: A variable created outside of a function, able to be used anywhere within the script, it is called a Global Variable
  - How memory and variables work: Global variables use more memory, because the browser must remember them the whole time that the oage is open. Local variable are only remembered when the function is executed. 

  # 6 Reasons for Pair Programming

- How does it work: 
  - The Driver: The programmer who is typing, and the only one whose hands are on the keyboard.
  - The Navigator: Uses their words to guide the driver, but does not provide any direct input into the computer.
  - Why: Pair programming touches on all four skills needed to learn a new language:
    - Listening 
    - Speaking
    - Reading
    - Writing
  - Benefits:
    - Greater efficiency
    - Engaged collaboration
    - Learning from fellow students
    - Social skills
    - Job interview readiness 
    - Work environment readiness