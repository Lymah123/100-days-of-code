Day 1: 25/11/24

Today I started working on a project(Personal Document Vault with Encryption). I set the project architecture
I completed a module in the Meta backend development specialization.

Day 2: 26/11/24

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


Day 4: 28/11/24

Today, I setup the login page for my app. I handled the backend authentication as well.
I read up on tailwindcss.

Day 5: 29/11/24

Today, I setup database for the Hackathon application. 
I connected the authentication endpoint

Day 6: 30/11/24

Today, I created the entire database for the Hackathon app using Postgres PgAdmin. I worked on the connection with the API endpoint using postman. I added two more fields to the registration form.

Day 7: 01/12/24

Today, I focused on my personal document vault project.
I was able to test the API endpoint using cURL API client request; a command based API testing automation and tried Postman API client; a GUI API client request. I read about some other open source alternatives to these two. 

Day 8: 02/12/24

Today, 
- I set up the MongoDB(Database)  
- I connected the Backend to MongoDB
- I handled file upload functionality
- And I handle the integration of AWS S3 for secure storage

Day 9: 03/12/24

Today, I worked on the app's front end. I set up the login page, register page, and dashboard.
I spent a couple of hours on the FCC react course.

Day 10: 04/12/24

- I spent half of today debugging. I was able to figure out some 
- I spent a few hours on FCC React course

Day 11: 05/12/24

- I was able to debug the error I have in the code.
- I started setting up connections with Backend and frontend
- I setup an account on AWS
- I added a dark mode toggle to the app.
