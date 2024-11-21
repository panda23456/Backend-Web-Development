Project: Doing Tasks to earn points and get Pets

Brief Description: Players have to register for an account(s), then create User(s) to start the game.
User can do tasks in order to earn points.
Points can be used to buy new pets or feed pets to level them up.
There is a messaging page for users to post messages to which all other users can see.
All other players can also see which other accounts are registered.

## Prerequisites

Before you run this project, ensure you have the following installed on your machine:

- [Node.js](https://nodejs.org/) (v14.17.5 or higher)
- [npm](https://www.npmjs.com/) (Node Package Manager)
- [MySQL](https://www.mysql.com/) database

### Dependencies

This project relies on the following Node.js packages. Make sure to install them using npm:

- [bcrypt](https://www.npmjs.com/package/bcrypt) (Version ^5.1.1)
- [dotenv](https://www.npmjs.com/package/dotenv) (Version ^16.3.2)
- [express](https://www.npmjs.com/package/express) (Version ^4.18.2)
- [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken) (Version ^9.0.2)
- [mysql2](https://www.npmjs.com/package/mysql2) (Version ^3.7.1)
- [nodemon](https://www.npmjs.com/package/nodemon) (Version ^3.0.3)

You can install these dependencies by running:

bash
npm install
//

Usage: Explain how to use your application.
First, click the Register button on the top right to register for an account.
Enter your Username, Email, Password and Confirm password to register for an account
Then, you will be logged in and redirected to the NavBar(Profile) page to create a new User for the registered Account

After User creation, go to the navBar , click on Users > View Details to access User Details and User Actions
Here, User Info, User Actions, User Pets will be displayed.

NavBar(Users > View Details)
User Info - User ID, Username and Points
User Actions - Change Username, Delete User, Perfom Task, Buy Pet, Feed Pet, Post Message
User Pets - Pets will be displayed if User Owns Any

User Actions
Change Username- User can change their username
Delete User- User can delete their User
Peform Task- User can perform different tasks to earn points
Buy Pet - User can spend points from doing tasks to buy pets from a Pet Shop (User can own multiple of the same pet, and more than one pet)
Feed Pet- User can spend 10 points to feed a pet(Pet increases by 1 level for each feed, where max level is 3)
Post Message - User can post multiple message to the Message Page
Delete Pet - User can pick which pet to Delete
Update Message- Users can update/Delete their posted message

Upon purchasing a pet,the Pet will show up under User Pets when viewing Users > View Details(if user can afford)
Upon feeding a pet, the Pet will level up by 1 level and upgrade its pet ability and be updated when viewing Users > View Details(if user can afford and pet can level)

NavBar(Home)
Show all pets created after running npm run init_tables

NavBar(Pets)
Also shows all pets created after running npm run init_tables

NavBar(Tasks)
Show all tasks created after running npm run init_tables

NavBar(Accounts)
Shows all registerd accounts and their created users

NavBar(Messaging Page)
Shows all messages posted by all Users
Filter option to filter out messages only posted by a specific User

NavBar(Logout)
Ends session with currently logged in Account

NavBar(Master Ball img)
Redirects to NavBar(Home) page

Unauthorized users be be redirected(Accessing someone else's user/ invalid token) etc.
When token expires after 15mins, users will be logged out of their account and redirected to the Home page.

//
License: PokeAPI for Pokemon Pet images
