# Br Petshop API User Guide
>**Br Petshop** is an API that simulates a pet shop management server. The API allows you to access Petstore data using a set on individual calls.
>This User guide describes step by step how to use the <nomedaminhaapi> API. The purpose of this API is to exchange data between your system and the Swagger Petstore, most of the time these data exchanges have the objective to automate manual process and/or allow the creation of new functionalities.

* [System-Overview](#system-overview)
* [React Axios](#react-axios)
* [Characteristics](#characteristics)
* [Prerequisites](#prerequisites)
* [Installation and configuration](#installation-and-configuration)
* [Code explanation](#code-explanation)
* [API endpoints](#api-endpoints)
* [Conclusion](#conclusion)

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

 
 ![image structure](https://user-images.githubusercontent.com/45776133/201383856-727fb071-b86c-42ba-8f9e-e2aa2fa9856b.JPG)

**Page’s structure.**

## Code explanation ##
 ![code explanation](https://user-images.githubusercontent.com/45776133/201384930-91681362-54b6-4d5d-a0e7-15a92db96545.JPG)

 
 `Line1` <sub>Requering the 'Axios library</sub>
 
`Line3` <sub>Using the get()method, to receive data, in this case, data from the Swagger Petstore API.
We pass it with the endpoint,that is, the URL with the path that will be requested withi the API.
//This path will be combined with the URL base that we defined earlier. At the end the request will be sent to https://petstore.swagger.io/v2/pet/findByStatus?status=available.</sub>

 `Line5` <sub>Using 'then' method to get the result and using 'res' variable to get the response</sub>

 `Line6` <sub>Getting the JSON data with 'res.data'</sub>

 `Line8` <sub>'Slicing up' my Array to get only 10 available pet</sub>

 `Line11` <sub>Printing out the Dog Id and Dog Name</sub>

 `Line15` <sub>In case of any error with the request, the catch()method will be responsible for handling and displaying the error.</sub>

 

**Data displayed**

 ![result](https://user-images.githubusercontent.com/45776133/201396640-e9029e04-3aed-4662-9132-1181aa87d160.JPG)

## API endpoints

<table>
 <table border="1">
   <thead>
   <tr>
       <th>Method 1</th>
       <th>Description 2</th>
   </tr>
   </thead>
   <tbody>
   <tr>
       <td>Get /pet/{petId}</td>
       <td>Method used to return the information of available pets.</td>
   </tr>
   <tr>
       <td>POST /pet</td>
       <td>Method used to create a new register, in this case, a new pet.</td>
   </tr>
   </tbody>
   <tfoot>
       <td>DELETE /pet</td>
       <td>Method used to remove a selected pet from the system.</td>
   </tfoot>
</table>

## Conclusion
Our API is using Axios,which is a library that allows integration from our project to the Swagger PetStore.
