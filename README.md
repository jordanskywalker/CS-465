# CS465

Architecture:

In this project, I used a few different types of frontend development. The customer-facing side used Express with HTML, JavaScript, and Handlebars templates to render pages like the travel page. This worked well for displaying trip information from the database in a more traditional website format. The admin side used Angular as a single-page application, which gave the site more interactive functionality. With Angular, the page could add, edit, and update trips through API calls without needing the same kind of full-page reload that a basic Express page would use.

The backend used MongoDB because the project needed a flexible NoSQL database for storing trip data. Since each trip is stored like a document with fields such as code, name, price, resort, image, and description, MongoDB worked well for this type of application. It also connected smoothly with Node and Express through Mongoose, which made it easier to define the trip schema and perform database actions.

Functionality:

JSON is different from JavaScript because JSON is a data format, while JavaScript is a programming language. JSON uses a structured format of key-value pairs, which makes it easy to send data between the frontend and backend. In this project, JSON tied the full stack together because the Express API returned trip data as JSON, and the Angular admin app used that data to display, add, and update trips.

One example of refactoring was moving from static HTML pages to Handlebars templates and then using Angular components for the admin side. This improved the project because the same structure could be reused instead of rewriting the same code on multiple pages. Reusable UI components also made the application easier to maintain because features like trip listing, adding trips, and editing trips were separated into their own parts.

Testing:

Testing in this project involved checking different API methods and making sure each endpoint worked correctly. GET requests were used to retrieve all trips or one specific trip. POST requests were used to add a new trip, and PUT requests were used to update an existing trip. These endpoints had to be tested through the browser, the Angular app, and the database to make sure the data was actually being saved and returned correctly.

Security added another layer to testing because the admin features required authentication. It was not enough for the pages to load. I also had to make sure that protected actions like adding or updating trips only worked after logging in. This helped me understand how methods, endpoints, and security all work together in a full stack application.

Reflection:

This course helped me understand how a full stack web application is built from front to back. Before this project, I had worked with individual parts like HTML, JavaScript, APIs, or databases, but this course helped me see how they connect in one complete system. I gained more practice with Express, Angular, MongoDB, routing, API testing, and authentication.

These skills help me move closer to my professional goals because full stack development is a valuable area in computer science. Being able to build both the customer-facing side and the admin side of an application makes me a stronger candidate because I can understand how the user interface, backend logic, and database all work together.
