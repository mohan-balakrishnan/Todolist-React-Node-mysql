# Todolist-React-Node-mysql


## Simple Todo List with technology stack NodeJs, ReactJs, Mysql, JWT, Javascript

1. Create a windows instance - Install Node.js, allow required ports (80,8080,3000,3306)

2. Create a RDS Mysql databse 5.7.** 

3. connect RDS database in mysql client app -> import the Database, Database dump available in database_schema directory. Open sql file in text editor -> copy queries and run in mysql client.

4. Download codebase to server from this repo (or)  [Click here to download code](https://codeload.github.com/mohan-balakrishnan/Todolist-React-Node-mysql/zip/refs/heads/main)

5. Unzip the code

6. modify the db details(endpoint, username, password, database name) in code base in the following path : `Todolist-React-Node-mysql\database\db.js`  refer line no. 5 and 8.
   
  eg: 
      
      const sequelize = new Sequelize('Db Name', 'Username', 'Password',
      host: 'YourEndpoint',


## Backend(Todolist-React-Node-mysql) - NodeJs, Mysql, JWT

go to `Todolist-React-Node-mysql` folder open command prompt

Install all package by running `npm i`   

Run `npm run dev`


## Frontend(Todolist-React-Node-mysql/frontend) - ReactJs

go to `Todolist-React-Node-mysql/frontend` folder  open command prompt

Run `npm i`

Run `npm start`

Open http://localhost:3000  to see the app or http://publicip:3000

Register a new user and login with that user in application. verify the user in db

## Screenshots

![Home Page](https://raw.githubusercontent.com/mohan-balakrishnan/Todolist-React-Node-mysql/main/home.JPG)

![Register](https://raw.githubusercontent.com/mohan-balakrishnan/Todolist-React-Node-mysql/main/register.JPG)
