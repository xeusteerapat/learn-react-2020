# Introduction to React.js

_A JavaScript library for building user interfaces._ React is a declarative library that can create interactive UIs that will efficiently update and render just the right components when data changes. React can build encapsulated components that manage their own state, then compose them to make complex UIs.

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

// or with ES6 Arrow function
const Hello = () => {
  return <h1>Hello</h1>;
}
```

Let's see some example with a todo list app using react components principle.

![todo app](todo_app.png)

- `TodoListItem` component that can be reused for each todo item in the list.
- `TodoList` component that contains list of all the todo items.
- `TodoForm` component that allow user to add new todo item.
- `TodoApp` component that uses all components as above to create entire application.

To create an react application, we need to understand `JSX` syntax that I will explain in the next section.
