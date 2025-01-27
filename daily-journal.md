Day 1: 25/11/24

Today I started working on a project(Personal Document Vault with Encryption). I set the project architecture
I completed a module in the Meta backend development specialization.

Day 2: 26/11/24

Today, I started working on the frontend part of the project. 
I spent a couple of hours on React's official documentation.

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

Today, what I did on my personal project, was I spent 2 hours on the FreeCodeCamp React course.
I worked on the tasks given to me by my team members for an Hackathon. So, today, I started working on the Login and Register route for what we're building.


Day 4: 28/11/24

Today, I set up the login page for my app. I handled the backend authentication as well.
I read up on tailwinds.

Day 5: 29/11/24

Today, I set up a database for the Hackathon application. 
I connected the authentication endpoint

Day 6: 30/11/24

Today, I created the entire database for the Hackathon app using Postgres PgAdmin. I worked on the connection with the API endpoint using postman. I added two more fields to the registration form.

Day 7: 01/12/24

Today, I focused on my personal document vault project.
I was able to test the API endpoint using a cURL API client request; a command based API testing automation and tried the Postman API client; a GUI API client request. I read about some other open source alternatives to these two. 

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

- I read about hero icons as a popular React and Tailwind CSS library.
- I learned the key differences between solid and outline icons and when to use either of these two
- I also learned about Mini and Micro hero icons.
- I completed the dashboard. I want to add the Dark and light mode functionality. I started with it but not working as I expected yet, I will be doing some troubleshooting on that.
- I wrote and published a blog post on week 3 of this #100DaysOfCode journey. 

Day 22: 16/12/24

- I added a dark mode feature on the app frontend
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

Day 26: 20/12/24

- I did some fine-tuning on the app dashboard
- I started with the testing
- Spent a couple of hours on debugging

Day 27: 21/12/24

- Preparing for an interview (The interviewer didn't show up. I waited more than 1 hr)
- I worked on the Docker part of the project and did some troubleshooting(uninstalling and reinstalling)

Day 28: 22/12/24

- I added a feature for deployment(dev container) using an open-source platform known as Daytonai to the URL-shortened app
- I set up comprehensive documentation for the repository
- I wrote an article on the app
- I submitted the project for an Open Source Hackathon
- I wrote another article on Week four #100DaysOfCode

Day 29: 23/12/24

- I set the password reset section for the app
- I implemented email notifications for document upload and deletion
- I integrated forgot password section on the frontend to the backend

Day 30: 24/12/24

- I was able to complete the frontend part of the app.
- I did all the frontend and Backend integrations. Everything is working perfectly fine
- I only need to carry out a couple of tests before deployment.

Day 31: 25/12/24

I didn't do much today. The Project I submitted for an open source Hackathon got accepted. I received some suggestions which I worked on throughout the night. I spent the rest of the day resting.

Day 32: 26/12/24

- I implemented the OpenSSL certification setup on the Backend for the app.
- I finally started testing the application.

Day 33: 27/12/24

- I implemented a rate limiter to protect all routes from excessive  request
- I continue with testing and debugging a lot.

Day 34: 28/12/24

- I continue with the testing
- I set up the Rancher desktop with the S3 for data storage using a Docker container.
  
Day 35: 29/12/24

- I was able to fixed docker-rancher issues.
- I spent half of the day on FreeCodeCamp React course.
- I published a blog post on week 5 recap.

Day 36: 30/12/24

- I worked on the app readme
- I completed the tests.
- I pushed it to GitHub and deployed it on Vercel
- I applied for an MLH fellowship.

Day 37: 31/12/24

- I started working on a GitHub issue.
- I sourced resources for learning the Golang.

Day 38: 01/01/25

- I worked on the Bitcoin test challenge repository. I made changes and worked on the failing tests.
- I learned how to use Visual Studio Developer Building tools.
  
Day 39: 02/01/25

- I started learning Golang by exploring the official Go documentation.
- I had a meeting with a GitHub product team member about my experience using GitHub Co-pilot. (Sadly, the network did me dirty)
- I built a small app for blog reading streak which I am planning on integrated to my GitHub Readme profile.

Day 40: 03/01/25

- I wrote some functions in Golang programming language today. I learned more about compiler and runtime errors.
- I learned when to use naked returns and when to use named returns
- I also learned the Guard clause and how it provides a linear approach to logic trees.
- I am currently Reading "Ultralearning by SCOTT H. YOUNG", and I am trying to implement what I am learning in the book to approach this new programming language I am learning and see the changes. 

Day 41: 04/01/25

- I worked on the Leetcode question (two sums). My approach was to write down my thought process on paper and implement it in VS Code. I transferred the solution to Leetcode and submitted it after all the test cases passed.
- I started with the draft for week 6 of the #100DaysOfCode blog post, which I will publish tomorrow.

Day 42: 05/01/25

- I worked on a leet code question (Merge sorted array)
- I published the week 6 recap of the #100DaysOfCode blog post.

Day 43: 06/01/25

- I continue learning the Go programming language.
- Today, I learned about structs, interfaces and switches
- 

Day 44: 07/01/25

- Today, on the Go programming language, I was able to learn;
- errors, formatting, fizz buzz, and slices.
- I check the official documentation for more understanding
- I was able to try out some exercises on each topic.

Day 45: 08/01/25

- Today, I learned about mutations, maps, and advanced functions in Go
- I practiced exercises on those topics.

Day 46: 09/01/25

Today, 
- I delve deep into advanced functions in the Go programming language, such as higher-order functions, first-class functions, anonymous functions, currying, defer, closures, and pointers.
- I practiced a few problems on each of the topics.
  
Day 47: 10/01/24

- I learned channels, mutex, and generic in Go programming language.
- I practiced problems on the topics.
Based on the resources I am using and the roadmap I created for learning this programming language, I can say I have been able to cover the basics of the Go programming language. The rest of my learning will be project-based.
- Next thing, I will work on 3 projects for now on GO, which are, basic, medium and advance.
- The weekend(Sat & Sun) for leetcode, however I will also research on the project to work on this weekend and start with by Mon.

Day 48: 11/01/24

- I solved "remove element" problem on leetcode.
- I wrote and published a blog post on my 2024 review.

Day 49: 12/01/25

- I worked on leetcode problem"Remove duplicate from sorted array"
- I published a blog post on week 7 of #100DaysOfCode
 

Day 50: 13/01/25

- I started working on a new project "expense tracker" using Golang. I will be applying what I have learned so far on Go and learn new concepts on the project. 

Day 51: 14/01/25

- I continue working on the expense tracker.
- I did troubleshooting and I read up on Database connections in Go.

Day 52: 15/01/25

- I hopped on a challenge where I have 24hrs to build an app using GitHub Copilot and write a blog post about it.
- I built a dynamic habit tracker app within 18 hours with detailed documentation on the app, published a blog post about the app and turned in my submission.

Day 53: 16/01/25

- Today,  I continued working on the expense tracker app with Go.

Day 54: 17/01/25

- I continued working on the app and I spent most of the day debugging and reading the documentation

Day 55: 18/01/25

- I worked on leetcode problem question 80 on Array(Remove Duplicates from Sorted Array II)
- I spent some times reading a couple of chapter on a programming book

Day 56: 19/01/25

- I worked on the leetcode problem question 169 on the array(Majority element).
- I published a recap blog post for week 8 of #100DaysOfCode
  
Day 57: 20/01/25

- I was able to add two extra features to the app.
- I read more about URL Parsing and JSON in GO

Day 58: 21/01/25

- Today, I didn't have achieved much. As I was finding the solution to one bug, I was facing another bug. I am still finding my way around it till now. One of those frustrating days but I learned some new concepts while solving the problems.

Day 59: 22/01/25

- I fixed the bug I that had me stuck yesterday. The application is working fine now for the command line interface 
- I have started implementing the live web application feature. Already added ths necessary dependencies.

Day 60: 23/01/25

- I added the HTML and CSS pages to the app. It remains JS for the app's interactivity. I am trying different features that are simple and functional. I should be done with the app this week.
- I also read extensively on panic in Go. I faced some panic while testing the app. I learned more about understanding and preventing panic in Go

Day 61: 24/01/25

I implemented on some essential security measures for the app, which are user authentication,  password hashing,  http implementation,  sql injection prevention, and CSRF protection 

Day 62: 25/01/25

- I solved a question on leetcode ( Rotate Array)
- I studied a few pages in a book, cracking the coding interview.

Day 63 : 26/01/25

- I solved a problem on LeetCode (Best time to buy and sell stock)
- Publish a blog post on the recap of week 9 of my #100DaysOfCode 
- Read a few pages on the book Cracking the Coding interview

Day 64: 27/01/25

- I resumed back to working on the expense tracker app in Go. I started adding more features for enhancements. I worked on some HTML pages, including their CSS and JS.
- I will work on the mobile app version once I am done with the web app.
