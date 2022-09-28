### Table of Contents
| No. | Questions |
| --- | --------- |
|   | **Core React** |
|1  | [What is Module?](#what-is-module) |
|2  | [What is Mongoose?](#what-is-mongoose) |
|3  | [What is bind,call and apply?](#what-is-bind,-call-and-apply) |
## Core React
    

1. ### What is Module?
    A module in JavaScript is just a file containing related code. In JavaScript, we use the import and export keywords to share and receive functionalities
   **[⬆ Back to Top](#table-of-contents)**

2. ### What is Mongoose?
    Mongoose is a MongoDB object modeling tool designed to work in an asynchronous environment. Mongoose supports both promises and callbacks.  
    ```
    // Using Node.js `require()`
    const mongoose = require('mongoose');

    // Using ES6 imports
    import mongoose from 'mongoose';

    ```
   **[⬆ Back to Top](#table-of-contents)**

3. ### What is bind,call and apply?

    ```
    Bind- bind method takes an object as a first argument and creates a new function.


    const obj1={
        name:"manish",
        role:"admin"
    }

    const obj2={
        name:"rabi",
        role:"customer"
    }

    function printRoleandName(){
        console.log(`He is ${this.role}. his name is ${this.name}`)
    }
        
    const person1=printRoleandName.bind(obj1);
    const person2=printRoleandName.bind(obj2);

    person1();
    person2();
  

    ```
   **[⬆ Back to Top](#table-of-contents)**