# EJStags
This repository demonstrates the usage of Embedded JavaScript (EJS) templating engine in a simple Express.js application. The main goal of this project is to showcase how to dynamically render HTML content with EJS tags based on the current second of the server's time.

# Getting Started
To run this project locally, follow these steps:

Clone the repository:

bash
Copy code
git clone https://github.com/your-username/ejs-tags-demo.git
Navigate to the project directory:

bash
Copy code
 ´´´cd ejs-tags-demo
Install dependencies:

bash
Copy code
 ´´´npm install
Run the application:

bash
Copy code
npm start
The server will start, and you can access the application at http://localhost:3000 in your web browser.

### Overview
The main file of interest is views/index.ejs, where the dynamic content is defined using EJS tags. Let's break down some key elements:

<%= title %>: Displays the title dynamically.
<%= seconds %>: Shows the current second dynamically.
<% if (seconds % 2 === 0) { %>: Checks if the current second is even.
<ul>: Displays a list of items if the second is even.
<% for (let i = 0; i < items.length; i++) { %>: Iterates over items.
<%= items[i] %>: Displays each item in a list.
<% } else { %>: Displays a message if the second is odd.
<p>No items to display</p>: Message for odd seconds.
<%- htmlContent %>: Renders HTML content dynamically.
<%- include("footer.ejs") %>: Includes the footer using EJS.
