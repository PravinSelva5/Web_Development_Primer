# Web Development: a Primer

Created By: Pravin Selvarajah
Last Edited: May 24, 2020 12:27 AM
Tags: Web Development

# The Front End

## HTML

- True Programming languages have the ability to describe logic. HTML, however, is used to display and format parts of a webpage.
- Everything in an HTML document is enclosed in <HTML> tags
- The <head> tag contains metadata such as the page title, links to CSS and JS files, and keywords that are used by search engines like Google
    - Not displayed in the browser
- The <body> tag actually contains the actual markup like paragraphs, images, and tables that are **displayed in the browser./**
- The *doctype* is a declaration that the browser the HTML version that the document is written in.
- Example:
![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled.png)


- HTML comments look like this:
    - <! - - Comment - - >
- Attributes are always placed in the opening tag of an element and exist as key/value pairs:

![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%201.png)

## CSS

- The purpose of CSS is to restore HTML to its original status as a structural language.
- There are three ways of adding CSS to the HTML Code
    - Inline CSS
        - When CSS is used in the **style attribute** of HTML tags.
        - This is inefficient and not scalable

        ![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%202.png)

    - Internal CSS
        - You can use <style> tags within the <head> of the HTML to define the style of a certain tag
    - External CSS
        - CSS is written in a separate file
        - You can link the CSS file to the HTML file by writing a **self-closing link tag in your HTML head:**

            ![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%203.png)

        - The **rel** attribute of the link element above tells the HTML to import a CSS file
- Page Layout Techniques
- Animations
- Preprocessors
    - **Syntactically Awesome Style Sheets (SASS) and Leaner Style Sheets (LESS)** are language extensions for CSS that allow you to use more conventional programming constructs such as *variables, conditionals, and loops.*

## Javascript

- Javascript is syntactically similar to C and C++
- Javascript allows you to implement complex things on web pages
- On Mac to view a console on the browser, hit Cmd+Option+J
- Javascript can be written directly into an HTMl file using the <script> tag
- You can also import javascript files into the HTML file similar to CSS

![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%204.png)

- You can place an external reference in either the <head> or <body>.
- The HTML structure can be mapped onto a **tree**. The DOM stores these HTML elements as objects that can then be manipulated in various ways through JavaScript

# The Back End

## What is the Back End?

- The Back end of a website loosely consists of a server, database, and APIs.
- A web server is a system that delivers content and services to users over the Internet
- Web Hosting Services?
    - Web Hosting companies provide space on a server that is owned or leased for use by clients, as well as providing Internet connectivity, usually in a data center.
- Web server operating systems include:
    - Linux
        - packaged in the form for both desktop and server use
    - CentOS
        - Stable and infrequent crashes
        - Difficulty in running newer packages
    - Debian
        - works on both Desktop & server
    - Ubuntu
        - most popular Linux distro for the desktop

## Micro-service Architecture

- Websites are hosted on virtual machines. As a result, a website is essentially hosted on a **server within a server, and that server delegates tasks to other servers.**
- Many Virtual Machines exist on one physical server, and each has a separate job (ex: interface).
- Micro-services structures an application as a collection of services that are:
    - Highly maintainable and testable
    - Loosely coupled
    - Independently deployable
    - Organized around business capabilities

## Back-End Programming

- Back End Engineers are responsible to program servers to process user requests & respond with the requested resource correctly.
    - They also write code to process and store user data
- Efficient storage and delivery of information
- Customized user experience
- Controlled access to content
- Store session/state information
- Notifications
- Data Analysis

## Node JS

- It's an asynchronous event driven javascript runtime, Node is designed to build scalable network applications and upon each connection the **callback is fired**, BUT fi there no work to be done, **NODE WILL SLEEP**
- In other words, node can handle multiple connections at once, **which makes them more efficient**
- Node is great for software prototyping
- Node is also incredibly fast and highly scalable

# Web Development Frameworks

## What are the Frameworks?

- A **web framework** is defined as a package made up of a structure of files and folders of standardized code.
    - This can be used to support the development of websites as a basis to start building a site
- Essentially, frameworks are used to simplify the web development process
- Most web application frameworks rely on the **Model View Controller** architecture
    - **Model**
        - Stores all information about the content and structure of the application
        - Once it receives input from the C**ontroller**, it will send the required information to the **View** component.
    - **View**
        - most commonly known as the **user interface**
        - View takes input from the user to the **Controller** for **processing** and the **instructions are sent from the Model**
    - **Controller**
        - middle man for the Model and the View

    ![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%205.png)

### Types of Frameworks

- Front -end (client-side) frameworks
    1. Angular JS
    2. Bootstrap
    3. React.js
    4. Backbone
    5. Semantic-UI
- Back-end (server-side) frameworks
    1. Express (JS)
    2. Symfony (PHP)
    3. Django (PHP)
    4. Ruby on Rails (Ruby)
    5. ASP .NET (C#)
- Isomorphic (client-server) frameworks
    1. Meteor JS
    2. Lazo.js
    3. Rendr

## Front-End Frameworks

1. Angular (Google)
    - Designed for creating dynamic web applications
    - highly expressive, readable, and quick to develop
    - **used to update the user interface in real time and provide a highly interactive website**
2. Bootstrap (Twitter)
    - used to ease up the process of adding CSS to HTML
    - adheres to responsive web design standards
3. React.js
    - Used for building UI's, essentially the View layer of an MVC application
    - allows you to build encapsulated components, each of which **manages its own state, and then compose them to make complex User Interfaces.**
        - Therefore, when data changes, only the **concerned components are updated**
4. Backbone
    - allows you to structure your JS code in an MCV form
    - helps you avoid a myraid of callbacks and other extraneous pieces of code that make changes complicated
    - Any changes to these models automatically trigger changes to any views that display these models.
5. Semantic-UI
    - highly desirable for beginners
    - has multiple third party libraries so development process is easier
    - not viable for developing websites with more complex structures

## Back-End Frameworks

1. Express
    - standard server framework for Node.js
    - minimal and highly flexible node.js web application framewokr
    - simpligy back-end development process enough to reduce basic back-end features to a **single instruction**
2. Symphony
    - essentially a set of reusable components
    - you can focus on the higher level functionality with the mundane tasks become confined to much smaller pieces of code.
3. Django
    - takes care of reducing code for basic functionalities to simple instructions.
4. Ruby on Rails
    - built on MVC architecture
5. ASP .NET
    - Developed by Microsoft to facilitate the process of developing dynamic web pages
    - can create not only simple &  fast but also has the capacity to scale to millions of user

## Isomorphic Frameworks

- These frameworks allow developers to write their entire application in a single framework w/o worrying about integrating multiple components
1. Meteor JS
    - allows for prototyping
    - allows for versioins of the same application to be stored and tested
    - produces code that can span multiple platforms (Android, iOS, and the web itself)
    - On the back-end, it integrates MongoDB. It creates a DBMS that enables data changes to be generated to the client-side
    - On the client side, it has its own templating engine Blaze.
        - It can also be integrated with angular or react frameworks
2. Lazo.js
    - built on Node.js
    - provides an optimized first-page load with the help of tools such as Backbone.js, RequireJS, and jQuery
    - user interface separated into mutually exclusive components
3. Rendr
    - allows you to run your Backbone.js applications on both the client and the server

## Software Stacks

### LAMP stack

- Linux (OS), Apache (HTTP server), MySQL (relational database), and PHP (programming language the app is built on)

### MEANStack

- Consists of:
    - MongoDB
        - serves as the database
        - It acts as the **Model** in MVC as it is the storage component of the website
    - Express JS
        - this is used to create the backend of the web application
        - creates the server, handling all kinds of requests coming in from the client end & processing data from the database accordingly
        - In the MVC architecture, Express would be the **Controller**
    - Angular JS
        - used to create the front-end of the application
        - used to program everything that happens within the browser on the client side
        - In the MVC architecture, Angular would be the **View** component.
    - Node JS
        - back-end run-time environment for the web application
        - Express is built on Node js to simplify operations that may be complicated in the basic Node js code.
        - Therefore, the underlying event-driven code that you will be writing is Node JS

        ![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%206.png)

### MERNStack

- Same structure as the MEANStack but **the front-end framework is different.**
- The front-end of MERN stacked applications are made with **React JS instead of Angular JS.**

![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%207.png)

## Isomorphic frameworks vs software stacks

- Meteor JS vs MEANStack
    - Meteor has a strong focus on ease of use and allows users to focus on development
        - MEAN, requires multiple components to be integrated manually
    - Meteor is a **full stack framework,** which means it has an inbuilt database.
        - MEANStack requres each component of the stack to be **intstalled, learned, and integrated manually.**
    - MEANStack is more **flexible**
        - Meteor has a stringent limitation on what technologies are being used.
        - This means that, apps that have highly customized specs, MEANStack is more appropriate.
    - MEANStack doesn't have reactivitiy like Meteor. Additional technologies need to be integrated to client's web pages to be updated automatically.

# Version Control with Git

## The Command Line Interface

- **ls** - listing files and directories
- **pwd** - checking what directory you are in
- **cd** - changing directories
- **cd ..** — to move back a directory
- **cat nameOfFile** — reading files
- **touch nameOfFile** — creating files
- **mkdir newFolder** — creating a new directory
- **mv path/to/file/filename new/path** — moving files
    - **mv path/to/file/filename .** —  moves file to the current directory
    - **mv path/to/file/filename ..** — moves file to the parent directory
- **rm fileName** — removing files
- **git diff fileName** - can be used to check the differences between the working directory and staging area

## What is Git and Why Use it?

- Git is the world's popular version control system
- **History**
    - Git maintains a complete history of changes made to any project
- **Collaboration**
    - Git manages changes and merges them for the users allowing team members to work on projects simultaneously.
- **Feature branches**
    - Git has the ability to make separate branches for each feature & can be worked on simultaneously and when done, it can be **merged back to the main branch**

## Using Git Locally

### Git Jargon

- **Repository**
    - a project is a repository
- **Working** **Directory**
    - the folder **on your local computer where your project exists**
    - Git tracks any changes made within the folder
- **Commit**
    - Git doesn't save any changes until you 'commit' it.
- **Staging**
    - Staging a file means that you have marked it for a commit.

### Setting up and starting a new Git repo

- To mark a directory as a Git working directory:

        **git config** --global user.email "you@example.com"

        **git config** --global user.name "Your Name"

        **git init**

- **git status** can be used to view all the changes in your working directory
- To add new files to the staging area:
    - **git add** folder/that/contains/files
- To commit the file:
    - **git commit -m** "a message to commit with"
- To check commit history:
    - **git** log
- The -q can be used to make the console output less cluttered
    - **git init -q**
- Reverting to a previous commit
    - **git checkout hashvalue**

## Repo Hosting

- repo hosting allows your to work on your project even if you lost your local machine
- GitHub is an example of repo hosting

### Creating a GitHub repo from an existing Git repo

- Once you create a new repository in GitHub.
- Open terminal and change your directory to an existing Git repo
- On the top of your GitHub repository's Quick Setup page, click & copy the remote repository URL
- Add the URL like this:

![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%208.png)

- **Then push your changes in your local repository to Github:**

![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%209.png)

- A branch:
    - It's a parallel version of a repo. It's contained within the repo but doesn't affect the primary or master branch, allowing you to work freely without disrupting the "live" version.
    - When you're ready you can merge the branch back to the master branch
- A **pull request** is a proposed change to the repo submitted by a user & needs to be reviewed, and accepted or rejected by the other collaborators.
    - Once **approved**, it can be *merged with the master branch or other branches*

    ![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%2010.png)

# Principles of Software Engineering

## Software Process Models

- The four fundamental software engineering activities:
    1. Software specification
        - define the intended functionality of the software and potential constraints
        - example for a web application, here is where you define the features you want to implement on your website
    2. Software design and implementation
        - Producing software according to the specifications
    3. Software Validation
        - Ensuring the software does what users want it to do
        - You want to make sure the features are implemented correctly
    4. Software Evolution
        - Ongoing stage, where you continuously come up with features that you think **will make your application better & implement them**

    ![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%2011.png)

    - All process models can be categorized as:
        1. Plan-Drive
            - all process activities are planned in advance

            ![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%2012.png)

        2. Agile
            - Planning is incremental
            - Easier to change the process in accordance with changing customer requirements

            ![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%2013.png)

    ## The Waterfall Model (Plan-Driven Process)

    - First published model of the software development process.

    ![](https://github.com/PravinSelva5/Web_Development_Primer/blob/master/Web%20Development%20a%20Primer%20/Untitled%2014.png)

    - There are multiple stages involved and each stage must be completed before the next one
    - The 5 stages are:
        1. Analyze and define requirements
            - system's intended services, potential constraints, and goals are established & defined in detail
                - These requirements serve as a product specification
        2. Design software
            - taking the requirements realized in the previous stage and allocating it to different software components.
            - Overall system architecture is established
            - Identify and describe the fundamental software system abstractions & relationships amongst them
        3. Implement and test units
            - Software design is translated to a set of programs or multiple program units
            - Unit testing is used to make sure each unit meets its specifications
        4. Integrate units and test system
            - Program units are integrated & tested as a complete system
            - After testing, the software is delivered to the client
        5. Operation and maintenance
            - Not necessary but typically the longest stage in the life cycle
            - Correcting new errors, improving the implementation of system units, and **enhancing the system's services.**

## Incremental Development

- Interleaving the activities of specification, development, and validation
- System is developed as a series of versions/increments (each version will have more features than the previous)
- An example would be creating an initial version of your website, open it to feedback, and then incrementally developing newer versions based on feedbacks
- It's a more intuitive way of solving problems
- Benefits compared to the waterfall method:
    1. Cost of accommodating changing customer requirements diminishes as the amount of documentation that has to be redone is much less
    2. Easier to get customer feedback on the development work
    3. More rapid delivery and deployment of useful software to the customer is possible

## Reuse-oriented Software Engineering

- Reduced actual development significantly
- Faster product delivery
- However, requirements will change over time and as a result, the software being developed may not be as flexible to future requirements
- Most prevalent approach right now

## Test Driven Development

- Testing and code development are interleaved together.
- You don't move to the next increment until the **code that you have developed passes its test**

## Automated Testing

- Core idea  is to simultaneously develop automated tests with each increment & ensure the tests are passed.
- APIs can be used to create automated tests
- **Selenium** is one of the most commonly used tools for web application testing
    - primary purpose is to automate browsers
    - allows us to check if the intended functionality works by **automatically accessing the application**
    - it allows users to define a set of activities for a web browser to carry out
- **Jest,** a javascript tool that is often used by Facebook to test all of its Javascript code (incl. React).
- **PyUnit** is the python unit testing framework. A **unit test targest a small unit of code.**
    - supports test automation, share test setups & shutdown code for tests, aggregation of tests into collections, **also able to keep tests independent from the reporting framework**
- **JUnit** is the **Java** equivalent of PyUnit.
