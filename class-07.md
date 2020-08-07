# [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

## Summary

Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

Here's some tips to follow when building your own domain models.

- When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
- Model its attributes with a constructor function that defines and initializes properties.
- Model its behaviors with small methods that focus on doing one job well.
- Create instances using the new keyword followed by a call to a constructor function.
- Store the newly created object in a variable so you can access its properties and methods from outside.
- Use the this variable within methods so you can access the object's properties and methods from inside.

# Tables (HTML - Chapter 6, pp. 126 - 145)

Definition of a table: A table represents information in a grid format, like financial reports, TV schedules and sports results.

- Basic Table Structure:
  - `<table>` - The table element is used to create a table.
  - `<tr>` indicates the start of each row.
  - `<td>` represents each cell.
- Table heading (names of columns) are represented by `<th>`.
- The colspan attribute can be used on a `<th>` and `<td>` element to indicate how many columns the cell should run across.
  - ex: `<td colspan="2">Geography</td>` will have Geography span 2 columns.
- The rowspan can be used to span across several rows in the same fashion.
- Long Tables

  - `<thead>` is used for the table headings.
  - The body should sit inside the `<body>` element.
  - The footer should sit inside the `<tfoot> element.

  Summary

  - The `<table>` element is used to add tables to a webpage.
  - A table is drawn out row by row. Each row is created with the `<tr>` element.
  - Inside each row, there are a number of cells, represented by the `<td>` element (or the `<th>` element if it is a header).
  - You can make cells of a table span more than one row or columns using the rowspan or colspan attributes.
  - For long tables, you can split the table in a `<thead>` and `<tbody>` and `<tfoot>`,

# Functions, Methods and Objects (JS, Chapter 3, pp. 106-144)

- Creating an object: Constructor Notation: The NEW keyword and the object constructor create a blank object. You can then add properties and methods to the object.

  - First, you create a new object, using a combination of the NEW keyword, and the object() constructor function.
  - Next, having created the blank object, you can add properties and methods to it. Maje sure statement end with a semi-colon.

  example:

  var hotel = new object();

  hotel.name = 'Quay';
  hotel.rooms = 40;
  hotel.booked = 25;

  hotel.checkAvailability = function() {return this.rooms - this.booked;};

- Obtating an object: To update the value of properties, use dot notationor square brackets. They work on objects created using literal or constructor notation. To delete a property, use the DELETE keyword.

- Creating many objects: Constructor Notation

  - Sometimes you will want several objects to represent similar things. Object constructirs can use a function as a TEMPLATE for creatig objects. First, create the template with the objects properties and methods.
  - You create instances of the object using the constructor function. The NEW keyword followed by the call to the function creates a new object. The properties of each object are given as arguments to the function. The

- Creating objects using constructor syntax - p. 110
- Create and access objects constructir notation - p. 111
- Adding and removing properties - p. 112

- This (It is a keyword): The keyword THIS is commonly used inside functions and objects. Where the function is declared alters what THIS means. It always refers to one object, usually the object in which the function operates.
- A function in Global Scope:
  - When a function is created at the top level of a script (not inside another object or function), then it is in the GLOBAL SCOPE or GLOBAL CONTEXT.
- Global Variables:
  - All global variable also become properties of the WINDOW object, so when a function is in the global context, you can access global variable using the WINDOW object, as well as its other properties.
- A method of an object:
  - When a function is defined inside of an object, it becomes a method. In a method, this refers to the containing object.
- Function expression as a Method:

  - Ifa named function has been defined in global scope, and it is then used as a method of an object, THIS refers to the objects that it is contained within.

- RECAP: Storing Data

  - In JavaScript, data is represented using name/value pairs. To organize your data, you can use an array or object to group a set of related values. In arrays and objects, the name is also know as a key.
    - Variables: A variable has just one key (the variable name) and one value.
    - Arrays: Arrays can store multiple pieces of information. Each piece of information is seperated by a comma. The order of the values is importantbecause items in an array are assigned a number.
  - If you want to access items via a propery name or jey, use an object. If the order is important, use an array.
    - Individual objects: Objects store sets of name/value pairs. If the order is important, use an array.
    - Multiple objects: When you need to create multiple objects within the same page, use an object constructor to provide a template for the objects.

- Arrays are objects. They hold a related set of key/value pairs (like all objects),but the key for each value is its index number.

- Arrays of objects and objects in arrays: You can combine arrays and objects to create complex data structures. Arrays can store a series of objects (and remember their order). Objects can also hold arrays (as values of their properties).

- What are built-in objects: Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in the window. These built-in objects act like a toolkit for creating interactive web pages.

  - 3 groups of built-in objects:

    - Browser Object Model (creates a odel of the browser tab or window). WIndow Object Properties on p.124.
    - Document Object Model (the DOM ctreates a model of the current page).Properties of the DOM on p.126
    - Global JavaScript Objects (a group of individual objects that rerlate to different parts of the JavaScript language). Global object properties on p. 128

  - Data types revisited:
    - Simple Types:
      - String
      - Number
      - Boolean
      - Undefined
      - Null
    - Complex Type:
      - Object

- Global Object: Number Objects: Whenever you have a value that is a number, you can use the methods and properties of the number object on it.

- Global Objects: Math Object: The Math Object has properties and methods got mathematical constants and functions.

- Creating an instance of the date object: In order to work with dtaes, you create an instance of the date object. You can then specify the timeand date that you want to represent.
  - Methods to set and retrieve the time and date on p. 137.

Summary

- Functions allow you to group a set of related statement together that represent a single task.
- Functions can take parameters (info to do their job) and may return a value.
- An object is a series of variables and functions that represent something from the world around you.
- In an object, variables are known as properties of the object; functions are known as methods of the object.
- Web browsers implement objects that represent both the browser window and the document loaded into the browser.
- JavaScript also has several built-in objects such as String, Number, Math and Date. Their properties and methods offer functionality that help you write scripts.
- Arrays and objects can be used to create compex data sets, and both can contain the other.
