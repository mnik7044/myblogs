---
title: "Building Your First Web Server Using NodeJs"
seoTitle: "Building HTTP web server using nodejs"
seoDescription: "Learn how to build an HTTP web server using Node.js - Step-by-step guide to creating a powerful server for your website."
datePublished: Sat Jun 10 2023 23:04:44 GMT+0000 (Coordinated Universal Time)
cuid: cliqlt85d000709l68bjufalx
slug: building-your-first-web-server-using-nodejs
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1686399534769/e2270f45-9162-4419-b391-e706b568e86b.png
tags: javascript, web-development, nodejs, wemakedevs, devsintechblogs

---

## Introduction

In today's blog we will be building our first HTTP server so there is some prerequisite for this blog which is some <mark>basic knowledge of javascript, an understanding of syntaxes in javascript</mark>. Node.js has gained significant popularity in recent years as a powerful platform for building <mark>scalable and efficient backend applications</mark>. Whether you're a newbie or an aspiring full-stack web developer, learning Node.js opens up a world of possibilities for creating robust and high-performing web servers, APIs, and other backend services. In this beginner's guide, we'll walk you through the essentials of Node.js, providing code snippets and explanations that are easy to understand, even if you're just starting out.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686436997032/9483bd25-2dd7-49f2-85b6-d3007a8908a2.jpeg align="center")

## **What is Node.js?**

Node.js is a JavaScript runtime environment that allows you to execute JavaScript code on the server side, <mark>don't confuse it with a framework it is not a framework</mark>. It provides an event-driven, non-blocking I/O model(Asynchronous), making it efficient and lightweight for building scalable network applications. Node.js is commonly used to create web servers, APIs, and other backend services.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686436508598/f1c377e5-17cf-42c8-91ac-4be140ed3640.png align="center")

## Step-by-step instructions for installing Node.js and creating a new project

### **Install Node.js**

To begin, you'll need to install Node.js on your computer. Visit the official Node.js website ([**https://nodejs.org**](https://nodejs.org)) and download the installer for your operating system. Follow the installation instructions provided.

### **Create a new Node.js project**

Once Node.js is installed, open your terminal or command prompt and navigate to the directory where you want to create your project. Use the `mkdir` command to create a new folder for your project, and then navigate into that folder using the `cd` command.

### **Initialize a new Node.js project**

In the terminal, run the following command to initialize a new Node.js project:

```javascript
npm init
```

This command will prompt you to provide information about your project (e.g., name, version, description). You can press enter to accept the default values for most options. This will create a `package.json` file in your project folder, which keeps track of your project's dependencies and configurations.

### **Installing dependencies**

Node.js uses packages and modules to extend its functionality. You can install packages using the Node Package Manager (npm), which comes bundled with Node.js. To install a package, run the following command in your terminal:

```javascript
npm install <package-name>
```

Replace `<package-name>` with the name of the package, you want to install. For example, if you want to install the Express framework, you would run:

```javascript
npm install express
```

With these initial steps completed, you're ready to start building your Node.js application. Let's explore some code snippets to help you understand key concepts.

## **Creating a Simple Web Server**

One of the common use cases for Node.js is building web servers. Here's a basic code snippet to create a simple HTTP server using the built-in `http` module in Node.js:

```javascript
const http = require('http');

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hello, World!');
});

const port = 3000;
server.listen(port, () => {
  console.log(`Server running on port ${port}`);
});
```

In this example:

* We import the `http` module using the `require` function.
    
* We create a server using the `createServer` method, which takes a callback function with two parameters: `req` (the request object) and `res` (the response object).
    
* Inside the callback function, we set the response status code to 200 and the content type to `'text/plain'`. The line `res.setHeader('Content-Type', 'text/plain');` sets the `Content-Type` header of the HTTP response. The `Content-Type` header informs the client (usually a web browser) about the type of content being sent in the response.
    
    In this case, the content type `'text/plain'` indicates that the response body contains plain text. <mark>It is a simple format that represents textual data without any special formatting or styling. It's commonly used for plain text documents, such as the body of an email or a basic text file.</mark>
    
    By setting the `Content-Type` header to `'text/plain'`, the server informs the client that the response body will be plain text. <mark>This allows the client to interpret and display the content appropriately.</mark> For example, a web browser will typically display plain text directly to the user without any additional formatting.
    
    Other common `Content-Type` values include:
    
    * `text/html`: Represents HTML content, which is used to structure and present web pages.
        
    * `application/json`: Represents JSON (JavaScript Object Notation) content, commonly used for exchanging data between a server and a client.
        
    * `application/xml`: Represents XML (eXtensible Markup Language) content, often used for data exchange and document storage.
        
    
    Different `Content-Type` values are used to indicate different types of content, and they help the client understand how to handle and display the received data appropriately.
    
    In the provided code snippet, setting `Content-Type` to `'text/plain'` suggests that the response body will be plain text, and the client should handle it accordingly.
    
* Then we send the response with the message `'Hello, World!'`
    
* We specify the port number (3000 in this case) on which the server should listen for incoming requests using the `listen` method.
    
* Finally, we log a message to the console when the server starts running.
    

You can save this code in a file (e.g., `server.js`) and run it using the `node` command:

```javascript
node server.js
```

Now, if you visit [`http://localhost:3000`](http://localhost:3000) in your browser, you should see the "Hello, World!" message.

## **Handling HTTP Requests**

Let's extend our server to handle different routes and HTTP methods using the Express framework(<mark>we will learn about it more in the upcoming blogs</mark>). For now, just understand that express simplifies the process of building web applications in Node.js. Start by installing Express using the command mentioned earlier (`npm install express`).

```javascript
const express = require('express');
const app = express();

app.get('/', (req, res) => {
  res.send('Hello, World!');
});

app.get('/about', (req, res) => {
  res.send('About page');
});

app.listen(3000, () => {
  console.log('Server running on port 3000');
});
```

In this example:

* We import the Express module and create an instance of the `express` object.
    
* We define different routes using the `app.get` method, which corresponds to the HTTP GET method. In this case, we define a route for the root URL (`/`) and the `/about` URL.
    
* Inside each route's callback function, we use the `res.send` method to send a response to the client.
    
* We start the server on port 3000 using the `app.listen` method.
    

Save this code in a file (e.g., `server.js`) and run it using the `node` command. You can then visit [`http://localhost:3000`](http://localhost:3000) and [`http://localhost:3000/about`](http://localhost:3000/about) to see the respective responses.

These examples cover the basics of getting started with Node.js and building a simple web server using the built-in `http` module and the Express framework. There's much more to explore, such as working with databases, handling POST requests, and building APIs. As you progress, you can dive deeper into these topics and expand your Node.js knowledge.

## Conclusion

Congratulations! You've taken your first steps into the exciting world of Node.js. By now, you should have some understanding of how to set up a Node.js project, create a web server, and handle different routes and content types. Additionally, you should gain insights into asynchronous programming using callbacks, promises(Prolly our next blog), and `async/await` by referring to the previous blogs. Remember that this is just the beginning of your journey, and there's so much more to learn and explore in the Node.js ecosystem.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1686438029134/e68b9b7c-d99e-4202-926c-17c7b5a68588.jpeg align="center")

## **Let's Connect**

If you enjoyed this post and would like to stay updated on my work, feel free to connect with me on social media

* LinkedIn: Click [**here**](https://www.linkedin.com/in/nikhil-mishra-8a6710244)
    
* Github: Click [**here**](https://github.com/mnik7044)
    
* Twitter: Click [**here**](https://twitter.com/nikktwts?t=WxH0im12f-NtbUJGeV2Xsw&s=09)
    

If you find my blog helpful you all can always support me by sponsoring me!