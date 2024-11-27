Day1: 25/11/24

Today I started working on a project(Personal Document Vault with Encryption). I set the project architecture
I completed a module in the Meta backend development specialization.

Day2: 26/11/24

Today, I started working on the frontend part of the project. 
I spent a couple of hours on the official documentation of React.

### Basic Concepts of React

1. Components: React applications are built using components. A component is a reusable piece of UI.
Components can be functional or class-based.

2. JSX: JSX is a syntax extension for JavaScript that looks similar to HTML. It is used to describe what the UI should look like.
Example: `const element = <h1>Hello, world!</h1>;`

3. Props: Props (short for properties) are used to pass data from one component to another.
   
Example: 
```
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```
4. State: State is a way to manage data that changes over time within a component.

Example: Using Hook
```
import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

5. Lifecycle Methods: Class components have lifecycle methods that allow you to run code at specific points in a component's lifecycle.
Example:

```
class Clock extends React.Component {
  constructor(props) {
    super(props);
    this.state = { date: new Date() };
  }

  componentDidMount() {
    this.timerID = setInterval(
      () => this.tick(),
      1000
    );
  }

  componentWillUnmount() {
    clearInterval(this.timerID);
  }

  tick() {
    this.setState({
      date: new Date()
    });
  }

  render() {
    return (
      <div>
        <h1>Hello, world!</h1>
        <h2>It is {this.state.date.toLocaleTimeString()}.</h2>
      </div>
    );
  }
}
```

Day 3: 27/11/24

Today,what I did on my personal project, was that I spent 2 hours on FreeCodeCamp React course.
I worked on the tasks given to me by my team member for an Hackathon. So, today, I started working on the Login and Register route for what we're building.
