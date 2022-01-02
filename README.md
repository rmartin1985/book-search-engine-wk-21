# Book Search Engine Week 21

  ![](https://img.shields.io/badge/license-MIT-blue)

  ## Description
 This week we were challenged to refactor an exisiting Book Search Engine from a RESTful API to a GraphQL API built with Apollo Server.

 The starter code had everything working correctly so the main challenge was to go through all of the code and change the necessary files to use Apollo server and GraphQL correctly. 

 After ensuring that the necessary dependencies were installed correctly and refactoring the middleware to make sure that the authentication would work with GraphQL, the next step was to create the schemas files. 

 In the the typeDefs.js file, the type definitions were declared. The Docs for the GrahpQL were needed to understand how to use the 'input type", specifically for the SavedBooks array. It comes in handy when creating an object in a database and updating an object in a database take the same parameters. Made updating the savedBooks array much simpler.

 Next step was to create the resolvers in their own separate file. This is where the query and mutations were defined according to the type definitions. Using the starter code as a guide, the resolvers were written to ensure that the same data was being accessed and displayed to the page. 

 Once the backend was done, the front end came next. Had to go through several files and import the correct hooks to each file and then refactor the code to use the queries and mutations that were written as opposed to the original RESTful api routes that were written.

 Once everything worked as it should, I removed all of the files that were no longer needed from the starter code. 

 On a final glance, I noticed that the acceptance criteria mentioned that a link to Google Books should be displayed as well for the search results. The starter code didn't have this displaying anywhere. I looked up the API call JSON results and determined the correct info needed and added that to display now for each book that comes up. 

 Please feel free to keep scrolling for more info on how to install this locally on your computer or for other information regarding the creation of this app.

  ## Table of Contents
  1. [Installation](##installation)
  2. [User Story](#user-story)
  3. [Acceptance Criteria](#acceptance-criteria)
  4. [Deployed Application](#deployed-application)
  5. [Demo](#demo)
  6. [Technology](#technology)
  7. [Questions](#questions)
  8. [License](#license)
  

  ## Installation
  1. Fork this repository
  2. Clone repository to your local directory
  3. Make sure you have installed Node.js 
  4. Run npm install to install the necessary dependencies
  ```
  npm install
  cd client/
  npm install
  cd ../
  cd server
  npm install
  cd ../
  ```
  5. Run npm run develop to get a development version of the app to inspect and test out
  ```
  npm run develop
  ```

  ## User Story
  ```
  AS AN avid reader
  I WANT to search for new books to read
  SO THAT I can keep a list of books to purchase 
  ```
  ## Acceptance Criteria
  ```
  GIVEN a book search engine
  WHEN I load the search engine
  THEN I am presented with a menu with the options Search for Books and Login/Signup and an input field to search for books and a submit button
  WHEN I click on the Search for Books menu option
  THEN I am presented with an input field to search for books and a submit button
  WHEN I am not logged in and enter a search term in the input field and click the submit button
  THEN I am presented with several search results, each featuring a book’s title, author, description, image, and a link to that book on the Google Books site
  WHEN I click on the Login/Signup menu option
  THEN a modal appears on the screen with a toggle between the option to log in or sign up
  WHEN the toggle is set to Signup
  THEN I am presented with three inputs for a username, an email address, and a password, and a signup button
  WHEN the toggle is set to Login
  THEN I am presented with two inputs for an email address and a password and login button
  WHEN I enter a valid email address and create a password and click on the signup button
  THEN my user account is created and I am logged in to the site
  WHEN I enter my account’s email address and password and click on the login button
  THEN I the modal closes and I am logged in to the site
  WHEN I am logged in to the site
  THEN the menu options change to Search for Books, an option to see my saved books, and Logout
  WHEN I am logged in and enter a search term in the input field and click the submit button
  THEN I am presented with several search results, each featuring a book’s title, author, description, image, and a link to that book on the Google Books site and a button to save a book to my account
  WHEN I click on the Save button on a book
  THEN that book’s information is saved to my account
  WHEN I click on the option to see my saved books
  THEN I am presented with all of the books I have saved to my account, each featuring the book’s title, author, description, image, and a link to that book on the Google Books site and a button to remove a book from my account
  WHEN I click on the Remove button on a book
  THEN that book is deleted from my saved books list
  WHEN I click on the Logout button
  THEN I am logged out of the site and presented with a menu with the options Search for Books and Login/Signup and an input field to search for books and a submit button

  ```

  ## Deployed Application
  Please click the following link  to be taken to a Heroku app of this application: 
  [Book-Search-Engine](https://pacific-dawn-01756.herokuapp.com/)

  ## Demo
  Below are gifs of the app in action! 

  ![Search for books](https://media.giphy.com/media/0aOwKSHqRlVdleBwJi/giphy.gif)

  ![Login/Signup](https://media.giphy.com/media/KYjYy12yixCai0NsHr/giphy.gif)

  ![Add books/Delete books](https://media.giphy.com/media/Rj8mCBUorwwHHL2hVk/giphy.gif)

  ## Technology Used
  **1. [Node.js](https://nodejs.org/en/)**

  **2. [MongoDB](https://www.mongodb.com)**

  **3. [Mongoose ODM](https://mongoosejs.com/)**

  **4. [Apollo Client](https://www.apollographql.com/docs/react/)**

  ## Questions

  If you have any questions regarding this project, you can reach me at my GitHub account or by email at:
  <br />
  Github: [rmartin1985](https://github.com/rmartin1985)
  <br />
  Email: rickmartinatx@gmail.com

  ## License
  Licensed under the [MIT License](LICENSE)
