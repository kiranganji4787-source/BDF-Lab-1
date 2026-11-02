# Lab 01: Node.js and Express Server

**Student Name:** Bolla Pradhyumna
**Registration Number:** 252U1R5027
**Section:** CSE-AIDE-2A
**Course:** Backend Development Fundamentals

## Deployment and Repository Links

**Live Application (Render):**  https://pradhyumna-lab-1.onrender.com/


**GitHub Repository:**
[https://github.com/bollapradhyumna1409-collab/Pradhyumna_Lab_1](https://github.com/bollapradhyumna1409-collab/Pradhyumna_Lab_1)

The Express application is developed using Node.js and Express.js. The application contains multiple routes that return text, JSON, date and time information, and a 404 response for undefined routes.

## 1. Aim

To create a basic web server using Node.js and learn how to build, manage, and test routes using Express.js.

## 2. Introduction

Node.js is a JavaScript runtime environment that allows JavaScript code to execute outside a web browser. It provides built-in modules such as the `http` module, which can be used to create web servers.

Express.js is a web framework built on Node.js that simplifies server development, routing, and HTTP request handling.

In this lab, I created a basic HTTP server using Node.js and then developed an Express application with multiple routes.

The application displays a welcome message, returns student details in JSON format, provides the current date and time, and handles undefined routes using a 404 response.

## 3. Technologies and Tools Used

- **Node.js:** Used to execute JavaScript code on the server.
- **Express.js:** Used to create the web server and define application routes.
- **JavaScript:** Used to implement server-side logic.
- **npm:** Used to initialize the project and manage dependencies.
- **Visual Studio Code:** Used to write and manage source code.
- **Git:** Used for version control.
- **GitHub:** Used to store and manage the project source code.
- **Render:** Used to deploy the Express application.

## 4. Project Structure

```text
Pradhyumna_Lab_1/
│
├── basic-server.js
├── app.js
├── server.js
├── package.json
├── package-lock.json
├── .gitignore
├── README.md
│
└── screenshots/
    ├── lab_home.png
    ├── lab_about.png
    ├── lab_time.png
    └── lab_unknown.png
```

### File Descriptions

- `basic-server.js` – Contains the basic HTTP server created using Node.js.
- `app.js` – Contains the Express application and route definitions.
- `server.js` – Starts the Express application.
- `package.json` – Stores project information, scripts, and dependencies.
- `package-lock.json` – Records the resolved versions of installed dependencies.
- `.gitignore` – Specifies files and folders that should not be tracked by Git.
- `README.md` – Contains project documentation and execution instructions.
- `screenshots/` – Stores screenshots of the tested application endpoints.

The `node_modules/` directory contains the installed packages required by the application. It is excluded from GitHub because the dependencies can be installed again using `npm install`.

## 5. Installation and Execution

### Prerequisites

- Node.js installed
- npm available
- Visual Studio Code or another code editor

### Step 1: Clone the Repository

```bash
git clone https://github.com/bollapradhyumna1409-collab/Pradhyumna_Lab_1.git
```

### Step 2: Navigate to the Project Directory

```bash
cd Pradhyumna_Lab_1
```

### Step 3: Install Dependencies

```bash
npm install
```

### Step 4: Run the Basic Node.js Server

```bash
node basic-server.js
```

Open the following address in your browser:

```text
http://localhost:3000
```

The browser displays the welcome message returned by the basic Node.js server.

Stop the server by pressing `Ctrl + C` before starting the Express server.

### Step 5: Run the Express Server

```bash
npm start
```

Alternatively:

```bash
node app.js
```

The Express server starts on port 3000.

Open:

```text
http://localhost:3000
```

Keep the terminal running while testing the application routes.

## 6. API Endpoints

The Express application contains the following GET routes:

| HTTP Method | Endpoint | Description                              | Status        |
| ----------- | -------- | ---------------------------------------- | ------------- |
| GET         | `/`      | Displays a welcome message               | 200 OK        |
| GET         | `/about` | Returns student name and section in JSON | 200 OK        |
| GET         | `/time`  | Returns current date and time            | 200 OK        |
| GET         | `/test`  | Demonstrates an undefined route          | 404 Not Found |

The application also returns a 404 response for other undefined routes.

### Local Endpoint URLs

- Home: [http://localhost:3000/](https://pradhyumna-lab-1.onrender.com/)
- About: [http://localhost:3000/about](https://pradhyumna-lab-1.onrender.com/about)
- Time: [http://localhost:3000/time](https://pradhyumna-lab-1.onrender.com/time)
- Not Found: [http://localhost:3000/test](https://pradhyumna-lab-1.onrender.com/unknown)

### Live Endpoint URLs

Replace the deployment URL below with your actual Render URL.

- Home: `YOUR_RENDER_URL/`
- About: `YOUR_RENDER_URL/about`
- Time: `YOUR_RENDER_URL/time`
- Not Found: `YOUR_RENDER_URL/test`

## 7. Screenshots and Testing Results

The following screenshots demonstrate the responses received while testing the Express application.

### 7.1 Home Route

Displays the welcome message returned by the Express server.
<img width="1917" height="955" alt="lab_home" src="https://github.com/user-attachments/assets/9a7d458a-1bc2-4144-9fbf-42fb227b99db" />



### 7.2 About Route

Displays the student's name and section in JSON format.

<img width="1917" height="960" alt="lab_about" src="https://github.com/user-attachments/assets/1132df27-5fa7-4d5e-a8f9-a353c80aded0" />




### 7.3 Time Route

Displays the current date and time generated using JavaScript's `new Date()` method.

<img width="1911" height="1043" alt="lab_time" src="https://github.com/user-attachments/assets/ee44f4c2-ce96-473b-a14a-a684243ef3f8" />


### 7.4 Unknown Route

Displays the 404 error message when an undefined route is accessed.

<img width="1917" height="952" alt="lab_unknown" src="https://github.com/user-attachments/assets/4c7b92ea-109a-44f3-b670-054925edc04e" />


## 8. Understanding package.json and node_modules

### package.json

Contains project information, including the project name, version, scripts, and dependencies. It defines the command used to start the Express server.

### package-lock.json

Records the resolved versions of installed dependencies to help maintain consistent installations.

### node_modules

Contains Express.js and other installed packages required to run the application.

This directory is excluded from GitHub because the dependencies can be recreated using:

```bash
npm install
```

## 9. Learning Outcomes

By completing this lab, I learned how to:

- Initialize a Node.js project using `npm init -y`.
- Install Express.js and manage dependencies using npm.
- Create a basic server using the built-in Node.js `http` module.
- Build an Express application and define GET routes.
- Handle HTTP requests and send text and JSON responses.
- Generate the current date and time using JavaScript's `new Date()` method.
- Handle undefined routes using HTTP status code 404.
- Test server responses through a web browser.
- Deploy a Node.js and Express application using Render.
- Store and manage project files using Git and GitHub.

## 10. Conclusion

Through this lab, I gained practical experience in creating web servers using Node.js and Express.js.

I learned how to define routes, send different types of responses, and handle requests to undefined URLs. Testing the endpoints helped me understand how HTTP status codes indicate the results of client requests.

Deploying the application on Render provided practical experience in making a backend application accessible through a public URL.

Overall, this lab helped me develop a foundation in backend development, server-side programming, and application deployment.

