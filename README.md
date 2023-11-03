Step 1: Pass setShowCategoriesDropdown as a Prop

- In the parent component App.js, you need to pass
down the setShowCategoriesDropdown function as a prop.

Step 2: Use setShowCategoriesDropdown in
CategoryDropdown

- In the CategoryDropdown component, use the
setShowCategoriesDropdown function to control
the visibility of the dropdown.

Step 3: Create a Ref

- Create a ref using the useRef hook. This ref
will be used to reference the dropdown element.

Step 4: Create a Function to Handle Outside Clicks

- Define a function, such as handleClickOutside(event),
that will be called when a click event occurs
outside the dropdown.

Step 5: Add Event Listener for Clicks

- Use document.addEventListener to listen for 
the "mousedown" event on the entire document.

Step 6: Attach Event Listener in useEffect

- Inside a useEffect hook, attach the event listener
created in step 3. This hook should run when
the component mounts.

Step 7: Remove Event Listener in Cleanup

- In the same useEffect hook, return a cleanup
function that removes the event listener. 

Step 8: Include Dependencies in useEffect
Dependency Array

- Make sure to include any dependencies of the
useEffect hook in its dependency array to
ensure that the hook behaves correctly.

Step 9: Toggle Dropdown Visibility

- Inside the handleClickOutside function,
toggle the visibility of the dropdown
based on whether it's currently open.

