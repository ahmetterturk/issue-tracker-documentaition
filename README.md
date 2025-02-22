# Final Assignment T3A2-A

- Ahmet Erturk
- Arturo Caceres
- Mohammad Reza Fayazi

# Lock Security

---

# R1 - Description of website

## Purpose

Lock security is a security company that offers various services to clients. These services include providing security officer assistance to small and enterprise companies, on-site patrolling in specialized worksites, security monitoring and screening for specific areas such as airports and shopping centres, etc. The company has the obligation to run flawless and smooth operations. As a company, they must ensure and maintain trust and rapport with their clients. To achieve this, they need to have exceptional communication within their operations. However, running a security company with multiple clients and employees is not always a smooth sail. They run into issues on a regular basis concerning both parties of the operation. Some examples to these issues could be;

- Security officer calling in sick an hour before their shift
- Security officer has an emergency and has to leave the jobsite ASAP
- Client does not want to work with the security officer
- Security officer does not show up to worksite
- Security officer falls asleep on the job
- Client without notification, needs more security officers

The purpose of this application is to provide a software platform for the security company to manage all their issues effectively. This application aims to provide issue tracking of operations to be managed in a way that is convinient and time efficient.

## Functionality / Features

### Authentication

The application has an authentication system where users need to sign in to the program to perform tasks and contribute to issues. This functionality provides features to handle actions, that require users to be identified when creating issues, contributing to issues, making comments and reviews, creating and editing personal accounts.

### Authorization

Authorization system, allows protect the management of issues and handling access to personal profiles. The authority to manipulate issues will only belong to users which the issue was posted by, or the administrator of the application. The authority to update details on user's profiles also belong to either the user itself or the administrator.

### Issue Feature

Users are able to create issues after being authenticated to use the application. Users can be added and removed from the issue tickets regarding the needs. Issues have statuses such as resolved and ongoing, private and public. Issues have a priority preference that determines which issue needs to be attented in what urgency.

### Communication

The application has a messaging system in the issue tickets where users can communicate with other users. This option will allow users to leave comments about any particular subject.

### Visual Data Display

The application visualizes statistics that are an outcome of the issue management. The program visualizes statuses of issues which are new, pending or resolved. It visualizes the amount of issues posted by frequency and it also uses visual representation of issues according to priority.

### Administrator

The application has an admin feature where the user who is given admin status has the authority and privileges to view and modify everything that is going on throughout the application.

### Roll Managament

Users in the program can have different roles assigned to them by the admin users.

## Target audience

The target audience of this application is the collective group of employees and managers in the Lock Security company. Personnel should be able to effectively use the application and contribute to issues posted.

## Tech stack

- Backend

  - **Node** - JavaScript runtime built on Chrome's V8 JavaScript engine.
  - **Express** - Express is a backend web application framework for Node.js
  - **mongoose** - Mongoose is a MongoDB object modeling tool designed to work in an asynchronous environment.

- Frontend

  - **React** - React is a front-end JavaScript library for building user interfaces based on UI components.
  - **JavaScript** - JavaScript is a high-level, interpreted programming language that conforms to the ECMAScript specification.
  - **HTML** - HTML is the standard markup language for Web pages.
  - **CSS** - CSS is the language used to style an HTML document.
  - **material ui** - MUI provides a simple, customizable, and accessible library of React components.

- Database

  - **MongoDB** - MongoDB is a source-available cross-platform document-oriented database program.

- Testing Libraries

  - **Jest** - JavaScript testing framework.
  - **Cypress** - JavaScript testing framework.

- External Services

  - **Firebase Authentication** - Firebase Authentication provides authentication for backend services.
  - **Heroku** - Heroku is a platform as a service that enables developers to operate applications in the cloud.
  - **Netlify** - Hosting and serverless backend services for web applications and static websites.
  - **AWS S3** - Service that provides object storage through a web service interface.

- Node Packages

  - **React Router** - Routing library for the React.
  - **Axios** - Promise based HTTP client for the browser and node.js

- Version Control

  - **Git** - Software for tracking changes in any set of files, usually used for coordinating work collaboratively developing source code.
  - **Github** - Hosting for software development and version control using Git.

- Tools

  - **Trello** - Trello is a web-based, Kanban-style, list-making application.
  - **Figma** - Web-based, vector graphics editor and prototyping tool.

---

# R2 - Dataflow Diagram

![alt text](docs/images/DFD.png)

---

# R3 - Application Architecture Diagram

![alt text](docs/images/AAD.png)

<hr/>

# R4 - User Stories

### **User Personas**

![alt text](docs/images/wireframe-imgs/personas.png)

### MVP for Employee

### **Employee**

<br>

- Ronald would like to have a safe authentication system within the application.
  - As an employee, I want to be able to log in to my account when I need to use the application and log out safely after I am done using it.
    <br>
    <br>
- Ronald would like to have access to his account for updating his details.
  - As an employee, I want to be able to update my details, after I have successfully signed into the application.
    <br>
    <br>
- Ronald would like to report an issue if there is one while his on duty.
  - As an employee, I want to be able to publish an issue when I come across a problem so that the managers could be notified and the issue could be addressed.
    <br>
    <br>
- Ronald would like to see a comment from management first on the issue he has published.
  - As an employee, I would like to be able to check comments which have been added by management so that I can reply to the comments.
    <br>
    <br>
- Ronald would like to prioritize any problem he reports.
  - As an employee, I want to be able to set the priority status of my issue, because there might be some urgent issues that need to be prioritized.
    <br>
    <br>
- Ronald would like to have an option to set his issue either to public or private. He might have sensitive information which he does not want to share with other employees.
  - As an employee, I want to be able to set the status of my issue to either public or private, because I might not want to share the details of some problems with every employee.
    <br>
    <br>
- Ronald would like to have an option to modify the issue he reports if there is any typo or misinformation.
  - As an employee, I want to be able to edit my issue, as I could have made a typo or would like to add missing information to my issue.
    <br>
    <br>

#### Possible Extension for Employee

- Ronald would like to tag other employees (s) to the existing issue, as they might be able to help to solve the problem, or have gone through something similar.
  - As an employee, I want to be able to add other participants to my issue ticket.
    <br>
    <br>
- Ronald would like to be assigned to other issues that he might be able to help resolve, to the existing problem for other employees
  - As an employee, I want to be able to participate in resolving issues that are made available to me.
    <br>
    <br>
- Ronald would like to add comments on others employees' issues that he might have a possible solution to.
  - As an employee, I want to be able to see the comments posted by other employees on issue tickets, as I might have gone through a similar situation, and might be able to help resolve the issue.
    <br>
    <br>
- Ronald would like to have access to the comments so he can share his opinion on the existing problem.
  - As an employee, I want to be able to reply to comments posted by other employees on issue tickets, so I can contribute to solving the problem.
    <br>
    <br>
- Ronald would like to be able to see other issues if they are visible to him.
  - As an employee, I want to be able to view the issues that are made available to me.
    <br>
    <br>
- Ronald would like to be notified if he has been assigned to an issue.
  - As an employee, I want to receive a notification when I am tagged on an issue ticket, so I can see it or reply if needed.
    <br>
    <br>

### **Admin**

- Leslie would like to have full control over the application as an Admin, as she is a manager at Lock Security.
  - As an admin, I want to be able to have an admin role, so that I can manage Employee information.
    <br>
    <br>
- Leslie would like to create an account for an employee and give them their login details so that they can sign in to the application. As a manager, she is responsible for creating an account for employees' use on the platform.
  - As an admin, I want to be able to create an account for the employee, so they can have access to the application with their account details.
    <br>
    <br>
- Leslie would like to check and view all the issues after they have been published so that she can keep track of them.
  - As an admin, I want to be able to view all issues regardless of their status, whether they are resolved, in progress, or new.
    <br>
    <br>
- Leslie would like to search through the issues, to find a specific issue she is looking for, instead of going one by one at a time.
  - As an admin, I want to be able to filter issues by either the date, name, priority, type, and status they were posted to find relative information faster.  
    <br>
    <br>
- Leslie would like to have access to updating and/or removing issues if it's needed. In the case a problem is resolved, for example, has a typo or there is no possible solution for the specific problem.
  - As an admin, I want to have the ability to update and delete all issues posted by employees.
    <br>
    <br>
- Leslie would like to have access to all the issues being published regardless of their status, as there might be some issues with private information.
  - As an admin, I want to be able to have access to issues with private status, as the employee may share sensible information.
    <br>
    <br>
- Leslie would like to see all different statuses for existing issues to keep better track of them.
  - As an admin, I want to be able to see how many employees published an issue, so that I can see new, pending, and resolved issues.
    <br>
    <br>
- Leslie would like to update the status of existing issues once they get resolved.
  - As an admin, I want to be able to update the status from new to either pending or resolved.
    <br>
    <br>
- Leslie would like to leave a comment on an existing issue, reply or delete them if it's needed.
  - As an admin, I want to have the ability to update and delete all comments made on issues by employees so employees.
    <br>
    <br>

#### Possible Extension for Admin

- Leslie would like to see all issues represented on graphs as a visual aid, so that she can keep track of issues being published weekly, monthly, or yearly, depending on their status, priority, or type.
  - As an admin, I want to be able to access visual charts that represent statistics of issues.
    <br>
    <br>

<hr/>

# R5 - Wireframes for multiple standard screen sizes, created using industry standard software

## Navigation of application

On the following images below we have mapped out navigation flow of each page of the application from the start point which is a login page.

![alt text](docs/images/wireframe-imgs/admin-navigation-view.png)
![alt text](docs/images/wireframe-imgs/employee-navigation-view.png)

### Admin Wireframe

- Login page
  ![alt text](docs/images/wireframe-imgs/loginpage.png)
- Dashboard page
  ![alt text](docs/images/wireframe-imgs/dashboardpage.png)
- Tickets page
  ![alt text](docs/images/wireframe-imgs/ticketpage.png)
- View ticket page
  ![alt text](docs/images/wireframe-imgs/SingleTicket.png)
- Create a new ticket page
  ![alt text](docs/images/wireframe-imgs/CreateNewTicket.png)
- List of employees page
  ![alt text](docs/images/wireframe-imgs/listofemployee.png)
- Create account / Sign up page
  ![alt text](docs/images/wireframe-imgs/Createaccount.png)
- Graph and statistic page
  ![alt text](docs/images/wireframe-imgs/graphpage.png)

### Employee wireframes

- Dashboard page
  ![alt text](docs/images/wireframe-imgs/employeedashboard.png)
- Create ticket page
  ![alt text](docs/images/wireframe-imgs/employeenewticket.png)
- View ticket page
  ![alt text](docs/images/wireframe-imgs/employeeviewticket.png)
- Edit account / profile page
  ![alt text](docs/images/wireframe-imgs/employeeeditprofile.png)

# R6 - Screenshots of your Trello board throughout the duration of the project

We decided to use Trello, as our project management tool to keep track of our group progress and assign tasks to each member of the group. <br>

Initially, we started at the planning phase, looking for the best idea to challenge us as junior developers. By using Trello, all cards must go through the following process to keep track of our features/tasks;

- Backlog
- To Do
- In progress
- On Hold
- Done

During this project, as a Team we will apply Scrum rituals, to succeed in delivering this application. With the use of Labels, Assign to Member options, Checklists, Dates and other Power-ups, we will be able excel on our project. <br>

This is a link to the project management tool [Trello](https://trello.com/b/OiNyPtJn/issue-tracker)

<hr>

### Day #1

![alt text](docs/images/trello-imgs/day1.png)

### Day #2

![alt text](docs/images/trello-imgs/day2.png)

### Day #3

![alt text](docs/images/trello-imgs/day3.png)

### Day #4

![alt text](docs/images/trello-imgs/day4.png)

### Day #5

![alt text](docs/images/trello-imgs/day5.png)

### Day #6

![alt text](docs/images/trello-imgs/day6.png)

### Day #7

![alt text](docs/images/trello-imgs/Day7.png)
