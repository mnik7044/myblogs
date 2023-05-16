---
title: "API Chronicles S01E01"
datePublished: Sat Apr 15 2023 12:59:11 GMT+0000 (Coordinated Universal Time)
cuid: clghzis63000209l4hejqe0cf
slug: api-chronicles-s01e01
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1681553768520/3c05879b-c451-42ed-ba90-8dfae0545651.png
tags: web-development, databases, apis, webdev, wemakedevs

---

## Introduction

Have you ever wondered how different apps and services communicate with each other? How does your ride-sharing app know your location and how to navigate to your destination? Or how does your online store process your payment securely? The answer lies in APIs, or Application Programming Interfaces.

In this blog post, we'll start with the basics of APIs and how they work. We'll then explore the different types of APIs and their architecture. We'll also cover key concepts such as accessibility, CRUD operations, HTTP request methods, response status codes, and the request-response pattern.

By the end of this blog post, you'll have a better understanding of APIs. So, grab a cup of coffee, and let's dive into the world of APIs!

## What is this API?

Having API is like having a universal translator that can make your app speak the same language as other apps. Or like having a superhero sidekick that can do all the heavy lifting while you focus on being the hero.

For example, what if you had to manually process every credit card payment that came through your website? That would be a nightmare! But with payment gateway APIs, you can let the computer do the hard work while you sit back and enjoy the sound of money flowing into your bank account.

APIs are interfaces that allow different software applications to communicate with each other. APIs make it possible for developers to access specific data or functionality of another application without needing to understand the complexities of the codebase. APIs essentially provide a way to interact with an application without needing to understand how it works internally.

In short, APIs are the glue that holds the internet together, and without them, we'd be lost in a sea of disconnected applications.

## Client -Server & Network

APIs are typically built with the client-server model. Go through the image below for a better understanding

![Client-Server Network model](https://cdn.hashnode.com/res/hashnode/image/upload/v1681557805653/08777f62-3e47-4169-98ed-0cadff78d39a.png align="center")

* **Client-** In the world of APIs, the client would be the browser/application or service that is requesting data or functionality. If we consider the credit card analogy which we used earlier then the client would be the person using the credit card to make a purchase.
    
* **Server-** Now if we consider the world of APIs, the server would be the API provider that processes the request and sends back a response. And again from the credit card analogy, the server would be the merchant's point of sale system that processes the transaction and sends the payment to the bank.
    
* **Network-** In the world of APIs network would be the infrastructure that connects the different components, such as the internet, the API gateway, and the database or backend system that provides the data or functionality. Again from the credit card analogy, the network would be the infrastructure that connects all the different components, such as the payment gateway, the bank's processing system, and the merchant's point of sale system.
    

## Types Of APIs

1. **Hardware API**: A hardware API, also known as a device API, is a type of API that allows developers to access and control hardware devices such as sensors, cameras, and microphones. They provide the interface for software to talk to the hardware. A perfect example of the same would be a phone's camera talking to the OS.
    
2. **Software Library API**: A software library API, also known as a local API, is a type of API that provides access to a software library or toolkit. It is an interface for directly consuming and using codes from other codebases. A perfect example of that would be, Windows API which provides access to the Windows operating system functions and features.
    
3. **Web API**: A web API, also known as a remote API or REST API, is a type of API that allows communication between different software applications over the internet. Provides an interface for communicating code from another code base across a network. A perfect example of that would be fetching stock prices from finance APIs.
    

We can even use multiple APIs together to get our tasks done. An example would be uploading a photo on your Instagram account. Wonder how?

<mark>Hardware APIs</mark> for the application to talk to your camera.

<mark>Software Library APIs</mark> for images to be processed using filters.

<mark>Web APIs</mark> for sending it to Instagram's server.

## Accessibility

* **Public APIs-** APIs that can be consumed by anyone who discovers it.
    
* **Private APIs**\- APIs that can be consumed only within an organization and not made public.
    
* **Partner APIs**\- APIs that can be consumed between one or more organizations, they need to have an established relationship for that.
    

## CRUD Operations

In the context of APIs, CRUD is an acronym that stands for <mark>Create, Read, Update, and Delete</mark>.

Here's what each of these operations means:

* **Create:** This operation involves adding a new record or object to the database. For example, in a social media app, this might involve creating a new user profile.
    
* **Read:** This operation involves reading the data from the databases. For example, in an e-commerce app, this might involve retrieving a list of products or the details of a specific order.
    
* **Update**: This operation involves modifying an existing record or object in the database. For example, in a project management app, this might involve updating the status of a task.
    
* **Delete:** This operation involves removing a record or object from the database. For example, in a messaging app, this might involve deleting a message from a user's inbox.
    

## API Requests

We can use the CRUD operation to create our first API request, you can use [Postman](https://www.postman.com/downloads/) to send your API requests.

To create our API request we need a Request method to make an HTTP call to a server, when we do so we use a Request method to indicate the types of operation we are about to perform. These are called <mark>HTTP verbs.</mark>

Some Request methods are listed below:

| Name of the Request Method | Operation performed |
| --- | --- |
| <mark>GET</mark> | READ |
| <mark>POST</mark> | CREATE |
| <mark>PUT/PATCH</mark> | UPDATE (<mark>Put for entire resource, Patch for partial updates)</mark> |
| <mark>DELETE</mark> | DELETE |

### Request URLs

With request methods, we need request URLs this request URL says where to make the call.

There are three parts of a Request URL:

1. **Protocol-** <mark> (HTTP/HTTPS)</mark>
    
2. **Host-** It is the location of the server.
    
3. **Path-** Route on the server.
    

## Response Status Code

Response Status codes are indicators of whether a request succeeded or failed.

Ever seen the error 404 messages? In the table given below, you will know the cause of it.

| Code Range | Meaning |
| --- | --- |
| 2xx | <mark>Success</mark> |
| 3xx | <mark>Redirection</mark> |
| 4xx | <mark>Client Error</mark> |
| 5xx | <mark>Server Error</mark> |

So yes your <mark> Error 404</mark> is because of the Client Error. It might be because of a bad request.

Here is a response I got, when I send my first API request using Postman.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681562331060/700e3b4c-2a8f-40ca-8ddb-04205c459f67.png align="center")

## Conclusion

In conclusion, APIs are like magic wands for developers allowing them to create complex applications by integrating different systems and services with ease. Whether it's a hardware API, a software library API, or a web API, many different types of APIs can be used to achieve your development goals.

Of course, there are many things to know about APIs, such as how they work, how to use them, and how to work with different types of APIs. But don't worry, that's for the next episodes of this season! In the meantime, just remember that APIs are powerful tools that can help you create amazing applications and solve complex problems with ease.

Go forth and explore the wonderful world of APIs!

Let's end a blog with a meme:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1681563427248/2c46deb4-207d-464e-9c26-590fba329208.png align="center")

## Let's Connect

If you enjoyed this post and would like to stay updated on my work, feel free to connect with me on social media

* LinkedIn: Click [**here**](https://www.linkedin.com/in/nikhil-mishra-8a6710244)
    
* Github: Click [**here**](https://github.com/mnik7044)
    
* Twitter: Click [**here**](https://twitter.com/nikktwts?t=WxH0im12f-NtbUJGeV2Xsw&s=09)
    

I'm always open to new connections and networking opportunities, so don't hesitate to reach out and say hello. Thank you for reading!