

 Answer the following questions clearly:

1. What is the difference between **getElementById, getElementsByClassName, and querySelector / querySelectorAll**?

  Ans:getElementById: Selects one element with the given unique id.It returns only one element.

       getElementsByClassName: Selects all elements that have a specific class name.Returns a live `HTML collection` not an array.

       querySelector: Select the first Element that matches any CSS selector. Or `null` if none found.

        querySelectorAll: Selects all elements that match any CSS selector .It returns a static `NodeList` of all matching elements.

2. How do you **create and insert a new element into the DOM**?

    Ans: 1. Create a new <p> element into the DOM
          const newParagraph = document.createElement('p');

          2. Set its text content
          newParagraph.textContent = 'Hello';

          3. Find the container where you want to insert it
            const container = document.getElementById('container');

        4. Insert the new element inside the container
              container.appendChild(newParagraph);

3. What is **Event Bubbling** and how does it work?

    Ans: Event Bubbling is the process where an event starts at the target element and propagates upward through its ancestors.
          It allows parent elements to listen for events on their child elements.

          How does Event Bubbling work?

          Event Bubbling means when user click on an element (like a button), the click event first happens on that element, then it "bubbles up" to its parent, then to the parent's parent, and so on, all the way up the page.
          
       Can stop this bubbling if  want, so the event doesn’t go up to the parents.

4. What is **Event Delegation** in JavaScript? Why is it useful?

    Ans:Event Delegation in JavaScript means putting one event listener on a parent element instead of many listeners on its child   elements. When a child is clicked, the event "bubbles up" to the parent, and the parent’s listener can handle it.

    Why is it useful?
      Event Delegation Saves memory .Only one listener instead of many.
      Works for new elements. If  add new child elements later, the parent listener still works.
     

5. What is the difference between **preventDefault() and stopPropagation()** methods?

  Ans: preventDefault(): Stops the browser’s normal action.
       
      stopPropagation(): Stops the event from moving up to parent elements.
       


