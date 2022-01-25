## ORM Challenge: E-commerce Back End
GIVEN a functional Express.js API:

- WHEN I add my database name, MySQL username, and MySQL password to an environment variable file THEN I am able to connect to a database using Sequelize
- WHEN I enter schema and seed commands THEN a development database is created and is seeded with test data
- WHEN I enter the command to invoke the application THEN my server is started and the Sequelize models are synced to the MySQL database
- WHEN I open API GET routes in Insomnia for categories, products, or tags THEN the data for each of these routes is displayed in a formatted JSON
- WHEN I test API POST, PUT, and DELETE routes in Insomnia THEN I am able to successfully create, update, and delete data in my database

## Built With:
- Node.js
  - Express
  - Sequelize
  - MySQL2
  - dotENV

## App Function
This Express API app provides GET, POST, PUT, and DELETE routes to support the use of the ecommerce_db.  

# E-Commerce Database
The database contains four tables called category, product, product_tag, and tag.  Product is linked to category through the category ID and tags through the product_tag ID.  The models for Category, Product, ProductTag, and Tag establish the structure of their respective tables and the models index.js provides the relationships between the models.

# Seeds
A seed folder is provided to provide the initial data for the database.  The seed data can be populated using "npm run seed".

# Model API Routes
There are three high-level API routes for categories, products, and tags which allow the user to:
- View all categories, products, or tags
- View a single category, product, or tag
- Add a category, product, or tag
- Update a category, product, or tag
- Delete a category, product, or tag

## Demo Video
https://github.com/texrob20/e-commerce-back-end/blob/main/demo/ecommerce-demo.webm

or

https://watch.screencastify.com/