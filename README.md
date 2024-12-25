## What is React?

React is a JavaScript library for building user interfaces, developed by Facebook. It allows you to build fast, scalable web applications with components that can be reused and managed efficiently.

## components in React

🔹In React, everything is a component! Components are the building blocks of a React app.
🔹They are independent, reusable pieces of code that return UI elements.

## What is Rendering of Components?

🔹Rendering in React refers to how components are displayed on the screen.
🔹In React, we create a component once and then render or invoke it wherever we need it. When the state or props of a component change, React will re-render the component to reflect the changes. 

## Components Hierarchy

🔹In React, components can be nested. A parent component can contain child components, and each child can have its own nested components. 

## What is JSX?

🔹JSX (JavaScript Extension Syntax) allows you to  write HTML-like syntax within JavaScript. 
🔹It might look like HTML, but it’s actually a syntax extension for JavaScript. React uses JSX to define components.

## Create React App vs Vite

When setting up a React project, two of the most popular options are Create React App and Vite. Let’s compare them:

## Create React App (CRA):

Comes with built-in configurations.
Easy to use for beginners.
Can be slower in larger projects due to bundling.

## Vite:

Newer, faster, and optimized for performance.
Great for modern JavaScript features and faster development.
Objects as State Variables

## State isn't limited to simple values like strings or numbers. It can handle objects too! Here's how :

🔹 Example:
const [user, setUser] = useState({ name: "John", age: 25 }); 
const updateName = () => { 
 setUser((prevUser) => ({ ...prevUser, name: "Jane" })); 
}; 

## Why Spread Operator?

React doesn’t merge objects automatically like class components. Always use the spread operator to copy other properties you don’t want to lose!

## Arrays as State Variables

Updating arrays can be tricky but fun! Instead of directly modifying the array, React encourages immutability.

🔹 Example: Adding an item
const [items, setItems] = useState([1, 2, 3]); 
const addItem = () => { 
 setItems((prevItems) => [...prevItems, 4]); 
}; 

## Unique Keys for List Items

When rendering lists in React, every child should have a unique key. React uses these keys to keep track of items efficiently and optimize re-renders.

🔹 Example:
const listItems = items.map((item, index) => ( 
 <li key={index}>{item}</li> 
)); 

# LIVE DEMO
https://delightful-churros-8574e6.netlify.app/
