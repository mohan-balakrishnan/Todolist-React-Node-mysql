# Todolist-React-Node-mysql

## Simple Todo List with Tech Stack **NodeJs, ReactJs, Mysql, JWT, Javascript**

1. **Create a Windows instance**: Allow required ports in security group (`80, 8080, 3000, 3306`).
   - Connect Windows Instance via `Remote Desktop Connection(RDP)`.
   - Install `Node.js`.

2. **Create a RDS Mysql database version 8.***  - Free Tier only.
    - Ensure that the security group associated with the database allows access to port number `3306` from `anywhere`.
    - Confirm that the database is `publicly accessible`. For example, verify this by attempting to connect to the database using a MySQL client from an Your Local PC.)

3. **Connect RDS database in mysql client app**:
   - **Import** the Database. Database dump available in `database_schema` directory.
   - Database schema path: `Todolist-React-Node-mysql/database_schema/dump.sql`.

5. **Download codebase to server from this repo (or)**: [Click here to download code](https://codeload.github.com/mohan-balakrishnan/Todolist-React-Node-mysql/zip/refs/heads/main).

6. Unzip the code.

7. **Modify the db details** (Endpoint, username, password, database name) in the codebase:
   - Path: `Todolist-React-Node-mysql\database\db.js`.
   - Refer to line no. 5 and 8.
   - Example:
     ```javascript
     const sequelize = new Sequelize('Your-DB-Name', 'UserName', 'Password',
     host: 'YourEndpoint',
     ```

## Backend(Todolist-React-Node-mysql) - NodeJs, Mysql, JWT

8. Go to `Todolist-React-Node-mysql` folder, open command prompt.
   - Install all packages by running `npm i`.
   - Run `npm run dev`.

## Frontend(Todolist-React-Node-mysql/frontend) - ReactJs

9. Go to `Todolist-React-Node-mysql/frontend` folder, open command prompt.
   - Run `npm i`.
   - Run `npm start`.
   - Open [http://localhost:3000](http://localhost:3000) to see the app or http://publicip:3000.
   - Map ip to [Free DNS](https://www.noip.com/) and confirm it. 

10. Register a new user and login with that user in the application. Verify the user in the DB table.

(Note: If you don't see the newly created user in the database or are unable to login, please double-check the database connection details in the `database\db.js` file.)

## Screenshots

![Home Page](https://raw.githubusercontent.com/mohan-balakrishnan/Todolist-React-Node-mysql/main/home.JPG)

![Register](https://raw.githubusercontent.com/mohan-balakrishnan/Todolist-React-Node-mysql/main/register.JPG)
