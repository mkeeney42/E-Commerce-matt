# E-Commerce Back End
Description
This project is a robust back end for an e-commerce website, built using Express.js API and configured to use Sequelize ORM with a PostgreSQL database. It provides a solid foundation for managing categories, products, and tags in an e-commerce platform.
Table of Contents

## Table Of Contents
Usage
API Routes
Database Models
Technologies Used
Contributing
License

## Installation

Clone the repository:
Copygit clone https://github.com/your-username/e-commerce-back-end.git

Navigate to the project directory:
Copy - cd e-commerce-back-end

Install dependencies:
Copy - npm install

Create a .env file in the root directory and add your PostgreSQL credentials:
CopyDB_NAME='your_database_name'
DB_USER='your_postgres_username'
DB_PASSWORD='your_postgres_password'

Create the database using the schema file:
Copypsql -U your_postgres_username -d your_database_name -f db/schema.sql

Seed the database:
Copy - npm run seed


## Usage

Start the server:
Copy - npm start

Use an API client like Insomnia to test the routes (see API Routes section).

## API Routes
### Categories

GET /api/categories - Get all categories
GET /api/categories/:id - Get a single category by ID
POST /api/categories - Create a new category
PUT /api/categories/:id - Update a category
DELETE /api/categories/:id - Delete a category

### Products

GET /api/products - Get all products
GET /api/products/:id - Get a single product by ID
POST /api/products - Create a new product
PUT /api/products/:id - Update a product
DELETE /api/products/:id - Delete a product

### Tags

GET /api/tags - Get all tags
GET /api/tags/:id - Get a single tag by ID
POST /api/tags - Create a new tag
PUT /api/tags/:id - Update a tag
DELETE /api/tags/:id - Delete a tag

### Database Models

Category: id, category_name
Product: id, product_name, price, stock, category_id
Tag: id, tag_name
ProductTag: id, product_id, tag_id

## Technologies Used

Node.js
Express.js
Sequelize ORM
PostgreSQL
dotenv

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
This project is licensed under the MIT License.
