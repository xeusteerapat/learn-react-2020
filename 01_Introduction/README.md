# Introduction to React.js

*A JavaScript library for building user interfaces.* React is a declarative library that can create interactive UIs that will efficiently update and render just the right components when data changes. React can build encapsulated components that manage their own state, then compose them to make complex UIs.

## Components

Component is the main building blocks of React. Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.

There are 2 ways to create React components, the first one is "Class components" and the second one is "Functional components"

```javascript
// Class components
class Welcome extends React.Component {
  render() {
    return <h1>Hello</h1>;
  }
}

// Functional components
function Hello {
    return <h1>Hello</h1>;
}
```
