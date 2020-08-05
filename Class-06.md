# [Understanding the problem domain is the hardest part of programming](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming/)

- Great article explaining how to approach problem domains. The idea is to simplify and build off of it, iike a video game with tutorial levels and so on.

# Object Literals (JS - Chapter 3, pp 100-105)

- Objects group together a set of variable and functions to create a model of something you would recognize from the real world. In an object, variables and functions take on new names.
  - In an object, variables become known as properties.
  - In an object, functions become known as methods.
- Creating an object: Literal notion: Literal notion is the easiest and most popular way to create objects. 
- Accessing an object and dot notation: You access the properties or methods of an object using dot notation. You can also access properties using square brackets. 

# Document Object Model (JS - Chapter 5, pp. 183-242)

## The Document Object Model(DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. 

- The DOM TREE is a model of a web page: As a browser loads a web page, it creates a model of that page. The mofel is called a DOM TREE, and it is sorted in the browser's memory. It consists of four main types of nodes: 
  - The Document Node: The Document Node represents the entire page. 
  - The Element Nodes: HTML elements 
  - Attribute Nodes: Opening tags of HTMLs carry attributes
  - Text Nodes: Text within elements.
- Working with the DOM Tree: Accessing and updating the DOM involves two steps: 
  1. Locate the Node that represents the element that you want to work with. 
  1. Use its text content, child elements and attributes.
    - Step 1: Access the elements (DOM Querries may return one element, or they may return a NodeList, which is a collection of nodes)
      - Select the individual node:
        - getElementById(): Unique attribuites. Allows you to select a single element node by specifying the value of it's ID attribute.
        - querrySelector(): CSS selectors
          - Both can search an entire document and return individual elements.
      - Select multiple elements (nodelists). Two ways to select, by item() and by array syntax:
        - getEllementsByClassName() 
        - getElementsByTagName()
        - querrySelectorAll()
      - Traversing between element nodes:
        - parentNode
        - previousSibling/nextSibling
        - firstChild/lastChild
    - Step 2: Work with those elements
      - Access/update text nodes 
      - Work with HTML content
      - Access or update attribute values

- Catching DOM Querries: Methods that find elements in the DOM tree are called DOM Querries. When you need to work with an element more than once, you should use a variable to store the result of this querry. When people talk about storing elements in variables, they are really storing the locatioon of the elements within the DOM Tree in a variable. The properties and methoids of that element node work on the variable.

- Accessing elements