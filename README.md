# E-commerce Back End

## Project Description
This project sets up a back end for a simple e-commerce site with a database containing tables for categories of products, products, and descriptive tags for products.  Relationships are established between the tables, and api routes are set up to provide useful information about the tables and their contents.

## Tools Used
* JavaScript ES6
* Node.js
* Express.js
* MySQL
* Sequelize

## Installation
If you would like to view this project, clone the repository to your computer. 

Create a `.env` file in the root directory of the project with the information below, adding your user name and password for your MySQL installation.
> DB_NAME='ecommerce_db'
>
> DB_USER='*your_username_here*'
>
> DB_PW='*your_password_here*'

Type `npm install` in the command line in the directory where you cloned the project to install the required packages.

Start MySQL by typing `mysql -u __*your_user_name*__ -p` and then entering your password on the next line.  Initialize the database by typing `source db/schema.sql`.  Quit MySQL by typing `quit`.

 Type `npm run seed` from the command line to seed the database.

## Usage
Start the server by typing `npm start` in the command line of the root directory of the project.

Test out the API routes in your application of choice, e.g. Insomnia Core or Postman.

  GET all categories (with associated products): http://localhost:3001/api/categories

  GET a single category by id (with associated products): http://localhost:3001/api/categories/1

  POST a new category: http://localhost:3001/api/categories

  PUT to update a category name specified by id: http://localhost:3001/api/categories/1

  DELETE a category by id: http://localhost:3001/api/categories/1

  GET all products (with associated category and a tag count): http://localhost:3001/api/products

  GET a single product by id (with the associated category and all tag information): http://localhost:3001/api/products/1

  POST a new product: http://localhost:3001/api/products
  
  PUT to update a product by id: http://localhost:3001/api/products/1

  DELETE a product by id: http://localhost:3001/api/products/1

  GET all tags (with a count of associated products): http://localhost:3001/api/tags/ 

  GET a single tag by id (with all associated product and category information): http://localhost:3001/api/tags/1

  POST a new tag: http://localhost:3001/api/tags/ 

  PUT to update a tag: http://localhost:3001/api/tags/1

  DELETE a tag by id: http://localhost:3001/api/tags/1

  ## Video Walkthrough
  A video walkthrough of the application in action can be found [here](#).