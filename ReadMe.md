### Table of Contents

| No. | Questions                                                    |
| --- | ------------------------------------------------------------ |
|     | **Core React**                                               |
| 1   | [What is Module?](#what-is-module)                           |
| 2   | [What is Mongoose?](#what-is-mongoose)                       |
| 3   | [What is bind call and apply?](#what-is-bind-call-and-apply) |
| 4   | [What is promise?](#what-is-promise) |

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

3. ### What is bind call and apply?

   ```
   Bind- bind method takes an object as a first argument and creates a new function.

   Example: -

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


   Call:
   -  call method are predefined javaScript function.
   -  Call invokes the function and allows you to pass in arguments  one by one.

   Example:-

     const obj = {
       name: "manish",
       role: "admin",
       charater: function (char) {
           console.log(`He is ${this.name}. His role is ${this.role}. His character is ${char} `)
        }
      }

      const person = {
        name: "rabi",
        role: "customer"
     }

     obj.charater.call(person,"honest");

   Apply: it is similar to call , besides it takes the arguments as an array.

   Example:

       const obj = {
       name: "manish",
       role: "admin",
       charater: function (rating, char) {
           console.log(`He is ${this.name}. His role is ${this.role}. His character is ${char}. his rating is ${rating}`)
        }
     }

       const person = {
           name: "rabi",
           role: "customer"
       }

     obj.charater.apply(person, [5, "honest"]);

   Defference:

   call : binds the this value, invokes the function, and allows you to pass a list of arguments.

   apply : binds the this value, invokes the function, and allows you to pass arguments as an array.

   bind : binds the this value, returns a new function, and allows you to pass in a list of arguments.

   ```

   **[⬆ Back to Top](#table-of-contents)**

1. ### What is Promise?
   The Promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting value.
   ```
        let promise = new Promise(function(resolve, reject) {
        // executor (the producing code, "singer")
        if(resolve){
            console.log("Done!")
        }
        else{
            console.log("Not Done");
        }
        });
   ```
   **[⬆ Back to Top](#table-of-contents)**