# FORMS (HTML - Cahpter 7, pp.144-175)

Why Forms?

The best know form on the web is probabaly the search box, that sits right in the middle of google's homepage.

- Form controls
  - There are several types of form controls that you can use to collect information from visitors to your site.
    - Adding Text Fields
      - Text input
      - Passwords
      - Text area
    - Making Choices
      - Radio buttons
      - Checkbox
      - Drop down box
    - Submitting Forms
      - Submit button
      - Image Button
    - Uploading Files
      - File Upload
  
  How forms work: A user fills out a form, then pushes a button to upload it to a server.

  - A form may have several form controls, each gathering different information. The server needs to know which piece of imputted data corresponds with which form element. 

  ## Form Structure

  - Form controls live inside the `<form>` element. 
    - Every `<form>` element requires an attribute
  - Forms can be sent using one of two methods: 
    - Get 
      - Values are added to the end of the url specified in the action attribute. Ideal for:
        - Short forms
        - When retrieving data from the web server
    - Post 
      - Values are sent in HTTP headers. As a rule of thumb, you should use the post method for:
        - Users to upload a file.
        - Long forms
        - Sensitive data like passwords
        - Adding or deleting info from a database.

  If the method attribute is not used, the form data will be sent using the get method.
  
  ## Text Input

  - The `<input>` element is used to create several different form controls. When the type attribute has a value of text, it creates a single line text input.

  - Becasue servers needt to know which  form control is being used, each form control requires a name attribute. You can use the maxlength attribute to limit the number of characters in the field.

  ## Password Input

  - When the type attribute has a value of password (type="password"), it creates a single line of text that is blocked out. They will require:
    - name attribute
    - size, maxlength

  ## Text Area 

  - The `<textarea>` element is used to create a multi-line text input.

  ## Radio Button 

  - The (type="radio") radio button is used to pick just one of multiple options. Could contain the following attributes:
    - name
    - value
    - checked

  ## Checkbox Radio

  - The (type="checkbox") radio button is is used to select or unselect several options. Could contain:
    - name
    - value
    - checked

  ## Drop Down List Box

  - A drop down list box allows users to select one option from a drop down menu. Use the `<select>` element to create the option list, and the `<option>` element to specify the options available to the user.

  ## Multiple Select Box

  - You can turn a drop down select box into a box a box that shows more than one option by adding the size attribute.

  - Users can select more than one option, by adding the multiple attribute.

  ## File input box 

  - If you want to allow users to upload a file, you need to add the (type="file") attribute.

  ## Submit button

  - The (type="submit") button is used to send a form to the server.

  ## Image Button

  - If you want to use an image for the submit button, you can give the type attribute a value of image (type="image")

  ## Vutton and hidden controls

  - The `<button>` elemnt was introduced to give users more control over how their button was used.

  - To allow page authors to add values to forms that users cannot see, you use the (type='hidden") attribute.

  ## Labeling form controls

  - The `<label>` element can be used in two ways:
    - Wrap around both the text description and the form input.
    - Be kept separate from the form control, and use the FOR attribute to indicate which form control it is a label for.

  ## Grouping form Elements

  - You can group related form controls inside the `<fieldset>` element.
  - The `<legend>` element can come dirrectly from the `<fieldset>` element, and helps identify the purpose of the form.

  ## HTML5: Form Validation

  - Messages in the form control com efrom validation. Validating content helps to:
    - Redice the server load
    - Users can see if there are problems with the form.

  ## HTML: Data input 

  Many forms need tp gather info throuhg text input. HTML standardized this through:
    - type="date"
    - type="email"
    - type="url"
    - type="search"

  ## Summary

  - When you need to collect info, you need a form (`<form>` element)
  - Info from a form is sent in name/value pairs
  - Each form control is given a name, and the etxt that the user types in or the values of the options they select.
  - HTML5 introduced new form elements.

  # Lists, Tables and Forms (HTML - Chapter 14, pp. 33-357)

  ## Bullet Point Styles

  - The list-style-type property allows you to control the shape or size of a bullet point. It can be used to apply to the `<ol>`, `<ul>` and `<li>` elements.

  ## Images for bullets

  - The list-style-image property allows an image to act as a bullet

  ## Positioning the marker

  - The list-style-marker property indicated whether the marker should appear inside or outside of the box containing the main points.

  ## List Shorthand

  - Uses list-style

  ## Table Properties

  - width
  - padding
  - text-transform
  - letter-spacing, font-size
  - border-top, border-bottom
  - text-align
  - background-color
  - :hover

  ## Border on empty cells

  - Use the empty-cells property to show whether borders should be shown on empty cells.

  ## Gaps between cells

  - Use border-collapse and border-spacing

  ## Styling text inputs

  - font-size
  - color
  - background-color
  - border
  - border-radius
  - :hover
  - :focus
  - background-image

  ## Styling submit buttons

  - color
  - text-shadow
  - border-bottom
  - background-color
  - :hover

  ## Styling fieldsets and legends

  - Width
  - color
  - background-color
  - border
  - border-radius
  - padding

  ## Aligning form controls

  - Problem: Labels are often different lengths, which can throw our table off.
  - Solution: Use the FLOAT property to move the titles

  ## Cursor Styles

  - auto
  - crosshair
  - default
  - pointer
  - move
  - text
  - wait
  - help
  - url("cursor.gif")

  # Events (JS - Chapter 6, pp 243-292)

  ## Event Types
  
  - Event types and terminology on pp 246-247

  ## How events trigger JavaScript Code 

  1. Select the element node that you want the script to respond to.
  1. Indicate which event on the selcted node will trigger the response.
  1. State the code that you want to run.

  ## Three ways to bind an event to an element

  - HTML event handlers (DO NOT USE)
  - Traditional DOM event Handlers
    - Attach one function to each event handler.
      - `element.onevent = functionName;`
  - DOM Level 2 event listeners
    - If you use a named function when the event fires on your chosen DOM node, write that function forst.
    - Stored as a variable.

  ## Event listeners

  - Deal with more than one function at a time, but they are not supported by older browsers.

  ## Event Flow

  - Event Bubbling
    - `<a>`
    - `<li>`
    - `<ul>`
    - `<body>`
    - `<html>`
    - DOCUMENT

  - Event capturing
    - DOCUMENT
    - `<html>`
    - `<body>`
    - `<ul>`
    - `<li>`
    - `<a>`

  ## The Event Object

  - When an event occurs, the event object tells you information about the event.

  ## Event Delegation

  Creating event listeners for a lot of elements, can slow a page down, but event flow allows you to listen for an event on a parent element. pp. 268.

  ## Different types of Events

  - W3C DOM events
  - HTML5 Events
  - BOM Events

  ## User interface Events

  UI events occur as a result of interaction with the browser window rather than the HTML page. 

  ## Mouse Events

  Fired when the mouse is moved onto a button (pp. 276)

  ## Keyboard Events

  Fire with any device with a keyboard.

  ## Summary

  - Events are the browsers way of indicating when something has happened. Like a page has finished loading.
  - Binding is the process of stating which event you are waiting to happen, and which event you are waiting for that event to happen upon.
  - When an event occurs on an element, it can trigger a JS function. When this function changes the webpage in some way, it feels interactive because it has responded to the user.
  - You can use event delegation to monitor for events that happen on all of the children of an event.
  The most commonly used events are W3C DOM, althouhg there are others in the HTML specification as well as browser-specific events.










