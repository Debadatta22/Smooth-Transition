# Smooth-Transition
🌟 Major Project 1: Dynamic Section Transitions 🚀 Created a seamless toggle between White and Black sections using HTML, CSS, and React. Smooth transitions, state management with React’s useState, and a centered layout via CSS Flexbox bring this project to life. Phrases like “Welcome to my Project” make it uniquely mine.


# Project Title:
Create Transition Effects from White Section to Black Section Using HTML, CSS, and React

# Project Concept:  
This project demonstrates how to create smooth and seamless transitions between two visually contrasting sections—**white** and **black**—using **HTML, CSS, and React**. A button acts as a trigger to toggle the sections dynamically, providing users with an interactive and visually appealing experience.


### **Key Components and Workflow**  

1. **HTML Structure**:  
   - The core HTML file (`index.html`) contains the root container:  
     ```html
     <div id="root"></div>
     ```  
   - React dynamically renders components into this `root` using ReactDOM.  


2. **React (App.js):**  
   - **State Management**: The `useState` hook defines a state variable (`isWhiteSection`) to determine the current background—**white** or **black**.  
   - **Event Handling**: A `handleToggle` function toggles the state when the button is clicked.  
   - **Conditional Rendering**: The `isWhiteSection` state conditionally applies either the `white-section` or `black-section` CSS class to switch backgrounds.  
   - **Render Output**:  
     ```jsx
     <div className={isWhiteSection ? "white-section" : "black-section"}>
       <div className="content">
         <h1>Welcome to my Major Project 1</h1>
         <p>This was created by Debadatta Rout</p>
         <button onClick={handleToggle}>Switch Section</button>
       </div>
     </div>
     ```  

---

3. **CSS (style.css):**  
   - **Smooth Transition**: The `transition` property ensures a gradual change of the background color over 1 second:  
     ```css
     .white-section, .black-section {
       height: 100vh;
       display: flex;
       justify-content: center;
       align-items: center;
       transition: background-color 1s ease;
     }
     .white-section {
       background-color: white;
       color: black;
     }
     .black-section {
       background-color: black;
       color: white;
     }
     ```  
   - **Flexbox Layout**: Ensures content is centered both vertically and horizontally regardless of screen size.


### **Working Flow**:  
1. **Initial State**:  
   - The webpage loads with a white section (`isWhiteSection = true`).  
   - The content (heading, button, and phrases) appears centered on the screen.  

2. **User Interaction**:  
   - When the button is clicked, the `handleToggle` function switches `isWhiteSection` from `true` to `false` (or vice versa).  

3. **Dynamic Update**:  
   - The background transitions smoothly:  
     - From white to black (when `isWhiteSection = false`).  
     - From black to white (when `isWhiteSection = true`).  

4. **User Feedback**:  
   - The button’s text remains interactive.  
   - The transition provides a clean, visually appealing effect, ensuring a better user experience.  


### **Summary**  
By combining **React's state management** with **CSS transitions**, this project effectively demonstrates:  
- Smooth and dynamic section switching.  
- Responsive, clean layout via Flexbox.  
- Seamless integration of user interaction and animation.  

It’s a simple yet powerful example of how React and CSS can be used to enhance interactivity and deliver smooth UI effects. 🚀  

