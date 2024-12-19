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

Day 12: 06/12/24

Today, I faced challenges while trying to setup the billing on AWS in order to have access to S3. The issue was due to the NG debit card I was trying to use. It had me stuck for a while but I was able to find my way around it. So, in order to get the application running. I read up on alternatives. Which I finally opted for Docker. So, I started with the docker setup and I was able to get the docker running.  The next thing is to start with the Backend and frontend connection 

Day 13: 07/12/24

Today, 
- I was troubleshooting issues related to AWS CLI configuration and environment setup.
- I was able to setup AWS LocalStack to simulate AWS services like S3.
-  I set up and tested the AWS CLI to interact with LocalStack's S3 emulation, including creating a bucket, uploading files, and running tests locally.

  Day 14: 08/12/24
  
 -  I spent today learning React on FreeCodeCamp. I solved a couple of challenges on React and also learned about the Single-Responsibility Principle (SRP), i.e., that a component should ideally only do one thing.
 -  I published a blog post on my week two of #100DaysOfCode. The blog post was a highlight of the progress, challenges and what I was able to learn over the course of week 2 on this journey.

Day 15: 09/12/24

- I was able to implement encryption in the upload.js file using node.js by using built-in crypto module. This ensure that the document is encrypted locally before it is uploaded to S3.
- I learned how to generate a strong secret key in node.js terminal, which I was able to use the generated token for the JWT secret
- I did a lot of troubleshooting as well. 

Day 16: 10/12/24

- I setup MongoDB for the application
- I added more Routes(CRUD Operations) for the app.
- I worked on the functionalities.
- The app is getting ready. I can't wait to get to the deployment phase.

Day 17: 11/12/24

- I started implementing the backend API for document upload and encryption.
- I did a lot of troubleshooting while trying to connect the docker container with the API.
- I read two blogs on Docker with S3, for better understanding and easy debugging.

Day 18: 12/12/24

- I was able to find solution to the challenge I faced throughout yesterday.
- I had the backend API for document upload and encryption running perfectly well
- I setup user storage service for the app.
- I integrated AWS S3 storage with MinIO using Docker

Day 19: 13/12/24

- I started working on the app dashboard.
- I worked with React and Tailwind
- I will probably be spending the weekend on the dashboard.
 
Day 20: 14/12/24

- I started updating dashboard features
- I worked on the document overview
- I worked on the document uploading area
- I worked on search and tagging sections
- I worked on security indicators

Day 21: 15/12/24

- I read about heroicons as a popular React and Tailwind CSS library.
- I learned the key differences between solid and outline icons and when to use either of these two
- I also learned about Mini and Micro heroicons.
- I completed the dashboard. I want to add the Dark and light mode functionality. I started with it but not working as I expected yet, I will be doing some troubleshooting on that.
- I wrote and published a blog post on week 3 of this #100DaysOfCode journey. 

Day 22: 16/12/24

- I added dark mode feature on the app frontend
- I setup backend APIs for organizing documents with S3 integration
- I started with the backend APIs for deleting documents with the S3 integration

Day 23: 17/12/24

- I added frontend hooks to call the backend for file uploads and manage encrypted file viewing
- Did some troubleshooting/debugging
  
Day 24: 18/12/24

- Added error handling for failed file uploads, authentication failures, etc.
- Implemented search functionality in the frontend to filter documents based on tags or names.

Day 25: 19/12/24

- I added a complete password reset flow with email verification
- I added email verification for document actions
- Implemented secure API endpoints for all operations
