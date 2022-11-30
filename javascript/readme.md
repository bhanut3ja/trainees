# JavaScript
- ### What is javascript?
     JavaScript is a scripting or programming language that allows you to implement complex features on web pages — every time a web page does more than just sit there and display static information for you to look at — displaying timely content updates, interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. — you can bet that JavaScript is probably involved. It is the third layer of the layer cake of standard web technologies, two of which (HTML and CSS) we have covered in much more detail in other parts of the Learning.
     
     <strong>Html</strong> is the markup language that we use to structure and give meaning to our web content, for example defining paragraphs, headings, and data tables, or embedding images and videos in the page.
     
     <strong>CSS</strong> is a language of style rules that we use to apply styling to our HTML content, for example setting background colors and fonts, and laying out our content in multiple columns.
     
     <strong>Javascript</strong> is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much everything else. (Okay, not everything, but it is amazing what you can achieve with a few lines of JavaScript code.)

    <img src="javascript/img/Picture1.gif">
   
    Let's look at some more specific uses of JavaScript in web development
     
     - <strong>Front-End Interactivity:</strong> Web development is only made better by the increased interactivity and features that JavaScript offers.
     - <strong>Web Applications:</strong> Web applications are similar to websites, but instead, they get packaged into a neat little box, which improves control over security and more.
     - <strong>Browser Games:</strong> The modern web browser has come a long way; developers even make robust games that function in a browser.
     - <strong>Back End Web Development:</strong> Web development has come a long way, and now JavaScript is so robust it can even be used to manage the back end of websites and web applications

    Here’s an illustration of all the possible use cases of JS today:
 
    ![image](https://user-images.githubusercontent.com/117704825/204896016-af814468-c2b5-46b4-a3a5-78678c2e3893.png)
     
- ### How does JavaScript work?   
     JavaScript is considered a client-side scripting language, which means that it operates on the user's browser and does not function on an external device. An example of a language that is not client-side would be MySQL, a server-side language that handles any database requests.
     
     JavaScript also does not require that anything be downloaded to the user's devices, as modern browsers have the required software integrated into them. This makes JavaScript much more user-friendly than some other languages can be.

  Execution of js –
     1. in browser ( open browser and inspect or console) 
     2. js can be run outside of browser using nodejs
     3. use < script> tag inside any html doc and run that html file

- ### Variables  –      
     
     There are some rules while declaring a JavaScript variable (also known as identifiers).
     1.Name must start with a letter (a to z or A to Z), underscore( _ ), or dollar( $ ) sign.
     2.After first letter we can use digits (0 to 9), for example value1.
     3.JavaScript variables are case sensitive, for example x and X are different variables.

- ### Local variable - 
     A JavaScript local variable is declared inside block or function. It is accessible within the function or block only. 
    
     For example:
     
      <script>  
      If(10<13){  
      var y=20;//JavaScript local variable  
      }  
      </script>  

- ### Global variable -      
     A JavaScript global variable is accessible from any function. A variable i.e. declared outside the function or declared with window object is known as global variable. 
     For example:
           
      <script>  
      var data=200;//gloabal variable  
      function a(){  
      document.writeln(data);  
      }  
      function b(){  
      document.writeln(data);  
      }  
      a();//calling JavaScript function  
      b();  
      </script>  

- ### VAR     
     Before the advent of ES6, var declarations ruled. There are issues associated with variables declared with var , though. That is why it was necessary for new ways to declare variables to emerge i.e. <strong>let</strong> and <strong>const.</strong>
     
- ### Let
     let is now preferred for variable declaration. It's no surprise as it comes as an improvement to var declarations. It also solves the problem with var that we can’t redeclare  a variable so that to resolve the overriding of variable value if not done knowingly.

     However, if the same variable is defined in different scopes, there will be no error:

      let greeting = "say Hi";
      if (true) {
      let greeting = "say Hello instead";
      console.log(greeting); // "say Hello instead"
      }
      console.log(greeting);//”Say hi”
     
- ### Const     
     Variables declared with the const maintain constant values. const declarations share some similarities with let declarations.   

      const greeting = "say Hi";
      greeting = "say Hello instead";// error: Assignment to constant variable. 

      nor this:
      
      const greeting = "say Hi";
      const greeting = "say Hello instead";// error: Identifier 'greeting' has already been declared

    ![image](https://user-images.githubusercontent.com/117704825/204896812-3f14da02-7053-4fdb-bb53-c2ba0babcb12.png)
     
- ### Data Types     
     There are eight basic data types in JavaScript. They are:
     
     | Data Types | Description | Example |
     |-----:|---------------|---------------|
     |1.String| represents textual data|'hello', "hello world!" etc|
     |2.Number|an integer or a floating-point number|3, 3.234, 3e-2 etc.|
     |3.Big Int|an integer with arbitrary precision|900719925124740999n , 1n etc.|
     |4.Boolean|Any of two values: true or false|true and false|
     |5.Undefined|a data type whose variable is not initialized|let a;|
     |6.Null|denotes a null value|let a = null;|
     |7.Symbol |data type whose instances are unique and immutable|let<br>value = Symbol('hello');|
     |8.Object|key-value pairs of collection of data|let student = { };|
     
     Here, all data types except Object are primitive data types, whereas Object is non-primitive.
     
     > Note: The Object data type (non-primitive type) can store collections of data, whereas primitive data type can only store a single data.     
     
- ### Template literals (Template strings)     
     Template literals are literals delimited with backtick (`) characters, allowing for multi line strings, string interpolation  with embedded expressions.
     
     Template literals are sometimes informally called template strings, because they are used most commonly , string interpolation  (to create strings by doing substitution of placeholders).
     
 - ### Syntax    
 
      `string text`

      `string text line 1`
      
      `string text line 2`
      
      `let expression = 2;`
      
      `string text ${expression} string text`
     
- ### Operators
     JavaScript operators are symbols that are used to perform operations on operands.
     For example:

     `1.	var sum=10+20;`

     Here, + is the arithmetic operator and = is the assignment operator.
     
     There are following types of operators in JavaScript.

    ![image](https://user-images.githubusercontent.com/117704825/204896938-30834dcb-6169-46ed-aa7d-dd38e2f72106.png)


- ### Arithmetic Operators     
     |Operator|Description|Example|
     |-----:|---------------|---------------|
     |  +  |Addition|10+20 = 30|
     |  -  |Subtraction|20-10 = 10|
     |  *  |Multiplication|10*20 = 200|
     |  /  |Division|20/10 = 2|
     |  %  |Modulus (Remainder)|20%10 = 0|
     |  ++  |Increment|var a=10; a++; Now a = 11|
     |  --  |Decrement|var a=10; a--; Now a = 9|

 - ### Comparison Operators    
     
     |Operator|Description|Example|
     |-----:|---------------|---------------|
     |  ==  |Is equal to|10==20 = false|
     |  ===  |Identical (equal and of same type)|10==20 = false|
     |  !=  |Not equal to|10!=20 = true|
     |  !==  |Not Identical|20!==20 = false|
     |  >  |Greater than|20>10 = true|
     |  >=  |Greater than or equal to|20>=10 = true|
     |  < |Less than|20<10 = false|
     |  <= |Less than or equal to|20<=10 = false|



- ### Bitwise Operators

     |Operator|Description|Example|
     |-----:|---------------|---------------|
     |  &  |Bitwise AND|(10==20 & 20==33) = false|
     |  |  |Bitwise OR|(10==20 | 20==33) = false|
     |  ^  |Bitwise XOR|(10==20 ^ 20==33) = false|
     |  ~  |Bitwise NOT|(~10) = -10|
     |  << |Bitwise Left Shift|(10<<2) = 40|
     |  >> |Bitwise Right Shift|(10>>2) = 2|
     |  >>> |Bitwise Right Shift with Zero|(10>>>2) = 2|
    
- ### Logical Operators

     |Operator|Description|Example|
     |-----:|---------------|---------------|
     |  &&  |Logical AND|(10==20 && 20==33) = false|
     |  ||  |Logical OR|(10==20 || 20==33) = false|
     |  !  |Logical Not|!(10==20) = true|



- ### Assignment Operators

     |Operator|Description|Example|
     |-----:|---------------|---------------|
     |  =  |Assign|10+10 = 20|
     |  +=  |Add and assign|var a=10; a+=20; Now a = 30|
     |  -=  |Subtract and assign|var a=20; a-=10; Now a = 10|
     |  *=  |Multiply and assign|var a=10; a*=20; Now a = 200|
     |  /=  |Divide and assign|var a=10; a/=2; Now a = 5|
     |  %=  |Modulus and assign|var a=10; a%=2; Now a = 0|
   
- ### Special Operators

     |Operator|Description|
     |-----:|---------------|
     |(?:)|Conditional Operator returns value based on the condition. It is like if-else.|
     |  ,  |Comma Operator allows multiple expressions to be evaluated as single statement.|
     |  delete  |Delete Operator deletes a property from the object.|
     |  In  |In Operator checks if object has the given property|
     |  Instanceof  |checks if the object is an instance of given type|
     |  New  |creates an instance (object)|
     |  Typeof  |checks the type of object.|
     |  Void  |it discards the expression's return value.|
     |  Yield  |checks what is returned in a generator by the generator's iterator.|

- ### String
     The <strong>JavaScript string</strong> is an object that represents a sequence of characters.
     |Methods|Description|
     |-----:|---------------|
     |charAt()| It provides the char value present at the specified index.|
     |charCodeAt()|It provides the Unicode value of a character present at the specified index.|
     |concat()|It provides a combination of two or more strings.|
     |indexOf()|It provides the position of a char value present in the given string.|
     |lastIndexOf()|It provides the position of a char value present in the given string by searching a character from the last position.|
     |search()|It searches a specified regular expression in a given string and returns its position if a match occurs.|
     |match()|It searches a specified regular expression in a given string and returns that regular expression if a match occurs.|
     |replace()|It replaces a given string with the specified replacement.|
     |substr()|It is used to fetch the part of the given string on the basis of the specified starting position and length.|
     |substring()|It is used to fetch the part of the given string on the basis of the specified index.|
     |slice()|It is used to fetch the part of the given string. It allows us to assign positive as well negative index.|
     |toLowerCase()|It converts the given string into lowercase letter.|
     |toLocaleLowerCase()|It converts the given string into lowercase letter on the basis of host?s current locale.|
     |toUpperCase()|It converts the given string into uppercase letter.|
     |toLocaleUpperCase()|It converts the given string into uppercase letter on the basis of host?s current locale.|
     |toString()|It provides a string representing the particular object.|
     |valueOf()|It provides the primitive value of string object.|
     |split()|It splits a string into substring array, then returns that newly created array.|
     |trim()|It trims the white space from the left and right side of the string.|

- ### Conditional Statements

     - if Statement
     
      if (condition) {
      //  block of code to be executed if the condition is true
      }

     - if else Statement
     
      if (condition) {
      //  block of code to be executed if the condition is true
      } else {
      //  block of code to be executed if the condition is false
      }

     - else if Statement 
    
      if (condition1) {
      //  block of code to be executed if condition1 is true
      } else if (condition2) {
      //  block of code to be executed if the condition1 is false and condition2 is true
      } else {
      //  block of code to be executed if the condition1 is false and condition2 is false
      }

     - Switch Statement
     
      switch(expression) {
      case x:
      // code block
      break;
      case y:
      // code block
      break;
      default:
      // code block
      }

- ### Loops
     The JavaScript loops are used to iterate the piece of code using for, while, do while or for-in loops. It makes the code compact. It is mostly used in array.
     
     There are four types of loops in JavaScript.
     1.for loop
     2.while loop
     3.do-while loop
     4.for-in loop

    - For loop
     The  `for loop` iterates the elements for the fixed number of times. It should be used if number of iteration is known. The syntax of for loop is given below.
     
     |    |    |
     |-----:|---------------|
     |for (initialization; condition; increment)<br>{<br>code to be executed<br>}|<script><br>for (let i=1; i<=5; i++)<br>{<br>document.write(i + "<br/>")<br>}<br></script>|

    - while loop
    
    `while loop` iterates the elements for the infinite number of times. It should be used if number of iteration is not known. The syntax of while loop is given below.
    
     |    |    |
     |-----:|---------------|
     |while (condition)<br>{<br>code to be executed<br>}|<script><br>var i=11;<br>while (i<=15) {<br>document.write(i + "<br/>");<br>i++;<br>}<br></script>|


     - do while loop

     `do while loop` iterates the elements for the infinite number of times like while loop. But, code is executed at least once whether condition is true or false. The syntax of do while loop is given below.


      do
      {  
      code to be executed  
      } while (condition);  
-

      <script>  
      var i=21;  
      do {  
      document.write(i + "<br/>");  
      i++;  
      } while (i<=25);
      </script>  

     - for...in loop
     In each iteration of the loop, a key is assigned to the key variable. The loop continues for all object properties.
     
      for (key in object) {
      // body of for...in
      }
-

      const student = {
      name: 'Monica',
      class: 7,
      age: 12
      }
      // using for...in
      for ( let key in student ) {
      // display the properties
      console.log(`${key} => ${student[key]}`);
      }


- ### Functions
     `Functions` are used to perform operations. We can call JavaScript function many times to reuse the code.


     - With Arguments
     
      <script>  
      function getcube(number){  
      alert(number*number*number);  
      }  
      </script>  
      <form>  
      <input type="button" value="click" onclick="getcube(4)"/>  
      </form> 

     - Return value
     
      <script>  
      function getInfo(){  
      return "hello javatpoint! How r u?";  
      }  
      document.write(getInfo());  
      </script> 

     - Function Object

      <script>  
      var add=new Function("num1","num2","return num1+num2");  
      document.writeln(add(2,5));  
      </script>  

- ### Let's see function methods with description.

     |Method|Description|
     |-----:|---------------|
     |apply()|It is used to call a function contains this value and a single array of arguments.|
     |bind()|It is used to create a new function.|
     |call()|It is used to call a function contains this value and an argument list.|
     |toString()|It returns the result in a form of a string.|

- ### Arrow Functions
     - Arrow functions were introduced in ES6.
     
     Syntax before arrow
     
      hello = function() {
      return "Hello World!";
      }

     Syntax after arrow

      hello = () => {
      return "Hello World!";
      }

- ### Objects
     A javaScript object is an entity having state and behavior (properties and method). For example: car, pen, bike, chair, glass, keyboard, monitor etc
     
     JavaScript is an object-based language. Everything is an object in JavaScript.
JavaScript is template based not class based. Here, we don't create class to get the object. But, we direct create objects

     There are 3 ways to create objects.

     - JavaScript Object by object literal

     Syntax
     
__

      object={
      property1:value1,
      property2:value2
      }  
__

      <script>  
      emp={
      id:102,
      name:"Shyam Kumar",
      salary:40000
      }  
      document.write(emp.id+" "+emp.name+" "+emp.salary);  
      </script>  

__

     - By creating instance of Object
__

     Syntax
     
      var objectname=new Object();  
__

      <script>  
      var emp=new Object();  
      emp.id=101;  
      emp.name="Ravi Malik";  
      emp.salary=50000;  
      document.write(emp.id+" "+emp.name+" "+emp.salary);  
      </script>  
__

     - By using an Object constructor
__

      <script>  
      function emp(id,name,salary){  
      this.id=id;  
      this.name=name;  
      this.salary=salary;  
      }  
      e=new emp(103,"Vimal Jaiswal",30000);  
      document.write(e.id+" "+e.name+" "+e.salary);  
      </script>  


- ### Arrays
     An array is a special variable, which can hold more than one value.

     - Why to use Arrays
     If you have a list of items (a list of car names, for example), storing the cars in single variables could look like this:

      let car1 = "Saab";
      let car2 = "Volvo";
      let car3 = "BMW";

     However, what if you want to loop through the cars and find a specific one? And what if you had not 3 cars, but 300?
     
     The solution is an array!
     
     An array can hold many values under a single name, and you can access the values by referring to an index number.

     - Creating an Array

      const array_name = [item1, item2, ...]; 
__

      const cars= ["Saab", "Volvo", "BMW"];
      Spaces and line breaks are not important. A declaration can span multiple lines:
      const cars = ["Saab","Volvo","BMW"];

- ### Arrays are Objects
     Arrays are a special type of objects. The typeof operator in JavaScript returns "object" for arrays.
     
     But, JavaScript arrays are best described as arrays.
     
     Arrays use numbers to access its "elements". In this example, person[0] returns John:
     
     Array : `const person = ["John", "Doe", 46];`
     
     Objects use names to access its "members". In this example, person.firstName returns John:
     
     Objects : `const person = {firstName:"John", lastName:"Doe", age:46};`

- ### Promises
     The Promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting value.
     A Promise is in one of these states:
     - pending: initial state, neither fulfilled nor rejected.
     - fulfilled: meaning that the operation was completed successfully.
     - rejected: meaning that the operation failed.


   ![image](https://user-images.githubusercontent.com/117704825/204896418-21544314-87a6-4931-98c2-4bfc48629c46.png)

     - A promise can be created using Promise constructor

     Syntax : 

      var promisename = new Promise (function(resolve,reject){
      //do something
      })
      
     Example :
     
      var promise = new Promise(function(resolve, reject) {
      const x = "geeksforgeeks";
      const y = "geeksforgeeks"
      if(x === y) {
      resolve();
      } else {
      reject();
      }
      });
   
      promise.
      then(function () {
      console.log('Success, You are a GEEK');
      }).
      catch(function () {
      console.log('Some error has occurred');
      });


     - When a promise is fulfilled
     When a promise is fulfilled, you can access the resolved data in the then method of the promise:

      promise.then(value => {
      // use value for something
      })

     Think of the then method as "this works and then do this with the data returned from the promise". If there is no data, you can skip the then method.
     It's also possible that the then method can return another promise, so you can chain another then method like this:

      Promise
      .then(value => {
      return value.anotherPromise()
      })
      .then(anotherValue => {
      // use this value
      })

     - When a promise is rejected
     When a promise is rejected (that is, the promise fails), you can access the error information returned in the catch method of the promise:

      promise.catch(error => {
      // interpret error and maybe display something on the UI
      })

     - When a promise settles
     There's a last stage of the promise. Whether the promise is fulfilled or is rejected, the promise has been completed (has been settled). At this completed stage, you can finally do something.
     
     example
     
      let dataIsLoading = true;

      promise
      .then(data => {
      // do something with data
      })
      .catch(error => {
      // do something with error
      })
      .finally(() => {
      dataIsLoading = false;
      })



- ### Async Syntax
     The keyword async before a function makes the function return a promise:

      async function myFunction() {
      return "Hello";
      }
      is same as :
      function myFunction() {
      return Promise.resolve("Hello");
      }

- ### Await Syntax

     The await keyword can only be used inside an async function.

      async function myDisplay(){
      let myPromise= new Promise(function(resolve,reject){
      resolve("resolved!");
      });
      document.getElementById("demo").innerHTML = await myPromise;
      }

      myDisplay();

     The two arguments (resolve and reject) are pre-defined by JavaScript.
     We will not create them, but call one of them when the executor function is ready.

- ### Browser Object Model (BOM)

     The Browser Object Model (BOM) is used to interact with the browser.

     example

      window.alert("hello javatpoint");  

      is same as: 

      alert("hello javatpoint");  

- ### Document Object Model
     The document object represents the whole html document.
     When html document is loaded in the browser, it becomes a document object. It is the root element that represents the html document. It has properties and methods. 

      window.document  
      is same as :
      document  

- ### The important methods of document object are as follows:

     |Method|Description|
     |-----:|---------------|
     |write("string")|writes the given string on the doucment.|
     |writeln("string")|writes the given string on the doucment with newline character at the end.|
     |getElementById()|returns the element having the given id value.|
     |getElementsByName()|returns all the elements having the given name value.|
     |getElementsByTagName()|returns all the elements having the given tag name.|
     |getElementsByClassName()|returns all the elements having the given class name.|


- ### Classes
     ECMAScript 2015, also known as ES6, introduced JavaScript Classes.
     JavaScript Classes are templates for JavaScript Objects.

     - Use the keyword class to create a class.
     - Always add a method named `constructor():`
     
      class ClassName{
      constructor(){ 
      ... }
      }

     - The example below creates a class named "Car".
     - The class has two initial properties: "name" and "year".

      class Car{
      constructor(name, year) {
      this.name =name;
      this.year =year;
      }
      }

     A JavaScript class is not an object.
     It is a template for JavaScript objects.

     When you have a class, you can use the class to create objects:

      let myCar1= new Car("Ford", 2014);
      let myCar2 = new Car("Audi", 2019);
      The example above uses the Car class to create two Car objects.
      The constructor method is called automatically when a new object is created.

   ![image](https://user-images.githubusercontent.com/117704825/204896540-7a36772e-8731-4a8c-95bd-f97a93eaca06.png)

- ### Exception Handling 
     In programming, exception handling is a process or method used for handling the abnormal statements in the code and executing them. It also enables to handle the flow control of the code/program. 

     `try{} statement`: Here, the code which needs possible error testing is kept within the try block. In case any error occur, it passes to the catch{} block for taking suitable actions and handle the error. Otherwise, it executes the code written within.

     `catch{} statement`: This block handles the error of the code by executing the set of statements written within the block. This block contains either the user-defined exception handler or the built-in handler. This block executes only when any error-prone code needs to be handled in the try block. Otherwise, the catch block is skipped


      try{  
      expression; //code to be written.  
      } catch(error){  
      expression;
      } // code for handling the error.  

__

      try{  
      var a= ["34","32","5","31","24","44","67"]; //a is an array  
      document.write(a);    // displays elements of a  
      document.write(b); //b is undefined but still trying to fetch its value. Thus catch block       will be invoked  
      }catch(e)
      {  
      alert("There is error which shows "+e.message); //Handling error  
      }  

__   
           
Throw statements are used for throwing user-defined errors. User can define and throw their own custom errors.
-
           throw exception;  
__

      try {  
      throw new Error('This is the throw keyword'); //user-defined throw statement.  
      }  catch (e) {  
      document.write(e.message); // This will generate an error message  
      }  


- ### try…catch…finally statements
     Finally is an optional block of statements which is executed after the execution of try and catch statements.

      try{  
      expression;  
      }  catch(error){  
      expression;  
      }  finally{  
      expression;
      } //Executable code  

__

      try{  
      var a=2;  
      if(a==2)  
      document.write("ok");  
      }  catch(Error){  
      document.write("Error found"+e.message);  
      }  finally{  
      document.write("Value of a is 2 ");  
      } 

- ### Use Strict (Strict Mode )
`"use strict"`; Defines that JavaScript code should be executed in "strict mode".

Strict mode is declared by adding `"use strict"`; to the beginning of a script or a function.

      “use strict”;
      myFunction();

      function myFunction() {
      y = 3.14;   // This will also cause an error because y is not declared
      }

__

      x = 3.14;       //  This will not causeerror.
      myFunction();

      function myFunction() {
      “use strict”;
      y = 3.14;   // This will cause an error
      }
     
 ---
