# startup
CS 260 - Startup Project Repository


Key Things Learned:
- How to create a new repository in Github and clone it into a specific directory.
- Committing changes to a readMe file from Github and its location on my computer and pulling those changes from either end.
- Pushing changes made in the local directory to Github.
- Merging changes when a commit is made in Github and in the local directory.
  
  
Elevator Pitch:
So often in our lives, whether on our own or when working with others, we find it hard to keep our responsibilities in order. We try to maintain a list in our head and end up forgetting something important. Or when working with a team, we lose track of all the current tasks being worked on and don't know what needs to be done. The solution to each of these dillemmas and many more can be described with one word: collaborate. Collaborate is a product which enables one to record tasks and check them off once they're done. It also encourages organization with the ability to group tasks together into lists. Lists which can be shared across a team to ensure collaboration and transparency. As soon as you choose to collaborate and organize yourself, what was a stress will be replaced with fulfillment and satisfaction.

![CS 260 - Startup Sketch](https://user-images.githubusercontent.com/116193374/214912795-f10228db-c09d-4bcb-b283-5b87e9b6aee5.png)

Startup Key Features:
- Secure login with a profile for the person.
- Ability to create task lists with a name.
- Viewing screen for both the lists and for the tasks in each list.
- Add a task with a description and due date.
- Delete individual tasks.
- Check a task off and have it move from in progress section to completed.
- A way to transition a completed task back to in progress.
- Scroll bar for both in progress and completed section for tasks.
- Task list sharing with other people allowing for collaboration.
- Notifies other users who have shared access to a list that a task was completed by a specific person or that someone accepted an invite to join the task list.
- (Optional) Incorporate some way of creating task reminders.
   
   
Server Startup:
- Elastic IP Address: 3.142.167.250
- ssh -i [key pair file] ubuntu@[ip address]
- `chmod  600 [key pair file]`
- I have been working as an intern for a Internet Security company so it has been cool to make some connections with the ISP things I have been doing there with this class. For example, understanding that 0.0.0.0 enables any IP to access something like a server or how an IP ended in .1 would be the network. I look forward to what will come next.
   
   
Route 53 Setup:
- I learned how to purchase my own domain with a specified/available TLD and from there was able to associate it with my server's public IP address.
- In addition, I was also able to add a record to make sure that no matter what subdomain is tagged onto the front of my domain.TLD, that it will still route to my server.
- Website domain: http://cs-260.click
   
   
Web Certificate Setup:
- When trying to use an ssh key to access a webserver, make sure to either navigate to the directory where it exists or find the correct path to it.
- On windows home doesn't exist so '~' doesn't work to bring you to the C drive.
- Inside of a Caddyfile, when using vi, if you want to edit its contents make sure that you see INSERT the bottom. Otherwise, hit 'i' and it will enable that mode.
- To leave a mode, hit ESC.
- When saving and quiting, make sure you are not in some mode and type at the bottom :wq and then hit enter; another option is ZZ.
- Once you're back in ubuntu, if you get the "There are stopped jobs" message preventing you from exiting, ctrl + z will terminate any ongoing stopped jobs.
   
   
HTML:
- [&nbsp]; is the escape sequence for adding a blank space which doesn't add a new line.
   
   
Simon Project:
- I learned how to adjust the height and width of an image that I've inserted into a webpage with HTML.
- After doing some googling, I figured out how to adjust the text size for certain pieces of text within in HTML tags.
- Found out how to update some of ubuntu files through ssh.
- Familiarized myself more with some of the unique HTML tags and their corresponding attributes.
   
   
CSS Practice:
- Learned how to remove a vertical scroll bar by doing the following: overflow-y: hidden;
- Figured out how to rotate text x number of degrees around a point by using the rotate function in the transform class.
- How to center text inside of a shape and how to create a circle element inside of CSS.
- Changing the position using the relative keyword and adjusting the positioning using top, right, bottom, and left.
   
   
CSS Flex:
- Flex can be a bit difficult to use in combination with the margin and position properties.
- Can use margin to make sure there is space between grid elements and the outer edge of a flex element when you use the grid option for display for a child which has a parent using the flex option instead.
   
   
CSS Simon:
- The hyperlinks in the navbar menu element are not blackend and appear somewhat lighter unless you add the "active" keyword to the     nav-item when you are currently at the hyperlink's webpage.
- Margins can also have four directional values for top right left bottom.
- border-radius determines how rounded shape elements or text boxes are.
- You use row for flex-direction when you want the flex items to appear in one row and column if you want them to appear one after the other in a vertical column.
- min/max-height and min/max-width are used to restrict a an element from surpassing either a lower or upper size bound.
- If you want to restrict a paragraph line from extending to far on one line, you can set a max-wdith and add a character max(ch).
- Applying a theme to the thread tag doesn't necessarily work, so you can instead apply it to the tr tag for the info row.

   
CSS/HTML Startup:
- You can change just about any property, if not every property, using media for a change in the webpages size.
- The "card" class is very useful for creating a background box to contain and provide a backdrop for other elements.
- Use "::-webkit-input-placeholder" as a block in CSS to adjust the input placeholder alignment, text size, weight, etc.
- .cursor-center CSS class with text alignment set to center starts the cursor at the center of an input box.
- The following is used to link button clicks to other webpages: onclick = "window.location.href = '[nameOfFile].html';".
   
   
JS Functions, Arrow Functions, Arrays, and Objects/Classes:
- Functions are used with the keyword function followed by the name of the function and parentheses with no or some parameters.
- Arrow functions must have curly brackets if they have more than one line otherwise they can be as simple as () = > [one line of code];.
- To get the output of an arrow function do the following: (() => [line of code])().
- Class member variables and functions are made private using a #.
- Classes do not declare their member variables outside of the constructor. They are defined and initialized in the constructor using this. followed by the name that you want to give it and set equal to either a specific value or a corresponding input.
   
   
JS Regex, Rest, Spread, and Destructuring:
- Regular expressions: textual pattern matchers; patterns used to match character combinations in strings. You can use them to find text in a string so that you can replace it, or simply know that it exists.
- Regex can be created either by using either the RegExp class constructor or a regular expression literal.
- Rest: prefixing the last parameter for a function with three dots allows for any number of parameters to be received and then converted into an array.
- Spread: prefixing an object or array with three dots before passing it to a function will match up each member variable or element to the function's parameters.
- Destructuring: the process of pulling individual items out of an existing one, or removing structure. This can be done with either arrays or objects.
   
   
Simon JavaScript:
- To store something locally, create a new variable to store an HTML element, and then write following: localStorage.setItem("[referenceName]", varEl.value).
- Once loaded to a local storage, call .getItem on localStorage with the given reference name to get the data stored.
- This will enable you to have a local reference to the value associated with an HTML element and be able to adjust it with a JavaScript.
- To retrive an element, you can either use querySelector("[#idName]") or getElementByClass("[classname]") if you want to reference its' class.
- querySelectAll with retrieve all elements with a certain id or class name.
- Use [nameOfElement].textContent to get a textual representation of a specific element.
- Buttons can be pressed with .press for a specified amount of time when applied to a button in a given moment.
- await allows us to enable things to run in the background even while the user may be on another page or is doing something else.
- JavaScript has built in capabilities for deserializing JSON strings and serializing JS code.
- [someArray].splice makes it possible to insert or disect arrays as you please.
- If you plan to initialize class member variables without using a variable with an identical name, then the member variables must be declared outside of constructor.
- It seems that you can include just an object in an if statement, and if the object has data, then it will return true, otherwise false.
- HTML elements can have be filled with other children with appendChild or by setting its innerHTML to a string of HTML code which builds the structures.
- Having const [var1, var2. ...] enables one to have variables that update as one iterates through an array of objects using a for loop.
   
   
Startup JavaScript:
- If I don't have access to a database, I can either store something in localstorage or sessionstorage if I want what is saved to disappear once webpage is closed.
- To swap between two icon states by clicking on them, I can add an event lister for one and when changing to a different icon, add an event lister to the new icon within the other eventlister to allow me to be able to cycle back and forth between them.
- In order to data from other js files, one must have the send file export the data desired and then have the receiving js file import them by name.
- However, the receiving js file needs to be a module since modules can only share data with other modules.
- When including the script in HTML, make sure to add type = 'module'.
- innerHTML looks down one level from the element it is called on.
- An alternative to using justify-content: center and flex: # is justify-content: space-between and width of each element set to a specific percent.
- Keypress is an event that can be used to listen for any key on the keyboard and do something when it is pressed.
  
  
Simon Services:
- When using Node.js to run a project using services, make sure to do npm init -y and then install express: npm install express.
- After installing express, consolidate all of your files (HTML, CSS, JS, etc) into one directory and call it public.
- Next create a JS file and call it server.js or index.js; it will be where code will be added for the server functionality which includes the port number that will be listening for HTTP requests, the imported use of express, different actions (endpoints), etc.
- Importing the use of express (or any other package):
  - const express = require('require');
  - const app = express();
- Unlike before where JSON had to deserialized everytime, we can do one command to do that for all request bodies: app.use(express.json());
- To use the static public directory we created to store our files, do the following: app.use(express.static('static'));
- If we want to route all of the requests through one junction, we can create a router: var apiRouter = express.Router(); app.use('/[subname]', apiRouter);
- And from there we can do what we would normally do with app and define the steps that will be taken when certain HTTP requests come through.
- For requests like get or post, the corresponding functions will take in two parameters: a string for the URL path and an arrow function which will have two parameters as well; req for the request and res for the response.
- To listen on a port, write this: app.listen(port, () => { console.log('Listening on port ${port}');};
- If you don't want certain things to be committed when using the commit command, create a .gitignore file and add directory to the file.
- Sometimes a period will need to be added at the beginning and a forward slash at the end to ignore all files within the directory.
- Use fetch to retrieve resources from webpages asynchronously. It will return a promise which will be fulfilled once the response, or resource(s), is available.
- Fetch takes in a URL and takes the response, converts it to JSON with one then statement, and with another then statement containing the parameter 'data' for the response, it can be used in whatever way the user desires.
- Since index.js links to the public directory, any global variables in the JS files can be referenced. So for instance, with scores, index.js can reference it and send the variables contents as a response when a get request with the URL path '/score';
- We can create default when no recognizable path is provided by using app.use with no path parameter and just an arrow function.
- For post requests, they can be captured by calling fetch for the given URL path and have their response stored in a variable.
- Once that is done, we can do an await to store the deserialized response in another variable.
  
  
Simon Database:
- For the database code, create a separate JavaScript file to contain it.
- Make sure your environment variables for user, password, and host name match what you have for your cluster and account with MongoDB Atlas.
- The url used for creating a MongoClient has the following template: const url = 'mongodb+srv://${userName}:${password}@${hostname}';
  - userName will be represented by process.env.[NameForUser], password represented by process.env.[NameForPassword], and process.env.[NameForHostName].
- Create the client by calling new MongClient([url]).
- To create a new database with a new collection for JSON objects (or other objects), call your newly created client in this way:
  - client.db('[NameForDatabase]').collection('[NameForCollection]');
  - The .db and .collection functions will create a new instance of a database and collection with the names you provided.
- We store objects in a collection by calling insertOne(Object) on the collection we created.
- If we want to use database functions that add or query for certain things, export them by typing module.exports = {function1, function2, ...};
- Make sure your server/index JS file adds the Database: const DB = require('./[databaseName].js');
- Now for each of our endpoints, we can use our defined database tractions to do certain things like updating scores and querying for data.
  
  
Simon Login:
- bcrypt: it is a library that provides hashing capabilities for making passwords/authtokens unrecognizable or crackable.
- 409 error code used to tell the user that the info provided is already in use for another existing user.
- When creating a cookie to store the info passed in to be verified, we can add three properties to make it more secure:
  - secure: ensures that only HTTPS is used when passing the cookie back; no HTTP or any other protocol.
  - httpOnly: will not be accessed or looked at by any JavaScript on the browser.
  - sameSite: the cookie's return destination is strictly the domain that generated it.
- Every cookie is given a specific name and an authentication token.
- We can divide up the responsiblities for routers which handle the various endpoints. An example of this is wrapping one router in another which specifically does the verification of credentials for endpoints before proceeding.
- Send a 404 code for things that are unknown like trying to login with credentials for an account that doesn't exits.
- Use bcrypt.compare to compare the hashed password stored in the database with the password provided by the end-user.
- When logging out, clear the cookie of contents like the authtoken and return a status code of 204.
- Optional Chaining operator('?.'): enables you to read the value of a property located deep within a chain of connected objects without having to check that a child actually exists deep in the object or not.
- Can use setDisplay function to block or show certain elements by their ID.
- To create bootstrap elements, you can do new bootstrap.[bootstrap element] to create the element you want from the framework.
   
   
Simon WebSocket:
- Good idea to create a separate proxy JavaScript file to contain and isolate the protocol upgrade to WebSocket, track any new WebSocket connections, pass or proxy requests between connections, and keep track of whether or not the connections are active by tracing pings/pongs.
- Since the instance of the proxy class will likely not be referenced or used in the other JavaScript files, you can just create a new instance by calling new [nameOfProxyClass] at the end of the JavaScript, where you want it to be initialized, without storing it in any local or gloabl variable.
- If you do that, you need to make sure to add a require statement in order to get access to the Class from the other JS file.
- Adding require('uuid') imports in the UUID library which generates long authentication tokens or passwords that are generally unique.
- To make the WebSocketServer independent of another server, put in the new instance creatiom parenthesis {noServer: true}.
- Performing the upgrade from HTTP to WebSocket involves using the on function with the general HTTP server created at the beginning and passing it 'upgrade' and an arrow function with parameters for request, the socket, and the header.
- You then call the handleUpgrade function on your WSS with those parameters and another arrow function which calls wss.emit('connection', ws, request).
- Make sure to store your connections so that you can reference, use, and delete at some later date.
- For a connection endpoint, include the four following pieces inside:
  - Create a new connection with a UUID, an indicator for its alive status, and a property for it being a WebSocket.
  - An embedded WS 'message' endpoint to take a message and send it using the WS for each connection except the connection from which the message originates.
  - An embedded WS 'close' endpoint to locate a stored connection and remove it to prevent it from forwarding messages to the other connections.
  - An embedded WS 'pong' endpoint that can be used when a connection is pinged and needs to notify the server that it is still live.
- Use setInterval to go through each connection and close any that did not respond to previous pings, otherwise, set the alive status to false and ping again.
- When creating WebSocket, it is good to verify what protocol is being used for the current webpage and then assign it ws or wss depending on if the webpage has a insecure or secure protocol, i.e. HTTP vs. HTTPS.
- Then using that protocol create the new WS by doing '[protocol]://hostName/ws'
- Include some messages to be displayed when the WebSocket is created with onopen and closed with onclose.
- Then you can use the onmessage attribute for your WS and create some customized functionality and messages to be displayed based on the event taking place.
- Events can then be broadcasted by using the WS send function with a JSON object containing data you want to be shown.


Startup - WS & MongoDB
- Overall, I have come to understand pretty well how to make a service and do something from end to end using JavaScript to transmit data from the front-end to the backend and from the backend to the front-end. I took CS 240 this semester and we used a local database, Java, and android to do what we've done with this class, so taking this different approach with webservices and web related languages has given me new perspective.
- To use third-party services, npm needs to be installed in a project directory so that you can use it to get available APIs like uuid, bcrypt, and express.
- And once in your index.js file, which is starting point for your project to load, require statements must be used to import in the endpoints.
- A variety of routers can be used to separate endpoints and restrict them in ways that you desire. And for every router that trails on from another one, a new addition to the url is appended.
- To add extra authentication, use bcrypt to store a hash of password inserted upon user creation and then use the compare function when checking to see if the provided password matches the password stored in the database.
- Having a chain of module dependencies can cause JS files to be loaded when you don't want them to. I had one JS file link to one JS file which linked to another. This caused a lot of confusion as the last JS file in the chain was being loaded without it being referenced in the JS file used by my index.html.
- To take in values with a get request, you can't add a request body. But you can add them to the URL that matches with an endpoint. Just add it when performing a fetch request and then when receiving the URL at the endpoint, put /:[paramName]. You will then be able to extract the value with req.params.paramName.
- A status and an object can be sent back at the end of the fetch with a status to indicate success, and anything you want to send that will provide key information or an message to indicate why the API failed.
- To avoid moving on from an asychronouse process before it is finished, always use the await keyword at the beginning.
- If we want to export functions from the database JS that will be used by our web service JS file, we can add module.exports = {functionName1, functionName2,...}.
- After we have created an account in Mongodb Atlas and a cluster to store our databases, define a database and the collections that will go inside.
- Then to reference and use them in our backend database JS file, we can store them in variable by calling client.db('nameOfCollection').collection('collectionName').
- Client is created by initilaizing a new MongoClient with a url that contains our credentials and the information relating to our cluster's connection.
- Once we've created the desired collection reference variables, we can call a variety of functions that will perform certain queries which can be singular in what they return or many in what is returned.
- Each query function takes in an object which contains specific fields or details that will be used to add, delete, find, etc.
- The find function will return everything that matches our query while findOne will return the first occurence of an object that matches our search.
- InsertMany and InsertOne work similarly in that they can either insert either one object, or many objects into the database collection.
- updateOne is used to update a the contents of the fields in the collections objects specified by the query.
- When getting more than one object using find, you will need to user .toArray() to return what you retrieved as a JSON array.
- $and: is used to append more than one query together to create a combination query.
- $push: is a opertation used to be able push data into an array.
- Websockets are used to transmit data between connections that are currently open for many users.
- In your proxy class, you need to create a WS server and once we've upgraded our protocol, we connect to an our WSS endpoint which establishes connections.
- And with those connections, you can define what happens when to indicate when they are active, in the process of being closed, or when they receive a message.
- As a last step in the proxy, make sure set a time limit or interval to ping connections to see if they are active, close them if they aren't and keep them open for an allotted amount of time.
- General setup for doing something from one end to the other is to have a function that interacts with a database, an endpoint to send that function important information, and a function iniated from the front end which performs a fetch on the endpoint and passes it the important information.
- To use websockets have them pass information to other users, we need to configure a soocket with url that contains the protocol, host, and /ws at the end.
- Then we can use have it do certain things when it is opened, closed, and when it receives a message:
  - Those actions are defined by asigning arrow functions to the following: socket.onopen, socket.onclose, and socket.onmessage.
- So with a socket configured for every user, we can send info via the socket which will be sent through our 'message' wss endpoint which will then be routed to the destination user(s) configured socket which will then do something based on the event that is sent.


React CLI:
- You cannot enter down the open parenthesis when returning some kind of HTML element from a component.
- Doing this will make anything that follows the return unrecogizable and usable; it would be loaded.
- App.js will contain the front-end UX and reactivity with JSX components which combine those two things.
- Anything backend related will be handled by index.js and other js files.


Simon React:
- Just as we had an index.js to initiate the beginning of our backend, with React we will have a file called App.jsx to initiate the beginning of our components for the front end of our code which includes the appearance from HTML and the reactivity from JS.
-One of the important aspects of React is that everything is compartamentalized.
- For each of the possible pages that our program will run, we will have a separate directory which will typically contain at least one JSX and CSS file, but there coule be additional JSX files to break things up and extra JS files to handle separate reactivity.
- So in the case of Simon, there is login, play, scores, and about directory, each with CSS files and JSX/JS files.
- In order to debug a React project, we need to be able to run on two ports: one for the node.js service and one for the React client HTTP debugger.
- To convert to React components, you'll want to copy over your HTML into separate components and put the code in the return line of the component.
- Make sure to change the class to be className and then delete any header or footer that is carried over from the default App.jsx file. If you don't have a footer and or header that don't carry across multiple pages, than you can leave that.
- The JS will then need to be converted into functions that are placed inside the component above the return line.
- Create React state variables for the following: for each stateful object in the component and for any DOM query selectors.
- Sometimes it might be necessary to move state objects to a parent component designated for a specific state as indicated by the name you give it.
- And vice versa, creating some parent components can be helpful to create coherent, readable, and effective code.
- Utilize the useEffect hook to watch the username's state so that it proper permissions are kept in order and certain things are restricted if the username changes to something that hasn't been authenticated.
- In order to reference Bootstrap styles in your components, this needs to be at the top: import 'bootstrap/dist/css/bootstrap.min.css';.
- Also, when beginning the conversion, generate the CLI template, clear out anything you don't want and then bring it over to your project.
- Make to install the different npm packages for the service directort and then at the root of the project before trying to deploy to your Server.


<br></br>
<br></br>
<h2>MIDTERM EXAM NOTES</h2>

<h3>Development Essentials</h3>

<h5>Internet History</h5>

- Three Distinct Phases of Web Programming:
  - Formation of the internet that supports the communication of web applications.
  - The creation of HTML and HTTP that made it possible to share hyperlinked documents.
  - Creation of CSS and JavaScript that enabled interactive web applications.
- Internet Management Controlled by Two Major Organizations:
  - Internet Engineering Task Force (IETF): defines the technical standards that specify how the physical network communicates.
  - Internet Corporation for Assigned Names and Numbers (ICANN): oversees both the Internet Protocol (IP) address space and the Domain Name System (DNS)
    - These two databases form the address book of the internet.
- Hypertext Markup Language (HTML):
  - Key innovations of HTML was the idea that documents could be interconnected with what are called hyperlinks which enable immediate access to related docs.
  - Contains over 100 elements or tags at the moment.
- Hypertext Transfer Protocol (HTTP):
  - Example: http://info.cern.ch/hypertext/WWW/Helping.html
- Uniform Resource Locator (URL):
  - Example: GET /hypertext/WWW/Helping.html HTTP/1.1
             Host: info.cern.ch
             Accept: text/html
- These two definitions specify how web documents are addressed and transmitted across the internet.
- Cascading Style Sheets (CSS): designed to give HTML documents visual styling independent of the content's structure.
- JavaScript (JS): gave the ability to script web pages.
  - Turns a static web into an interactive experience where a web page could dynamically change based upon a user's interaction.
  - Node.js: first successful application for deploying JS outside of a browser.
  - Standardization of common object notation JSON, a typed variant named TypeScript and other transpilers for converting languages into ECMAScript(JS).
 
<h5>Technology Stack</h5>

- Collection of technologies used to create or deliever a web application is called a technology stack.
- At the top is generally the web framework (Angular, React, Vue, Svelte): it communicates with one or more web services to provide authentication, business data, and persistent storage. It then uses backend services such as caching, database, logging, and monitoring.
- Example Technology Stack: React for the web framework, talking to Caddy as the web server hosted on AWS, running web services with Node.js, and MongoDB as the database hosted on MongoDB Atlas.
- Be careful when building a commercial stack as you will need to think about dependability, support, scalability, performance, security, and development productivity factors such as documentation, ease of use, common acceptance, community support, build times, and testing integration.

<h5>The Console</h5>  

- Also known as the command line, shell, or terminal the console window provides access to the file system and allows for the execution of command line applications.
- POSIX compliance: supports a standard set of console commands. (any necssary console commansd work on the operating systems with that compliance)
- A primary purpose for a console application is to view files on the computer. The files are organized into a tree structure of nodes called directories.
- You can see which directory you are in with the 'pwd' (present working directory) command.
- You can list all of the files in the director with 'ls' (list files).
- Most command line applications take parameters that are specified after you type the application name.
- 'ls' can list files (even hidden ones) in a long format if you provide '-la' after 'ls'.
- List of Basic Commands:
  - echo - Output the parameters of the command
  - cd - Change directory
  - mkdir - Make directory
  - rmdir - Remove directory
  - rm - Remove file(s)
  - mv - Move file(s)
  - cp - Copy files
  - ls - List files
  - curl - Command line client URL browser
  - grep - Regular expression search
  - find - Find files
  - top - View running processes with CPU and memory usage
  - df - View disk statistics
  - cat - Output the contents of a file
  - less - Interactively output the contents of a file
  - wc - Count the words in a file
  - ps - View the currently running processes
  - kill - Kill a currently running process
  - sudo - Execute a command as a super user (admin)
  - ssh - Create a secure shell on a remote computer
  - scp - Securely copy files to a remote computer
  - history - Show the history of commands
  - ping - Check if a website is up
  - tracert - Trace the connections to a website
  - dig - Show the DNS information for a domain
  - man - Look up a command in the manual
- Chain Input and Output of Commands Using Special Characters:
  - '|' - take the output from the command on the left and pipe, or pass, it to the command on the right.
  - '>' - redirect output to a file; overwrites the file if it exists.
  - '>>' - redirect output to a file; appends if the file exists.
- Console Keystrokes:
  - 'CTRL-R': use type ahead to find previous commands.
  - 'CTRL-C': kill the currently running command.

<h5>Git</h5>

- Git provides two valuable functions:
  - First it allows you to track versions of files in a directory.
  - Second, it allows you to clone all of those versions to a differnt location, usually to a differnt computer.
- Create a new directory and initialilze it as a Git repository:
  - ➜  mkdir playingWithGit
  - ➜  cd playingWithGit
  - ➜  git init
- If you list all of the files you wil see that you now have a hidden directory named .git.
- Use 'echo' to create a file and then after creation, 'git status' to tell you what git is doing.
- To begin tracking versions, you have add a file using 'git add .'.
- It will then tell you it has staged the file an dit is ready to be committed as a version in the repository.
- We commit a version of a file with the 'commit' command.
- You always have to add a meaningful commment about the version being committed so using '-m' will provide a message that will live with the version.
- To tell Git we want to add all the tracked modified files to our commit, we include the '-a' parameter along with our message parameter ('-am').
- We can view the versions in our repository with the 'git log' command.
- Every commit has a unique identifier generated by hashing the file along with the timestamp using the SHA hasing alogorithm.
- This is very useful if you ever want to refer to a specific commit in your version history by using its SHA.
- If we want to temporarily switch back to a previous version to see what it contains, we can use 'git checkout [first few characters of SHA]'.
- To get back to the top of the version chain, use the 'checkout' command and reference the branch name which is by default 'master'.
- In most cases, we don't want to reverse back to an earlier commit and instead just want to compare differences between commits.
- We do that with the 'diff' command:
  - Specify two SHAs that you want to compare or you can use HEAD which points to the top of the commit change.
  - To refer to earlier commits, just add '~' and the numerical distance from head that you want to reference.
- Branches can be created if you would like to work on variations of the code while allowing progress on the main branch.
  - Use the command 'git branch [nameOfNewBranch]' and then 'git checkout [nameOfNewBranch]' to start working on the new branch.
- When you want to combine the work done on both branches, you checkout the master branch and execute 'git merge [nameOfSeperateBranch]'.

<h5>Development & Production Environments</h5>

- It is critical to separate where you develop your application, from where the production release of your application is made publicly available.
- Multiple environments to contain the development of code to divide up the stages involved in making software ready to be realized publicly.
- Continuous Integration (CI) processes checkout the code, lint it, build it, test it, stage it, test it more, and finally, releases it to the production environment if everything checks out, notifying different departments of the releae.
- You run a deployment script from a console window in your development window with a command like the following:
  - ./deployService.sh -k ~/prod.pem -h yourdomain.click -s simon
- The '-k' parameter provide the credential file necessary to access your production environment.
- The '-h' parameter is the domain name of your production environment.
- The '-s' parameter represents the name of the application you are deploying (such as simon or startup).

<h3>Web Servers</h3>

<h5>The Internet</h5>

- The internet can be thought of as a massive redundant collection of wires that connect up all of the computers in the world.
- A lot of the wires are wireless (wiFi, satellite, or cell), and not all of the computers in the worl are connected.
- When a device wants to talk to another device, it must have an IP address (e.g. 128.187.16.184).
- A symbolic name for an IP address is called a domain name: domain names are converted to IP addresses by doing a lookup in the Domain Name System (DNS).
- You can look up the IP address for any domain name using the 'dig' console utility.
- Next, you connect to the device by first requesting a connection route to the device.
- Connetion Route: consists of multiple hops across the network until the destination is dynamically and discovered and the connection established.
- The hops can be determined using the 'traceroute' console utility.
- Internet Service Provider (ISP)
- Actual sending of data across the internet uses the TCP/IP model: a layered architecture that covers everything from physical wires to the data that a web application sends.
- TCP/IP Architecture:
  - Layers: Application, Transport, Internet, and Link.
  - Example: HTTPS, TCP, IP, and Fiber/Hardware.
  - Purpose: Functionality like web browsing, moving connection information packets, establishing connections, and physical connections.
 
 <h5>Web Servers</h5>
 
 - Web server: a computing device that is hotsing a web service that knows how to accept incoming internet connections and speak the HTTP application protocol.
 - We can run a web service code and use the console application 'curl' to make an HTTP request and see the response body.
 - It is common to find multiple web services running on the same computing device.
 - Every network device allows for separate network connections by referring to a unique port number.
 - To resolve the issue of remembering a port number, a service gateway (reverse proxy) is introduced which is a simple web service that listens on the common HTTPS port 443. The gateway then looks at the request and maps it to other services running on different ports.
 - Web services that provide a single functional purpose are referred to as microservices.

<h5>Amazon Web Services - EC2</h5>

- How to remote shell into a server hosted on AWS:
  - ➜  ssh -i [key pair file] ubuntu@[ip address]
  - Example: ➜  ssh -i ~/keys/production.pem ubuntu@53.104.2.123
- The chmod (short for change mode) command is used to manage file system access permissions on Unix and Unix-like systems. 
- There are three basic file system permissions, or modes, to files and directories:
  -read (r), write (w), and execute (x).
- To restrict the permissions on your file so that they are not accessible to all uses run the 'chmod' command:
  - 'chmod  600 [key pair file]'
- The Caddyfile is the configuration file for your web service gateway.
- public_html directory contains all of the static files that you are serving up through Caddy when using it as a web service.
- Use the 'exit' command to exit a remote shell.
- Assigning an Elastic IP address to a server keeps the same address even if the server is stopped.
 
<h5>Domain Names</h5>
  
- A single domain name can be associated with multiple IP addresses so that in case one of them fails, another one can be used to maintain connection.
- Domain Name: a text string that follows a specific naming convention and is listed in the domain name registry.
- They are broken up into a root domain with one or more possible subdomain prefixes.
- Root Domain: represented by a secondary level domain and a top level domain (TLD).
  - Examples: byu.edu, google.com, or cs260.click.
- Top Level Domain (TLD): represent things like com, edu, or click.
- Domain Name Structure:
  - [subdomain.]*secondary.top; where secondary.top is the root domain.
  - Example: react.simon.cs260.click.
- The owner of a root domain can create any number of subdomains off the root domain.
- To get information about a domain name from the domain name registry, run the 'whois' command with the a website domain following that.
- DNS database records that facilitate the mapping of domain names to IPs come in a variety such as address (A) and canonical name (CNAME):
  - (A): a straight mapping from a domain name to an IP address.
  - (CNAME): maps one domain name to another domain name; this acts as a domain name alias.
    - You would use CNAME to do things like map byu.com to the same IP address as byu.edu so that either one could be used.

<h5>Amazon Web Services - Route 53</h5>

- Using a domain name in place of an IP address makes it easy to remember and secure.
- Route 53 is an AWS service that handles everything DNS related: buying domain names, hosting domain on their DNS servers, and creating DNS records.
- (NS) Name Server Record: contains names of the authoritative name servers that authorize you to place DNS records in this DNS server.
- (SOA) Start of Authority Record: provides contact information about the owner of this domain name.
  
<h5>Caddy</h5>

- Caddy is a webservice that listens for incoming HTTP requests:
  - Handles all of the creation and rotation of web certificates allowing support of HTTPS.
  - Serves up all of the static HTML, CSS and JS files.
  - Acts as a gateway for subdomain requests to application services such as the Simon or Startup project.
    - Example: when a request is made to simon.yourdomain Caddy will proxy the request to the Simon application running with node.js as an internal web service.

<h5>HTTPS, TLS, & Web Certificates</h5>

- With HTTP (non-secure hypertext transport protocol), the number of devices through which your connection goes through would leave any data or information passed along would be very exposed to being captured by anyone that has access to the network traffic.
- HTTPS (secure hypertext transport protocol) is basically HTTP with a negotiated secure connection that happens before any data is exchanged.
- The secure connection ensures that all data is encrypted using TLS protocol.
- TLS is sometimes referred to by the now unsecure predecessor protocol named SSL.
- It works by negotiating a shared secret that is then used to encrypt data.
- The actual negotiation can be seen by using the console browser based application 'curl' in combination with '-v': 'curl -v -s [domainName] /dev/null'.
- That last piece throws away the actual HTTP response.
- A core piece of the handshake is the exchange of a web certificate that identifies the domain name of the server creating the secure connection.
- The browser will compare the certificate domain name to the one represented in the URL and if they don't match, or the certificate is invalid or out of date, it will display a massive warning.
- Web Certificates: a digital file containing information that indicates the security and identity of a website using an encrypted connection.
- They are generated by a trusted 3rd party using public/private key encryption.
- The certificate issuer is responsible for verifying that the certificate owner actually own sthe domain name represented by the certificate.
- Using the IETF standard ACME protocol, anyone who owns a domain name, can dynamically generate and renew a certificate for free.
- Caddy uses Let's Encrypt to generate a web certificate every time an HTTPs request is made for a domain name that Caddy doesn't have a web certificate for.
- A web certificate ensures that user data is secure when transferred, verifies website ownership, & prevents attackers from creating fake versions of the site.
- 'sudo vi [file]': allows a permitted user to execute a command as the superuser or another user, as specified in the sudoers file.
- To save the file and exit VI(text editor), type :wq and hit enter.
- Restart Caddy: 'sudo service caddy restart'.

<h3>HTML and CSS</h3>

<h5>Hypertext Markup Language</h5>

- The html element represents the top level page structure.
- The head element contains metadata about the page and the page title.
- The body element represents the content structure.
- The main element represents the main content structure, as opposed to things like headers, footers, asides, and navigation content.
-  Attributes describe the specific details of the element.
  - For example, the id attribute gives a unique ID to the element so that you can distinguish it from other elements.
  - The class attribute is another common element attribute that designates the element as being classified into a named group of elements.
- Attributes are written inside the element tag with a name followed by an optional value. 
- You can use either single quotes (') or double quotes (") to delimit attribute values.
- A hyperlink is represented with an anchor (a) element that has an attribute containing the address of the hyperlink reference (href).
  - Example: <a href="https://byu[.]edu">Go to the Y</a>
- HTML defines a header (<!DOCTYPE html>) that tells the browser the type and version of the document.
- Common Elements:
  - html:	The page container
  - head:	Header information
  - title:	Title of the page
  - meta:	Metadata for the page such as character set or viewport settings
  - script:	JavaScript reference. Either a external reference, or inline
  - include:	External content reference
  - body:	The entire content body of the page
  - header:	Header of the main content
  - footer:	Footer of the main content
  - nav:	Navigational inputs
  - main:	Main content of the page
  - section:	A section of the main content
  - aside:	Aside content from the main content
  - div:	A block division of content
  - span:	An inline span of content
  - h<1-9>:	Text heading. From h1, the highest level, down to h9, the lowest level
  - p:	A paragraph of text
  - b:	Bring attention
  - table:	Table
  - tr:	Table row
  - th:	Table header
  - td:	Table data
  - ol,ul:	Ordered or unordered list
  - li:	List item
  - a:	Anchor the text to a hyperlink
  - img:	Graphical image reference
  - dialog:	Interactive component such as a confirmation
  - form:	A collection of user input; input container and submission
  - input:	User input field
  - audio:	Audio content
  - video:	Video content
  - svg:	Scalable vector graphic content; render graphics inline in HTML.
  - iframe:	Inline frame of another HTML page
  - label: individual input label
  - option: selection option
  - select: selection dropdown
  - optgroup: grouped selection dropdown
  - canvas: facilitates 2D drawing and animation.
- Comments for HTML files are created by the placing the comment inbetween '<!-- -->'.
- Special Characters:
  - &	&amp;
  - <	&lt;
  - >	&gt;
  - "	&quot;
  - '	&apos;
  - 😀 &#128512;
- By default a web server will display the HTML file named index.html when a web browser, such as Google Chrome, makes a request without asking for a specific HTML file.

<h5>HTML Structure Elements</h5>

- A block element is meant to be a distinct block in the flow of the content structure.
- An inline element is meant to be inline with the content flow of a block element. They don't disrupt the flow of a block element's content.

<h5>HTML Structure Elements</h5>

- Type of input for 'input' element set with 'type' attribute:
  - text:	Single line textual value
  - password:	Obscured password
  - email:	Email address
  - tel:	Telephone number
  - url:	URL address
  - number:	Numerical value
  - checkbox:	Inclusive selection
  - radio:	Exclusive selection
  - range:	Range limited number
  - date:	Year, month, day
  - datetime-local:	Date and time
  - month:	Year, month
  - week:	Week of year
  - color:	Color
  - file:	Local file
  - submit:	button to trigger form submission
- Most input elements share some common attributes:
  - name:	The name of the input. This is submitted as the name of the input if used in a form
  - disabled:	Disables the ability for the user to interact with the input
  - value:	The initial value of the input
  - required:	Signifies that a value is required in order to be valid
- You can also specify the required attribute on an input element to mark it as requiring a value before it can be submitted.
- When pattern attribute is present, it provides a regular expression that must match for the input to be considered as valid.

<h5>Cascading Style Sheets</h5>

- CSS is primarily concerned with defining rulesets, or simply a rules.
- Rule: comprised of a selector that selects elements to apply the rule to, & one or more declarations that represent the property to style with given property value.
- A number followed by em for font-size will be the default size multiplied by the number.
- CSS can be associated with HTML by using the style attribute of an element and explicitly assign one or more declarations, define CSS rules in the HTML document, or by using the HTML link element to create a hyperlink reference to an external file containing CSS rules. (must appear inthe head element of the document).
- Within an element's box there are several internal boxes:
  - The innermost box holds the element's content. This is where things like the text or image of an element is displayed.
  - Next comes the padding. The padding will inherit things like the background color.
  - After padding is the border, which has properties like color, thickness and line style.
  - The final box is the margin. The margin is considered external to the actual styling of the box and therefore only represents whitespace.
- You can change the box-sizing CSS property from the default value of content-box to border-box in order to redefine the width and height to also include the padding and the border.

<h5>CSS Selectors</h5>

- Element Selectors: selecting an element by name will cascade a declaration down to all the children of that element.
- Wildcard Element Selector (asterisk): selects all of the elements.
- Combinators:
  - Descendant	      A list of descendants	      body section	Any section that is a descendant of a body
  - Child	            A list of direct children	  section > p	  Any p that is a direct child of a section
  - General sibling	  A list of siblings	        p ~ div	      Any p that has a div sibling
  - Adjacent sibling	A list of adjacent sibling	p + div	      Any p that has an adjacent div sibling
- Class Selector: use .[className] to pinpoint a specific element with the given class.
- You can also combine the element name and class selectors to select all paragraphs with a class of summary.
- ID Selector: use # followed by the name of the ID to select an element with that given ID.
- Attribute Selector: element[attribute]
- Psuedo Selector: select based on positional relationships, mouse interactions, hyperlink visitation states, and attributes.
  - Example: section:hover {
                border-left: solid 1em purple;
             }

<h5>CSS Fonts</h5>

- Importing Fonts:
  - In order to have the browser load a font you use the @font-face rule and provide the font name and source location.
  - If you do not want to host font files on your server, then you can load them from a font provider.
    - Example: @import url('https://fonts.googleapis.com/css2?family=Rubik Microbe&display=swap');

<h5>CSS Animation</h5>

- You create CSS animations using the animation properties and defining keyframes for what the element should look like a different times in the animation.
- Specify that we are animating the selected elements by adding the animation-name property with a value of demo. This name refers to the name of the keyframes.
- The keyframes tell what CSS properites should be applied at different key points in the animation sequence.
- Animation-duration property used to  specify how long an animation should last.
- We can use from and to for the defining of the start and end of an animation in @key frames [nameOfAnimation].

<h5>Responsive Design</h5>

- The CSS display property allows you to change how an HTML element is displayed by the browser.
  - Common Options: none (don't display element), block (display this element with a width that fills its parent element), inline (display this element with a width that is only as big as its content), flex (display this element's children in a flexible orientation), & grid (display this element's children in a grid orientation).
- Tell browser to not scale the page: <meta name="viewport" content="width=device-width,initial-scale=1" />
- The float css property moves an element to the left or right of its container element and allows inline elements to wrap around it.
- @media selector dynamically detects the size and orientation of the device and applies CSS rules to represent the structure of the HTML in a way that accommodates the change.

<h3>JavaScript</h3>

<h5>JavaScript Type and Construct</h5>

- JavaScript defines several primitive types:
  - Null:	The type of a variable that has not been assigned a value.
  - Undefined:	The type of a variable that has not been defined.
  - Boolean:	true or false.
  - Number:	A 64 bit signed number.
  - BigInt:	A number of arbitrary magnitude.
  - String:	A textual sequence of characters.
  - Symbol:	A unique value.
- JavaScript defines several object types:
  - Object:	A collection of properties represented by name value pairs. Values can be of any type.	{a:3, b:'fish'}
  - Function:	An object that has the ability to be called.	function a() {}
  - Date:	Calendar dates and times.	new Date('1995-12-17')
  - Array:	An ordered sequence of any type.	[3, 'fish']
  - Map:	A collection of key value pairs that support efficient lookups.	new Map()
  - JSON:	A lightweight data-interchange format used to share information across programs.	{"a":3, "b":"fish"}
- JS supports concatenation with '+' and equality with '==='.
- JavaScript is a weakly typed language. That means that a variable always has a type, but the variable can change type when it is assigned a new value, or that types can be automatically converted based upon the context that they are used in.
- Also supports loops used in other languages like for, while, and do while.
- But it has some other loops that are similar:
  - The for in statement iterates over an object's property names.
    - For arrays the object's name is the array index.
  - The for of statement iterates over an iterable's (Array, Map, Set, ...) property values.

<h5>JavaScript String</h5>

- A string variable is specified by surround a sequence of characters with single quotes ('), double quotes ("), or backticks.
- Single and double quotes have an equivalent meaning while backticks define string literals that may contain JavaScript which is evaluated in place and concatenated into the string. 
- A string literal is declared with a dollar sign followed by a curly brace pair.
- Useful String Functions:
  - length:	The number of characters in the string
  - indexOf:	The starting index of a given substring
  - split:	Split the string into an array on the given delimiter string
  - startsWith:	True if the string has a given prefix
  - endsWith:	True if the string has a given suffix
  - toLowerCase:	Converts all characters to lowercase

<h5>Functions</h5>

- JavaScript functions are first class objects: they can be assigned a name, passed as a parameter, returned as a result, and referenced from an object or array.
- If a parameter isn't provided to the function when called, then the parameter is undefined.
- A function can assign default values to its parameters by appending '=' and the value desired after the name of the parameter(s).
- Functions can be defined anonymously, or without a name, by including them inside of other things like function calls, variable declarations, or returns.
- They can also be placed inside of other functions so that you can modularize your code without exposing private details.

<h5>Arrow Functions</h5>

- With the ability to pass functions anonymously, things can begin to get cluttered. So to replace the function keyword, you can use => instead.
- The arrow functions canot be used for contructors or iterator generators.
- Return keyword is optional if no cury braces are provided and only a single expression is used.
- The result of that single expression is returned unless encased by curly brackets which then would behave like a standard function.
- Inherit this pointer from the scope of where it is created which makes what is called a closure: allows a function to continue referencing its creation scope even after it has passed out of that scope.
- Closures provide a valuable property when we do things like execute JavaScript within the scope of an HTML page, because it can remember the values of variables when the function was created instead of what they are when they are executed.

<h5>Arrays</h5>

- Static Array Functions:
  - push:	Add an item to the end of the array	~ a.push(4)
  - pop:	Remove an item from the end of the array ~ x = a.pop
  - slice:	Return a sub-array ~ a.slice(1,-1)
  - sort:	Run a function sort an array in place	~ a.sort((a,b) => b-a)
  - values:	Creates an iterator for use with a for of loop ~ for (i of a.values()) {...}
  - find:	Find the first item satisfied by a test function ~ a.find(i => i < 2)
  - forEach:	Run a function on each array item	~ a.forEach(console.log)
  - reduce:	Run a function to reduce each array item to a single item	~ a.reduce((a, c) => a + c)
  - map:	Run a function to map an array to a new array	~ a.map(i => i+i)
  - filter:	Run a function to remove items ~ a.filter(i => i%2)
  - every:	Run a function to test if all items match	~ a.every(i => i < 3)
  - some:	Run a function to test if any items match	~ a.some(i => 1 < 1)

<h5>JavaScript Objects and Classes</h5>

- A JavaScript object represents a collection of name value pairs referred to as properties.
- The property name must be of type String or Symbol, but the value can be of any type.
  - Example: const person = { name: 'John', age: 20 };
- Each property name before colons is an identifier (either a name, a number, or a string literal).
- Once it is created, you can add any properties to the object by calling object.[newPropertyName] and setting it equal to something.
- You can also declare a variable of object type with the object-literal syntax; allows you to provide the initial composition of the object.
- Static Object Functions:
  - entries:	Returns an array of key value pairs
  - keys:	Returns an array of keys
  - values:	Returns an array of values
- Any function that returns an object is considered a constructor and can be invoked with the new operator.
- Because objects can have any type of property value you can create methods on the object as part of its encapsulation.
- You can make properties and functions of classes private by prefixing them with a #.
- Classes can be extended by using the extends keyword to define inheritance.
- Parameters that need to be passed to the parent class are delivered using the super function.
- Any functions with the same name defined at the child level override the parent's implementation of those same functions.

<h5>JSON</h5>

- JSON Document Can Contain Many Data Types:
  - string:	"crockford"
  - number:	42
  - boolean:	true
  - array:	[null,42,"crockford"]
  - object:	{"a":1,"b":"crockford"}
  - null:	null
- Most commonly, a JSON doc contains an object: they contain zero or more key value pairs where the key is always a string and the value must be valid JSON value.
- Key-value pairs are delimited with commas; curly braces delimit an object, square brces and commas delimit arrays, and strings are always delimited with ".
- You can convert JSON to, and from, JavaScript using the JSON.parse and JSON.stringify functions.
- JSON cannot represent undefined objects, so it gets dropped when converting JS to JSON.

<h5>JavaScript Regular Expressions</h5>

- Regular expressions: textual pattern matchers; patterns used to match character combinations in strings.
- You can use them to find text in a string so that you can replace it, or simply know that it exists.
- You can create a regular expression using the class constructor or a regular expression literal:
  - const objRegex = new RegExp('ab*', 'i');
  - const literalRegex = /ab*/i;
- String class has several functions that accept regular expressions which includes match, replace, search, and split.
  - match: retrieves the result of matching a string against a regular expression.
  - replace: returns a new string with one, some, or all matches of a pattern replaced by a replacement.
  - search: executes a search for a match between a regular expression and this String object.
  - split: takes a pattern and divides a String into an ordered list of substrings by searching for the pattern, puts these substrings into an array, and returns the array.
- For a quick test to see if there is a match you can use the regular expression object’s “test” function.
- Regex Flags:
  - g: Global search
  - i: Case-insensitive search
  - m: Multi-line search
  - y: "sticky" search match starting at current position in target string

<h5>JavaScript Rest and Spread</h5>

- Rest Syntax: prefix the last parameter of any function with three periods to make it a rest parameter.
- This enables you to call it with any number of parameters which are all automatically combined into an array.
- Spread: prefix an array or string with three dots when sending it to a function.
- It takes an object that is iterable (e.g. array or string) and expands it into a function's parameters.

<h5>JavaScript Destructuring</h5>

- Destructuring: the process of pulling individual items out of an existing one, or removing structure. (can be done with arrays or objects)
- Example: const a = [1, 2, 3, 4]; -> const [b, c] = a; -> console.log(b, c); //Outut: 1, 2
- You can also combine multiple items from the original object using rest syntax.
- When object destructuring, you explicitly specify the properties you want to pull from the source object.
- You can also map the names to new variables instead of just using the original property names.

<h5>Scope</h5>

- JavaScript has four different types of scope:
  - Gobal: Visible to all code
  - Module: Visible to all code running in a module
  - Function: Visible within a function
  - Block: Visible within a block of code delimited by curly braces
- There are three different context that this can refer to:
  - Global - When this is referenced outside a function or object it refers to the globalThis object. The globalThis object represents the context for runtime environment. For example, when running in a browser, globalThis refers to the browser's window object.
  - Function - When this is referenced in a function it refers to the object that owns the function. That is either an object you defined or globalThis if the function is defined outside of an object. Note that when running is JavaScript strict mode, a global function's this variable is undefined instead of globalThis.
  - Object - When this is referenced in a object it refers to the object.
- A closure is defined as a function and its surrounding state; whatever variables are accessible when a function is created are available inside of that function.

<h5>JavaScript Modules</h5>

- Because modules create a file-based scope for the code they represent, you must explicitly export the objects that you want to be visible outside the module.
- You can import a module’s exported function into another module using “import”.
  - Example: import { alertDisplay } from './alert.js';
- The key thing to understand is that modules can only be called from other modules. You cannot import a module object into a globally scoped JavaScript file.

<h5>Document Object Model</h5>

- The Document Object Model (DOM) is an object representation of the HTML elements that the browser uses to render the display.
- You can provide a CSS selector to the querySelectorAll function in order to select elements from the document.
- textContent property: contains all of the element's text.
- innerHTML property: a textual representation of an element's HTML content.
- o create a new element you first create the element on the DOM document. You then insert the new element into the DOM tree by appending it to an existing element in the tree.
- To delete elements call the removeChild function on the parent element.
- All DOM elements support the ability to attach a function that gets called when an event occurs on the element. (event listeners)
- Commonly Used Events:
  - Clipboard:	Cut, copied, pasted
  - Focus:	An element gets focus
  - Keyboard:	Keys are pressed
  - Mouse:	Click events
  - Text: selection	When text is selected
- You can also add event listeners directly in the HTML using the onclick handler.

<h5>Promises</h5>

- You can asynchronously execute code with the use of a JavaScript Promise.
- Because the execution is asynchronous the promise object can be in one of three states at any given point in time:
  - pending - Currently running asynchronously
  - fulfilled - Completed successfully
  - rejected - Failed to complete
- You create a promise by calling the Promise object constructor and passing it an executor function that runs the asynchronous operation.
- Executing asynchronously means that promise constructor may return before the promise executor function runs.
- The setTimeout function takes the number of milliseconds to wait and a function to call after that amount of time has expired.
- The promise executor function takes two functions as parameters, resolve and reject.
- Calling resolve sets the promise to the fulfilled state, and calling reject sets the promise to the rejected state.
- The promise object has three functions: then, catch, and finally.
  - The then function is called if the promise is fulfilled.
  - The catch is called if the promise is rejected.
  - The finally is always called after all the processing is completed.

<h5>JavaScript Async/Await</h5>

- The await keyword wraps the execution of a promise and removed the need to chain functions.
- The await expression will block until the promise state moves to fulfilled, or throws an exception if the state moves to rejected.
- We can create equivalent executions with either a promise then/catch chain, or an await with a try/catch block.
- One important restriction for working with await is that you cannot call await unless it is called at the top level of the JavaScript, or is in a function that is defined with the async keyword.
- The async keyword transforms the function so that it returns a promise that will resolve to the value that was previously returned by the function.
- This turns any function into an asynchronous function, so that it can in turn make asynchronous requests.
- Adding async to a function will either return a default promise containing the return of the function or explicity create a promise instead of the automatically generated promose that the async keyword generates.
- The await keyword wraps a call to the async function, blocks execution until the promise has resolved, and then returns the result of the promise.
- If we prefix the call to the function with the await keyword, execution will stop until the promise has resolved, at which point the result of the promise is returned instead of the actual promise object.

<h3>Web Services</h3>

<h5>Introduction</h5>

- To make a web service request, we supply the URL of the web service to the fetch function that is built into the browser.
- Generally the functions provided by a web service are called endpoints, or sometimes APIs.

<h5>URL</h5>

- The Uniform Resource Locator (URL) represents the location of a web resource. A web resource can be anything, such as a web page, font, image, video stream, database record, or JSON object. It can also be completely ephemeral, such as a visitation counter, or gaming session.
- <scheme>://<domain name>:<port>/<path>?<parameters>#<anchor>
- Scheme: The protocol required to ask for the resource. For web applications, this is usually HTTPS. But it could be any internet protocol such as FTP or MAILTO.
- Domain name: The domain name that owns the resource represented by the URL.
- Port: The port specifies the numbered network port used to connect to the domain server. Lower number ports are reserved for common internet protocols, higher number ports can be used for any purpose. The default port is 80 if the scheme is HTTP, or 443 if the scheme is HTTPS.
- Path: The path to the resource on the domain. The resource does not have to physically be located on the file system with this path. It can be a logical path representing endpoint parameters, a database table, or an object schema.
- Parameters: (example: filter=names&highlight=intro,summary) The parameters represent a list of key value pairs. Usually it provides additional qualifiers on the resource represented by the path. This might be a filter on the returned resource or how to highlight the resource. The parameters are also sometimes called the query string.
- Anchor: The anchor usually represents an sub-location in the resource. For HTML pages this represents a request for the browser to automatically scroll to the element with an ID that matches the anchor. The anchor is also sometimes called the hash, or fragment ID.
- A Uniform Resource Name (URN) is a unique resource name that does not specify location information. (example: urn:isbn:10,0765350386)
- A Uniform Resource Identifier (URI) is a general resource identifier that could refer to either a URL and URN.

<h5>Port</h5>
  
- Port numbers allow a single device to support multiple protocols (e.g. HTTP, HTTPS, FTP, or SSH) as well as different types of services (e.g. search, document, or authentication).
- The ports may be exposed externally, or they may only be used internally on the device.
- For example, the HTTPS port (443) might allow the world to connect, the SSH port (22) might only allow computers at your school, and a service defined port (say 3000) may only allow access to processes running on the device.
- Ports from 0 to 1023 represent standard protocols. Generally a web service should avoid these ports unless it is providing the protocol represented by the standard.
- Ports from 1024 to 49151 represent ports that have been assigned to requesting entities. However, it is very common for these ports to be used by services running internally on a device.
- Ports from 49152 to 65535 are considered dynamic and are used to create dynamic connections to a device.
- Port - 20:	File Transfer Protocol (FTP) for data transfer
- Port - 22:	Secure Shell (SSH) for connecting to remote devices
- Port - 25:	Simple Mail Transfer Protocol (SMTP) for sending email
- Port - 53:	Domain Name System (DNS) for looking up IP addresses
- Port - 80:	Hypertext Transfer Protocol (HTTP) for web requests
- Port - 110:	Post Office Protocol (POP3) for retrieving email
- Port - 123:	Network Time Protocol (NTP) for managing time
- Port - 161:	Simple Network Management Protocol (SNMP) for managing network devices such as routers or printers
- Port - 194:	Internet Relay Chat (IRC) for chatting
- Port - 443:	HTTP Secure (HTTPS) for secure web requests

<h5>HTTP</h5>

- When a web client (e.g. a web browser) and a web server talk they exchange HTTP requests and responses. The browser will make an HTTP request and the server will generate an HTTP response.
- GET:	Get the requested resource. This can represent a request to get a single resource or a resource representing a list of resources.
- POST:	Create a new resource. The body of the request contains the resource. The response should include a unique ID of the newly created resource.
- PUT:	Update a resource. Either the URL path, HTTP header, or body must contain the unique ID of the resource being updated. The body of the request should contain the updated resource. The body of the response may contain the resulting updated resource.
- DELETE:	Delete a resource. Either the URL path or HTTP header must contain the unique ID of the resource to delete.
- OPTIONS:	Get metadata about a resource. Usually only HTTP headers are returned. The resource itself is not returned.
- 1xx: Informational.
- 2xx: Success.
- 3xx: Redirect to some other location, or that the previously cached resource is still valid.
- 4xx: Client errors. The request is invalid.
- 5xx: Server errors. The request cannot be satisfied due to an error on the server.
- 100	Continue	            The service is working on the request
- 200	Success	              The requested resource was found and returned as appropriate.
- 201	Created	              The request was successful and a new resource was created.
- 204	No Content	          The request was successful but no resource is returned.
- 304	Not Modified	        The cached version of the resource is still valid.
- 307	Permanent redirect	  The resource is no longer at the requested location. The new location is specified in the response location header.
- 308	Temporary redirect	  The resource is temporarily located at a different location. The temporary location is specified in the response location header.
- 400	Bad request	          The request was malformed or invalid.
- 401	Unauthorized	        The request did not provide a valid authentication token.
- 403	Forbidden	            The provided authentication token is not authorized for the resource.
- 404	Not found	            An unknown resource was requested.
- 408	Request timeout	      The request takes too long.
- 409	Conflict	            The provided resource represents an out of date version of the resource.
- 418	I'm a teapot	        The service refuses to brew coffee in a teapot.
- 429	Too many requests	    The client is making too many requests in too short of a time period.
- 500	Internal server error	The server failed to properly process the request.
- 503	Service unavailable	  The server is temporarily down. The client should try again with an exponential back off.
- Authorization	              (Bearer bGciOiJIUzI1NiIsI)	A token that authorized the user making the request.
- Accept	                    (image/*)	                              What content format the client accepts. This may include wildcards.
- Content-Type	              (text/html; charset=utf-8)	            The format of the response content. These are described using standard MIME types.
- Cookie	                    (SessionID=39s8cgj34; csrftoken=9dck2)	Key value pairs that are generated by the server and stored on the client.
- Host	                      (info.cern.ch)	                        The domain name of the server. This is required in all requests.
- Origin	                    (cs260.click)	                          Identifies origin that caused the request; host may only allow requests from specific origins.
- Access-Control-Allow-Origin	(https://cs260.click	                  Server response of what origins can make a request. This may include a wildcard.
- Content-Length	            (368)	                                  The number of bytes contained in the response.
- Cache-Control	              (public, max-age=604800)	              Tells the client how it can cache the response.
- User-Agent	                (Mozilla/5.0 (Macintosh)	              The client application making the request.
- The format of the body of an HTTP request or response is defined by the Content-Type header. A client may specify what formats it accepts using the accept header.
- This means that one HTTP request does not know anything about a previous or future request. However, that does not mean that a server or client cannot track state across requests. 
- One common method for tracking state is the cookie. Cookies are generated by a server and passed to the client as an HTTP header.
- The client then caches the cookie and returns it as an HTTP header back to the server on subsequent requests.
- This allows the server to remember things like the language preference of the user, or the user's authentication credentials.
- A server can also use cookies to track, and share, everything that a user does.

<h5>SOP & CORS</h5>

- When website architecture and browser clients were still in their infancy they allowed JavaScript to make requests from one domain while displaying a website from a different domain. These are called cross-origin requests.
- Simply stated SOP (Same Orgin Policy) only allows JavaScript to make requests to a domain if it is the same domain that the user is currently viewing.
- CORS (Cross Origin Resource Sharing) allows the client (e.g. browser) to specify the origin of a request & then let the server respond with what origins are allowed.
- If the server doesn't specify what origin is allowed then the browser assumes that it must be the same origin.
- However, if you want to make requests to a different domain than the one your web application is hosted on, then you need to make sure that domain allows requests as defined by the Access-Control-Allow-Origin header it returns.
- Make sure they are responding with * or your calling origin. If they do not then you will not be able to use them.
  
<h5>Fetch</h5>

- The basic usage of fetch takes a URL and returns a promise. The promise then function takes a callback function that is asynchronously called when the requested URL content is obtained. If the returned content is of type application/json you can use the json function on the response object to convert it to a JavaScript object.
- fetch('https://jsonplaceholder[.]typicode[.]com/posts', {
  method: 'POST',
  body: JSON.stringify({
    title: 'test title',
    body: 'test body',
    userId: 1,
  }),
  headers: {
    'Content-type': 'application/json; charset=UTF-8',
  },
})
  .then((response) => response.json())
  .then((jsonResponse) => {
    console.log(jsonResponse);
  });

<h5>Service Design</h5>

- Remote Procedure Calls(RPC): expose service endpoints as simple function calls. RPC usually just leverages the POST HTTP verb. The actual verb and subject of the function call are represented by the function name. The name of the function is either a whole URL path or a parameter in the POST body. Maps directly to the function calls in service but also exposes the inner workings of the service.
- Representational State Transfer (REST): REST HTTP verbs always act on a resource. Operations on these resources alter and impact the state of the resource as it is transferred by a REST endpoint call.
- GraphQL: focuses on data manipulation instead of function calls and resources. It is centralized on a query that specifies the desired data and how it should be joined and filtered.
-  
  
  
