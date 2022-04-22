# Architectural Decision Log
**Database:** MongoDB  
  
**Primary Code Language:** JavaScript 
  
**UI Frameworks:** Material UI  
  
**State Management System:** Redux

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
JavaScript and TypeScript are basically the same language with only a few slight differences. TypeScript is a language that was built off of JavaScript with a stricter typing scheme. Therefore, all JavaScript code can be turned into typescript code by changing the .js extension to .ts in each file. This means that TypeScript has almost the same advantages as JavaScript and can use all its extensive libraries. The main differences as mentioned before is TypeScript has static typing (though not true static typing compared to languages like Java). This means that you cannot change the types of variables once you have declared them unlike JavaScript where the typing is dynamic. This makes it easier to debug code as well, and TypeScript points out compilation errors at runtime unlike JavaScript. This also means that you need to write more code in one file of TypeScript than you would in JavaScript.   
Another issue is since TypeScript is built off of JavaScript, when you compile the code, you need to first compile it into JavaScript then run it where JavaScript does not require compilation. This means that it takes a lot longer to run TypeScript code. There are also more users of JS then there are TS so there is more tutorials and videos out there to use for reference of ask questions. 
### Conclusion
The two programing languages are very similar and would both work well with for we are trying to accomplish. The solution we picked is JavaScript because it is so widely used and opensource platforms similar to the platform we want to create are built using JavaScript. This makes it easier to learn from other examples and implement them in our own code.
### Sources
[Advantages and Disadvantages of JavaScript](https://data-flair.training/blogs/advantages-disadvantages-javascript/)  
[TypeScript Pros and Cons](https://www.altexsoft.com/blog/typescript-pros-and-cons/)  
[TypeScript or JavaScript](https://www.stxnext.com/blog/typescript-pros-cons-javascript/)

# MaterialUI  
Material design is a set of style guidelines. Rule set to handle design situations. 
### Pros
-	Smooth UI transitions and animations between elements (can be used for movement on screen or highlighting buttons ect…)
-	Fast page switching, animations, fast screen scrolling and content updates
-	Self contained UI components that are reusable and packed with API styles for your use.
-	Responsive to different page sizes (for example if have a small screen size)
-	Takes less time to make animations since elements are standardized within a webpage
-	Customizable by colour, graphics, typography, ect… you can choose the correct fit for you
-	Has a robust component library
-	Has extensive icon library
-	Good documentation in framework with examples
-	Works well with react

### Cons
-	Objects on page move when you do certain actions, for example scrolling down
-	Requires a learning curve. 
-	Easily identifiable with its increasing popularity
-	Made by google, so primary for people who use google or android

### Conclusion 
Material UI is a easy and simple way to create and standardize components to be used later on in the code. 

### Sources

[Material Design Pros and Cons](https://www.bootstrapdash.com/why-choose-material-design-pros-cons/)  
[why use material design](https://www.toptal.com/designers/ui/why-use-material-design)

### HWP Adoption
[Implementation Info Page](https://github.com/bcgov/CITZ-HybridWorkplace/wiki/Material-UI)

# Database Decision - MongoDB/PostgreSQL
### Background
This report compares database providers, MongoDB or PostgreSQL, and we will determine which will be a better fit for our project
### MongoDB 
#### Pros

- Schema free NoSQL database with distributed architecture meaning its flexible
- Can search by field, range query and regular expressions
- Index any field in a document and supports the master/slave replication process
- Can group similar data in the database due to its automatic load configuration
- Stores files of any size without complicating the stack
- Uses aggregation pipelines to process queries (framework for data aggregation (data is expressed in summary form))
- Uses redundant replica sets (collection of MongoDB instances where each have primary and secondary node. (secondary node copies changes by primary node for recovery)) to maintain data allowing you to record or an as required basis. 
- Uses indexes to connect tables together
- Free but offers different pricing plans for use. 
- Has the potential for ACID (Not built in though)
- Document database and uses BSON for processing, and supports JSON data model
- High data availability and scalability for handling large data
- Easy set up and learning curve
#### Cons 
- Does not support foreign keys
- Hard to uncover insights rapidly
- Difficult to integrate data from multiple sources and store in a common formatting scheme
- Has some vulnerabilities in security
- Does not support traditional SQL syntax
- Joins not supported since its not a relational database
- Uses a lot of memory

### PostgreSQL
#### Pros
- Object-relational free opensource database
- Robust feature set
- Highly extensible meaning you can define your own data types, build custom functions and write code from different programing languages in the database
- Keeps up with SQL standard
- Comes with Reliability or disaster recovery. 
- Advanced and well documented database system. 
- Easy to learn and understand
- It supports the storage of image, video, audio and graphical data
- High recovery
- Table inheritance
- Can run on all operation systems
- A lot of community support available
- Supports ACID (Built in); Atomicity, Consistency, Isolation, Durability
- access control system have features that allow row and column level security and multi-level authentication with certificates
- reliable storage with fail safes and redundancies. 
- SQL based database 
- supports foreign keys (column or group of columns that references another column to establish relationship between)
- free for everyone
#### Cons
- Architecture creates separate services for every client which turns into a lot of memory utilization
- compared to other Database models, Postgres is not good at performance
- not very fast compared to others
- replication is complex
- Hard installation process
- limited scalability since processing power depends on the machine its running on
- cant use indexes in results of a query

### Comparison

MongoDB is a document oriented database meaning it is designed for storing retrieving and managing documented oriented info.  
Postgres is a relational database based on the relational model of data. It stores data points that are related to one another.  
If your using lots of unorganized data, document databases are the way to go, versus if your using structured data related to each other, you should use relational.   
  
PostgreSQL is a SQL based database but supports some NoSQL. MongoDB only supports NoSQL features. MongoDB uses collections to enforce the rules, and relationships between attributes are maintained through triggers. PostgreSQL uses tables to set triggers on data. It tries to structure the data so it can efficiently process it.   
  
MongoDB uses indexes to connect multiple tables together versus PostgreSQL uses joins. Indexes are a data structure with a small amount of data (easy to understand). Joins also combines data as long as you have 2 or more data tables, and there are 4 different types of joins.  
  
MongoDB is a good choice if you are first learning database management and lack programing experience since it does not follow SQL syntax. It is also a good choice if you want high computation and processing power.   
PostgreSQL is a good choice if you want traditional SQL syntax and have fewer resources.   
### Conclusion

Both databases are strong choices, but since we want an easy to use system and we are all new to database design, we are going with MongoDB as our database choice. 

### Sources
[PostgresSQL](https://www.postgresql.org/about/)  
[What Is PostgreSQL](https://www.educba.com/what-is-postgresql/)  
[mongoDB vs PostgreSQL](https://hevodata.com/learn/mongodb-vs-postgresql/#:~:text=MongoDB%20is%20a%20document%20database%20and%20uses%20BSON,schema-free%20NoSQL%20database%20that%20supports%20a%20distributed%20architecture.)  
[Advantages of MongoDB](https://data-flair.training/blogs/advantages-of-mongodb/)  

# State Management System 
### Background
This Report Chooses the state management system we are using in our code  
  
### Redux
#### Pros
- good integration with react frameworks
- Makes state predictable
- Maintainable due to its strict organization
- Persistent state
- Easy to debug since log actions and states  
- can manage state in a single place so changes made are more predictable
- Components don't need to share data for their children
- can optimize performance of your app
#### Cons
- Very large boiler plate
- Requires a learning curve
- Complex if don't require data from multiple sources
- Small changes could require you to write a large amount of code

### Conclusion 
Redux is a hard to learn and understand tool that requires a lot of boiler plate code to run, however since we will potentially be using a lot of data, it is a good system to use to manage state. Using Redux will make our code maintainable and easier to debug. 

### Sources 
[When to choose Redux](https://blog.boardinfinity.com/working-with-redux-pros-and-cons/)
[Why Choose Redux](https://blog.logrocket.com/why-use-redux-reasons-with-clear-examples-d21bffd5835/)
[Don't use Redux](https://orgler.medium.com/dont-use-redux-9e23b5381291#:~:text=What%20I%20Hate%20About%20Redux,result%20in%20small%20code%20changes.)

### Documentation

[tips] (https://github.com/kkk987/mern-documentation)
