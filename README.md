# Ecommerce Back-End Development

## Description
An initial layout for a back-end server for a ecommerce website.
This project was created to show the interface of what goes behind the scenes through the app Insomnia.
You would be able to make GET, POST, PUT, and DELETE requests for the three models: Category, Product, and Tag.

## Installation Guide
1. Download Node.js on your local machine.
2. Clone this repo to your local machine.
3. Run in VSCode and open an integrated terminal.
4. Before use, run `npm install` to load any dependencies. (see package.json file for more detail)
5. Create a ‘.env’ file and paste these lines of code changing password to MySQL's root user password.

```
DB_USER=root
DB_PW=password
DB_NAME=ecommerce_db
```

6. Initial database login to the MySQL shell using `mysql -u root -p`.
7. Run the schema file with `source db/schema.sql`.
8. Run the seed database provided using `npm run seed`.

## Usage
[Click here for Walkthrough Video]()

After proper installation (see below), run using `npm start` in the command line within the terminal.
Use a program such as Insomnia to make GET, POST, PUT, and DELETE requests for the three models:
 * Category
 * Product
 * Tag
## User Story

```md
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies
```

## Thought Process

```md
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database
```