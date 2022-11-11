# Br Petshop API User Guide

## Introduction
>**Br Petshop** is an API that simulates a pet shop management server. The API allows you to access Petstore data using a set on individual calls.
>This User guide describes step by step how to use the <nomedaminhaapi> API. The purpose of this API is to exchange data between your system and the Swagger Petstore, most of the time these data exchanges have the objective to automate manual process and/or allow the creation of new functionalities.
## System Overview
>This API User Guide contains a React project that makes HTTP requests to the Swagger Petstore API, which is a Promise-based HTTP client for making request.
## React Axios
>Axios is a Promise based HTTP client for making requests. Can ben both in the browser and in Node.js or any API service. On this API User guide, we are going to create a React project that makes `HTTP requisitions` to the Swagger Petstore sample API using Axios.
## Characteristics
- Using ‘Ajax’ as a layer bellow, makes requisitions through the browser via XMLHttpRequests;
-	Makes HTTP requisition with Node.js;
-	Supports Promises;
-	Every answer will be transformed and returned in JSON;
-	It supports cross-site forgery request known as XRSF.
## Prerequisites
-	Noje.js running on your machine
- React Axios
## Installation and configuration
**Npm commands to install Node.js;**
1.	Type `npm nit` on your terminal or cmd(command prompt) then press Enter.
2.	Type `npm install –save <module-name>` on your terminal or cmd(command prompt) then press Enter.
3.	Run the JavaScript files with `node <filename.js>` on your terminal or cmd(command prompt) then press Enter.

>We need to access it and install the Axios package to integrate the HTTP requisitions and to consume the external API.
The installation of this package is very simple, just type the **command bellow** on your terminal.

![npm install axios](https://user-images.githubusercontent.com/45776133/201379999-7e0ddf36-e853-49a8-ab53-0747434567b5.jpg)

**Package installation.**

>After installation is completed, you already can use Axios on your project, we are going to create an application that consumes the Swagger Petstore sample API, and displays pet information data on the screen.


## Creating the file
>To better organize your project, create a file `<filename.js>`, which will be responsible for all the configuration and the Axios library import.
The page structure should look like this.
 
**Image. Page’s structure.**


## Get requisiton
>With this example, we are going to make a requisition using HTTP GET through the get() method. 
<Line 9> is returning the Pet id and Pet name data from Swagger Petstore.
 
**Code 5. Requisiton call.
## Code explanation:
**PRINT**

>Code execution.
 

**(PRINT execucao do codigo)**

## Requisition with POST
>The post() method makes requisition utilizing HTTP POST, as per Code6.
**(print)
Code 5. Requisition with post**
Here you can see on the third line, beyond the endpoint the second parameter is being passed to the post() method, which is an data object that are being sent to the API.
The difference between the get() method and post() method is;
The parameters will be sent through the HTTP request header, and in post() the parameters are sent through the body request.
The most common methods for HTTP request are: GET, POST, DELETE and PUT. For each method Axios has its own ‘method’ with the same name, as we see in code 7.
**(print)**


Code 5. Requisition examples.


## Conclusion


