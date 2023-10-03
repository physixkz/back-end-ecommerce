# back-end-ecommerce

## Table of Contents
. Description
. Technologies Used
. Installation
. Configuration
. Usage
. API Routes
. Testing
. Contributing
. License

## Description
This is the back end for an e-commerce website that utilizes the latest technologies to help your company compete effectively in the online retail space. It provides a robust Express.js API integrated with a MySQL database using Sequelize for data modeling and interaction.

## Technologies Used
. Express.js
. MySQL
. Sequelize

## Installation

Here is a quick video on how to get this application started:

    https://drive.google.com/file/d/1R9boIapfuEpNwZn7dtLGbPt6EX1U1pTt/view

To set up the project locally, first make sure you clone the repository to your machine by running the following command in terminal in the directory you want the project in:

git clone git@github.com:physixkz/back-end-ecommerce.git

Once you have the project cloned, make sure you navigate to the project by running the following command in terminal:

cd back-end-ecommerce

Once there, be sure to install the dependencies by running this code:

    npm install

## Configuration

Before running the application, you need to configure your database connection. Be sure to rename the file ".env.EXAMPLE" to ".env". Once you have renamed the file, go ahead and edit the file to include your mysql username and mysql password within the '' in their corresponding lines. The database name has been provided for you already if you are using the same database used within the project. Once you have this configured, make sure to log into your mysql database and run 

    source db/schema.sql

This will create your database if you have not done so already.


## Usage

After configuring the database, you can start the application by right clicking on the server.js file and opening your terminal, in your terminal enter the following commands:

    npm run seed 
    
    npm start

This will start the server and sync Sequelize models with the MySQL database.


## API Routes

The API provides the following routes:

GET /api/categories: Get a list of all categories in JSON format.
GET /api/products: Get a list of all products in JSON format.
GET /api/tags: Get a list of all tags in JSON format.
POST /api/categories: Create a new category.
POST /api/products: Create a new product.
POST /api/tags: Create a new tag.
PUT /api/categories/:id: Update an existing category by ID.
PUT /api/products/:id: Update an existing product by ID.
PUT /api/tags/:id: Update an existing tag by ID.
DELETE /api/categories/:id: Delete a category by ID.
DELETE /api/products/:id: Delete a product by ID.
DELETE /api/tags/:id: Delete a tag by ID.

## Testing
You can use the program Insomnia or any API testing tool to test the API endpoints. Make sure to test GET, POST, PUT, and DELETE routes for categories, products, and tags as specified in the acceptance criteria.

## Contributing
N/A

## License
This project is licensed under the MIT License.