# What is LLAVER? :mag_right:
Finish date: 23-04-22 :date:
LLaver is an attempt of automation for the geriatric exam "Menti", also, it provides a system for manage and analyse the data results of the examns. 

## How did we create the backend? :construction:
- We developed the backend in `Nodejs` with `express`
- The database used was MySQL.
- For the project we implement a basic authentication system, using a **local strategy** (email and password stored in our database), we encrypted the password with `Bcrypt`.
- For persistence of session user, we use `JWT`.
- The backend was deployed in `Heroku`.

## Usage :memo:
1- If the database doesn't existe run the script located in: *conection_store > database.sql.*

2 - Set the environment variables in *config.js*
    
    > api: {
    >    port: process.env.PORT || 3002  
    > },
    > frontend: {
    >    port: process.env.PORT || 3000
    > },
    > mysql: {
    >    host: process.env.MYSQL_HOST || <YOUR_HOST>,
    >    database: process.env.MYSQL_DATABASE || <YOUR_DATABASE>,
    >    user: process.env.MYSQL_USER || <YOUR_USER>,
    >    password: process.env.MYSQL_PASSWORD || <YOUR_PASSWORD>
    > },
    > jwt: {
    >    key: <YOUR_KEY>,
    >    time: <EXPIRATION_TOKEN_TIME>
    > },
    >hash: {
    >    times: <TIME_TO_HASH_BYCRP>
    > } 
   
3 - Install the dependencies: npm install 

4 - Run the project `node index.js` (Be careful of be in the project directory)

## Deploy in heroku :computer:
Create your repository on heroku and follow the instructions.
