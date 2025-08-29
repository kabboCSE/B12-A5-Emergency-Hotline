1. Difference between getElementById, getElementsByClassName, querySelector / querySelectorAll

getElementById("id") → Finds one element by ID.

getElementsByClassName("class") → Finds all elements with a class (HTMLCollection, live).

querySelector("css") → Finds the first match using CSS selector.

querySelectorAll("css") → Finds all matches (NodeList, static).

2. Create and insert a new element into the DOM

let div = document.createElement("div"); // create
div.textContent = "Hello";               // add content
document.body.appendChild(div);          // insert into DOM


3. Event Bubbling
Events start from the target element and bubble up to parent elements.
Example: clicking a button → event goes from button → div → body → document.

4. Event Delegation
Attach one event listener to a parent element to handle events on its children.


5. Difference between preventDefault() and stopPropagation()

preventDefault() → Stops default action (e.g., form submit, link navigation).

stopPropagation() → Stops event from bubbling up to parent elements.
