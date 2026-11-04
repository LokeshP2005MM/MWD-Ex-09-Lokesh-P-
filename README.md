# Exp 9 – React Lab Exercise: React Fragments

## NAME:  Lokesh P 
## REG NO: 2305001015  

## Aim
To understand and implement React Fragments to group multiple JSX elements without creating unnecessary HTML elements in the DOM.

## Objectives
- Understand the concept of React Fragments.
- Use Fragment shorthand syntax.
- Use the explicit Fragment syntax.
- Group multiple JSX elements without an extra DOM node.
- Understand the difference between Fragments and div elements.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest react-fragments
cd react-fragments
npm install
npm run dev
```

Select React as the framework and JavaScript as the variant.

### Step 2: App.jsx – Using Fragment Shorthand

```jsx
function Student() {
  return (
    <>
      <h2>Student Details</h2>

      <h3>Name: Lokesh P</h3>

      <p>Register Number: 2305001015</p>

      <p>Department: Computer Science and Engineering</p>
    </>
  );
}

function App() {
  return (
    <>
      <h1>College Information System</h1>

      <Student />
    </>
  );
}

export default App;
```

### Step 3: Using Explicit Fragment Syntax

```jsx
import { Fragment } from "react";

function Student() {
  return (
    <Fragment>
      <h2>Student Details</h2>
      <p>Name: Lokesh P</p>
      <p>Register Number: 2305001015</p> 
      <p>Department: CSE</p>
    </Fragment>
  );
}

function App() {
  return (
    <Fragment>
      <h1>College Information System</h1>
      <Student />
    </Fragment>
  );
}

export default App;
```

## Output

### Fragment Shorthand Syntax

<img width="1024" height="397" alt="image" src="https://github.com/user-attachments/assets/533bc6da-4569-48e8-9f3e-8dc0aeee379f" />

### Explicit Fragment Syntax

<img width="952" height="341" alt="WhatsApp Image 2026-11-04 at 7 36 13 PM" src="https://github.com/user-attachments/assets/f925c8a0-4f11-4623-8543-2e028536a6e6" />

## Result

Thus, React Fragments were successfully implemented using shorthand and explicit syntax to group multiple JSX elements without creating unnecessary DOM elements.
