# Architectural Decision Log
**Database:** MongoDB  
  
**Primary Code Language:** Undecided (JS or TS)  
  
**UI Frameworks:** Material UI  
  
**Database Language:** Undecided (SQL or NoSQL)  

# Style Guide 
We have decided to Adopt the AirBnB style guide for this project  
  
[AirBnB Style Guide](https://github.com/airbnb/javascript#:~:text=1%20Table%20of%20Contents.%20%202%20Types.%20Symbols,10%20Translation.%20%2011%20Contributors.%20%20More%20)
  
# Language Choice - JavaScript/TypeScript
### Background 
This report compares JavaScript and TypeScript to determine which is better for our project code. 
### JavaScript Pros and Cons
#### Pros
- All JavaScript can be converted to TypeScript if needed by changing .js extension to .ts
- Scripting langue
- Interpreted (reduced run time during compilation)
- Client-side script, speeds execution of the program
- Dynamically typed (don’t declare variable types concretely. You can change the types of variables)
- Very popular programming language, lots of recourses available to get help and ask questions
- Runs on a wide variety of platforms
- IDE supported (VSCode supports which is the IDE that we will use)
- Simplicity (easy to understand and learn) Simple for users and developers and feasible to implement
- Works well in correlation with other programing languages (It can be imbedded into other languages or into a webpage)
- Good server load (data validation occurs on the browser rather then server. Whole website has no need for reload so it makes for faster switching between web sections)
- Includes 3rd party add-ons to build applications with more ease. 
- Versatile ( works for front-end and back-end development (have libraries like node and express to help))
- Reduces code length
- Doesn’t require compilation
- All JavaScript can be converted to TypeScript if needed by changing .js extension to .ts
- Scripting langue  
  
#### Cons
-	Client-side security (Since code is viewable from the user's perspective)
-	Browsers may interpret the code differently depending on which you use.
-	Only supports single inheritance (methods from base class gets copied or ‘inherited’ to derived class, multiple inheritance copies features from more then one parent object or class)
-	Single code error can cause whole program to shut down.
-	Dynamically typed

### TypeScript Pros and Cons
#### Pros
-	Supports JavaScript Libraries
-	Object oriented programing language (objects which contain data and a code [fields and procedures])
-	Static typing (strongly / strict typed)
-	Points out compilation errors at run time
-	Refactoring (allows mistakes to be altered for example if you change a name of function, all instances where it is called will be changed)
-	Relies on JS syntax and semantics (very similar languages) and therefore comes with most of its pros (not all 😊)
-	Opensource code Backed by Microsoft
-	IDE supported (VSCode supports which is the IDE that we will use)
-	Manage code easier through types
#### Cons
-	Not true static typing (eventually gets compiled into JS so not same static typing as other languages)
-	Needs to be compiled to JavaScript before running so takes up more time.
-	Have to write more code than in JavaScript since has more syntactic sugar and type annotations.
-	Requires compilation
-	May not be supported in all browsers
-	Browsers may interpret the code differently depending on which you use.

### Comparison
JavaScript and TypeScript are basically the same language with only a few slight differences. TypeScript is a language that was built off of JavaScript with a stricter typing scheme. Therefore, all JavaScript code can be turned into typescript code by changing the .js extension to .ts in each file. This means that TypeScript has almost the same advantages as JavaScript and can use all its extensive libraries. The main differences as mentioned before is TS has static typing (though not true static typing compared to languages like Java). This means that you cannot change the types of variables once you have declared them unlike java where the typing is dynamic. This makes it easier to debug code as well, and TypeScript points out compilation errors at runtime unlike JavaScript. This also means that you need to write more code in one file of TS than you would in JS because of all the syntactic sugar.   
Another issue is since TS is built off of JS, when you compile the code, you need to first compile it into JavaScript then run it where JS does not require compilation. This means that it takes a lot longer to run TS code. There are also more users of JS then there are TS so there is more tutorials and videos out there to use for reference of ask questions. 
### Conclusion
The two programing languages are very similar and would both work well with what we are trying to accomplish. The solution we picked is JavaScript because it is so widely used and opensource platforms similar to the platform we want to create are built using JavaScript. This makes it easier to learn from other examples and implement them in our own code.


# MaterialUI  

# Database Decision - MongoDB/Postgres

# Database Language - SQL/NoSQL
