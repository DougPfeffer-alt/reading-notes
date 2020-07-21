# Text (HTML - Chapter 2, pp. 40-61)

- HTML has 6 levels of heading `<h1>` through `<h6>`
- `<p>` - Paragraphs 
- `<b>`(bold) and `<i>` (Italic)
- `<sup>` (superscripts) and `<sub>` (subscripts)
- Whitespace: Code is easier to read with white space, but the browser will recognize the gaps, and only display one space.
- `<br />` (line breaks) and `<hr />` (horizontal rules)
- Semantic Markup: Text elements that are not intended to affect the structure of the webpage, but do add extra information.
- `<strong>` (strong) and `<em>` (emphasis)
- `<blockquote>` (longer) and `<q>` (short) quotes.
- `<abbr>` - Abbreviations and acronyms.
- `<cite>` (citations) and `<dfn>` (definitions).
- `<address>` - Author details.
- `<ins>` (insert), `<del>` (delete) and `<s>` (strike through) - Changes to content.

# Introducing CSS (HTML - Chapter 10, pp. 226-245)

- CSS associates style rules with HTML elements. A CSS rule must contain 2 parts: 
  - Selector (what)
  - Declaration (how)
- CSS properties affect hpw elements are displayed 
- External CSS
  - `<link>` - Tells HTML where to find the CSS 
    - href: Path to the file.
    - type: Type of document.
    - rel: relationship.
    example: `<link href="css/styles.css" type="text/css" rel="styleesheet"/>`
  - Internal CSS
    - `<style?` - Should use TYPE attributres (`<style type="text/css">`)
  - CSS Selectors:
    - Universal Selector.
    - Type selector.
    - Class selector.
    - ID Selector.
    - Child Selector.
    - Descendant selector.
    - Adjacent sibling selector.
    - General sibling selector. 
  - CSS Rules Cascade - LAST RULE 
  - If you specify any font-family of color properties, all child elements will be affected.

# Basic JavaScript Instructions (Chapter 2, pp 53-84)

- Variables: Temporarily stored data in variables.
  - Declare variables by giving them a name: "var quantity;"
  - Assign a value: "quantity = 3"
  - Data types: 
    - Numeric
    - String
    - Boolean

- Arrays: A special type of variable that doesn't only store one value, it stores lists of values.
  - And Array literal (preferred): A list of items in square brackets. Can be any var. 
  - The list of iutems starts at "0".
  - You can change val;ues within the list as you go. Last statement counts.
- Expressions: An expression evaluates into (results in) a single value.
  - Expressions that assign a value to a variable.
    - var color = 'beige';
  - Use two or more values to return a single value.
    - var area = 3 * 2;
- Operators: Alloe programmers to create a single value from one or more values.
  - Arithmentic operators: +, -, /, *, ++ (increment), -- (decrement), % (modulus).

# Decisions and Loops (Chapter 4, pp. 145-162)

## Comparison Operators: Evaluating Conditions

- `==` - Is Equal To (Compares two values to see if they are the same)
- `===` - Strict Equal To (Compares two values to see if both the data type and value are the same)
- `!=` - Is Not Equal To (Compares two values to see if they are not the same)
- `!==` - Strict Not Equal To (Compares two values to see if both the data type and value are not the same)
- `>` - Greater Than (This operator checks to see if the number to the left is greater than the number to the right)
- `<` - Less Than (This operator checks to see if the number to the left is less than the number to the right)
- `>=` - Greater Than or Equal To (This operator checks to see if the number to the left is greater or equal than the number to the right)
- `>=` - Less Than or Equal To (This operator checks to see if the number to the left is less or equal than the number to the right)

## Logical Operators

### Comparison operators usually return single values of true or false. Logical operators allow you to compare the resukts of more than one comparison operator 

- Example:

    `((5<2) && (2>=3))

    5<2 is false
    2>=3 is false
    The logical operator `&&` will check to see if either is true, which they are not.

- `&&` - Logical And (This operator tests more than one condition) so `((2<5) && (3>=2))` returns TRUE.
- `||` Logical Or (Thsi operator tests at least one condition) so `((2<5) || (2<1))` also returns TRUE.
- `!` - Logical Not (This operator takes a single Boolean valuye and inverst it) so `!(2<1)` also returns TRUE.

## Loops 

- Loops check a condition, if it returns true, a code block will run. The the condition will be checked again, and if it still returns true, the code block will run again. It repeats until the condition returns false.There are 3 common types of Loops:
    - FOR: If you need to run a code for a specific number of times, use a FOR Loop.
    - WHILE: If you do not know how many times a piece of code should run, you can use a WHILE Loop. As long as the condition is true, the code will continue to run.
    - DO WHILE: Similar to the WHILE Loop, except that it will always run the statements inside the curly braces at least once, even if the condition returns false.

- Example: 

    `for (var i = 0; i < 10; i++) {   
         console.log(i);     
    }`  

    This will be going (0,1,2,3,4,5,6,7,8,9) until i is no longer smaller than 10. Then the counter stops.

        - var i = 0 (Initialization)
        - i < 10; (Condition)
        - i ++ (Update, or keep adding 1 until condition is met). Shorthand meaning i = i+1
        - for (this; many; times;){  
            //do the thing:
        }

### Using While loops

- Commonly used when you do not know exactly how many times you need the code run, so you set it to continue running the code until the condition is met.

- Example

    `while (response !== 'house'){
        var response = prompt("would you like a house or hotel?")
    }`

### Vocabulary

- Loops
- While True: Loop over code
- For: For a certain number of times
- Iterate: Each time it loops 
- Condition: Think of conditional statements ((true && true) || false)
- Increment - Increase (possibly by 1)
- Decrement - Decrease (possibly by 1)

