# The Chatrooms - Stream 3 Final Project (https://chatroom-client.herokuapp.com)

## Description
The Chatrooms. A place where you can meet and chat to people that share a common interest with yourself with real-time messaging. 

### Why I chose this project! 
With a year expierence in a junior .NET development role, I decided to choose the instant-messaging website to try test my abilites with something challenging. While I am not 100% happy with the outcome of the project due to time constraints, I feel alot more confident that I would be able to get involved with more complicated projects in the future.

### Who/What is this app for?
The Chatrooms is for anyone and everyone. Sign up, join a room that interests you, if there are none available and you have a subscription, create one. Start chatting. It is as simple as that.

### Current Features. 
Users:
    -   User Account: User can register for an account. User can edit their profile, choose a profile picture. This image will show beside evey User message posted. 
    -   General Room: On a successful registration, the user will be signed up to the general room.  
    -   Paymentn: A single payment provides the user the ability to create an unlimited number of rooms, although I planned to implement a limit of 20 for a payment. 

Chatrooms:
    -   Displays a list of messages between all users from a chatroom.
    -   When user scrolls to top of screen, will append another batch of messages to the list. 
    -   Searching. There is the ability to search for rooms.


### Features I would have liked to implement.
The main reason thee features have been left out is due to time. 

    -   Private Messaging: I really would have liked to implement this feature. I couldn't find a nice way of implementing the private room. 
    -   There are parts where a callback message displayed to the user would be useful. 

### Some Development Issues I don't have time to fix
Due to time constraints in work and project deadline creeping up fast I have not been able to fix the following features.

    -   Pasword Reset: I have implemented a password reset functionality from the home page. THis requires Django Rest-Auth sending a reset email. In debug mode it will print the email that would be sent to the debug console. Not much use there but the best I can do at the moment. 
    -   The UI - While I have made some effort to make this app mobile friendly, it has been primarily designed to be used on desktop. It is semi responsive on a mobile device but could be better. Again due to time constraints, and some of the site functionality not working properly (some still not doing as required) I have had to sacrifice 
    - User Id Undefined - Very rarely, when switching between the navbar tabs, the user stored in cookies will sometime get deleted. Not sure why this happens. 
    -   Searching: Rooms a user is already part should not included, unfortunately there was an issue after a rebuild and this functionality is tempermental.


## Tech Used

### Some the tech used includes:
- [AngularJs](https://angularjs.org/)
    - Used AngularJs to build the front-end of the website.
- [Bootstrap](http://getbootstrap.com/)
    - Used **Bootstrap** to give our project a simple, responsive layout
- [Bootswatch](https://bootswatch.com/superhero/)
    - Used **Bootswatch** theme "Superhero" with the google font Kanit for the style of the site
- [Nodemon](https://nodemon.io)
    -  Nodemon will continually monitor your applications source code for changes and automatically restarts your server if any changes are detected.
- [Bower](https://bower.io/)
    - Used for applying databaase migrations. Any changes to the Models could easily be applied to the database with this package
- [Angular-Payments](https://github.com/laurihy/angular-payments)
    - Provides validation and formatting of paymnets form.  
- [ng-file-upload](https://github.com/danialfarid/ng-file-upload/blob/master/README.md#full-reference)
    - Simple directive to make the uploadinf of profile images easy. 
- [socket.io](https://socket.io/)
    - Socket.io has been choosen to handle the real-time messaging in the chatrooms. 
- [Github](https://github.com)
    - Used for version control
- [Heroku](https://heroku.com)
    - Used to deploy the website.

### Getting the code up and running
1. Firstly you will need to clone both repositories by running the ```https://github.com/horan5034/chatroom-client.git``` command in a folder that will house the projects.
2. To get the front-end up and running you will need to make sure that you have **npm** and **bower** installed
  1. You can get **npm** by installing Node from [here](https://nodejs.org/en/)
  2. Once you've done this you'll need to run the following command:
     `npm install -g bower # this may require sudo on Mac/Linux`
3. When all dependencies have been installed, start the app by running node server.js or nodemon server.js (if you have nodemon installed (https://nodemon.io/)  npm install -g nodemon)

Credits: 
    Credit for loading spinner http://tobiasahlin.com/spinkit/
    I have used Bootswatch Theme (credit is also acknowledged at the top of the bootstrap.css file in the static folder)
