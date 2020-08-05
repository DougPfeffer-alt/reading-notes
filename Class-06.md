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

- Repeating actions for an entire NodeList: Whe you have a NodeList, you can loop through each node in the collection and apply the same statements to each. 

- Looping throigh a NodeList: If you want to apply the same code throigh numerous elements, looping throigh a NodeList is a powerful technique. 

- Traversing the DOM: When you have an element node, you can select another element in relation to it using these five properties. This is know as traversing the DOM: 
  1. parentNode
  1. previousSibling
  1. nextSibling
  1. firstChild
  1. lastChild

- Whitespace Nodes: Traversing the DOM can be difficult because some browsers add a text mode whenever they come across whitespace between elements. 

- How to get/update element content:
  - Access and update a text node with nodevalue: When you select a text node, you can retrieve or amend the content of it using the nodeValue property. 
  - Accessing and changing a text node: To work with text in an element, first the element node is accessed and then it's text node.
  - Access and update text with textcontent (& innertext): the textContent property allows you to collect or update just the text that is in the containing element (and it's children). 
  - Accessing text only: In order to demonstrate the difference between textContent and innerText, see example on p 217.
  - Adding or removing HTML content: There are two very different approaches to adding and removing content from a DOM tree:
    1. The innerHTML property
      - Approach: Content is provided as a string. It can contain markup for it's descending elements.
      - Adding content: 
        - Store new content as a string in a variable. 
        - Select the element whose content you want to replace
        - Set the contents innerHTML property to be the new string. 
      - Removing content: Set the innerHTML to an empty string.
    1. DOM Manipulation: Targets individual nodes in the DOM tree, whereas innerHTML is better suited to updating entie fragments.
      - Approach: DOM Manipulation refers to a set of DOM methods that allow you to create element and text nodes, and then attach them to the DOM tree or remove them from the DOM tree.
      - Adding content: Use a DOM method to create new content, one node at a time and store it as a variable.
      - Removing content: Remove from the DOM tree using a single element

  - Access anf update text and markup with innerHtml: Using the innerHTML property, you can access and amend the contents of an element, including any child elements.

  - Update text and markup: Example on p 221.

  - Adding elements using DOM manipulation: 
    1. Create the element: createElement()
    1. Give it content: createTextNode()
    1. Add it to the DOM: appendChild()

  - Adding an element to the DOM Tree: Use createElement to add an element to the DOM treet.

  - Removing elements using DOM manipulation (p. 225):
    1. Store the element to be removed in a variable.
    1. Stroe the parent of that element in a variable
    1. Remove the element from it's containing element.

  - Comparing techniques: Updating HTML content.
    - document.write(): 
      - Advantages:
        - Quick and easy for beginners
      - Disadvantages:
        - Only works when page initially loads.
        If you use it after the page loads, it can:
          - Overwrite the whole page 
          - Not add the content to the page
          - Create a new page 
        - Can cause problems with strict XHTML
        - Rarely used by programmers.
    - element, innerHTML:
      - Advantages:
        - You can use it to add a lot of new markup using less code than DOM manipulation methods.
        - Faster than DOM manipulation when adding a lot of new elements.
        - It is a simple way to remove all of the contant from one element (assign it a blank string)
      - Disadvantages:
        - Do not add content from a user, could cause a security risk.
        - Difficult to isolate single elements.
        - Event handlers may no longer work.
    - DOM manipulation:
      - Advantages:
        - Good for changing one element when there are many siblings.
        - Does not affect event handlers
        - Easily allows a script to add elements.
      - Disadvantages: 
        - Slower than innerHTML for a lot of changes.
        - More code needs to be written.

    - Cross-site scripting (XSS) attacks: If you add HTML to a page using innerHTML, you need to be aware of Cross-site scripting attacks or XSS; otherwise an attacker could gain access to your users accounts. To defend against it:
      1.Only let visitirs input the kind of characters they need to when supplying information (validation)
      1. Double check information on a server before displaying it in a database.
      1. The database may safely contain markup and script from a trusted source.

    - XSS: Validation and templates: Make sure that your users can only inpuit characters that they need to use, and limit where this content will be shown on the page.

    - XSS: Escaping and controling markup: Any content generated by users that contain characters used in code should be escaped on the server. You must control any markup added to the page.

    - Attribute nodes: Once you have an element node, you can use other properties and methods on that element node to access and change its attributes.

    - Check for an attribite and get its values: Before you work with an attribute, it is good practice to check whether it exists.
      - The hasAttribute() method of any element node lets you check if an attribute exists.

    - Creating attributes and changing their values: The className property allows you to change the value of the class attribute.

    - Removing attributes: Select the element and call removeAttribute().

    - Summary
      - The browser represents the page using a DOM Tree 
      - DOM Trees have four types of nodes: 
        - documemt nodes
        - element Nodes
        - attribute Nodes
        - text Nodes
      - You can select element nodes by their id or class attributes, by tag name, or by using CSS selector syntax.
      - Whenever a DOM query can return more than one node, it will always return a NodeList.
      - From an element node, you can access and update its contents using properties such as textContent and innerHTML, or using DOM manipulation techniques.
      - An element node can cointain multiple text nodes and child elements that are siblings of each other.
      - In oler browsers, implementation of the DOM is inconsistent.
      - Browsers offer tools for viewing the DOM tree.




  



