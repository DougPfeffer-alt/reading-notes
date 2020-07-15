# Operators and Loops

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
        - for (this; many; times;){//do the thing:
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

