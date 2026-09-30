# E-commerce Back End

The back end for an e-commerce site: a RESTful API built with Express.js and Sequelize on a MySQL database, managing products, categories and tags.

**Demo video:** https://watch.screencastify.com/v/NQB4sTGF0Qc5eZsJrRIO

## Features

- Full CRUD for **categories**, **products** and **tags**
- Sequelize models with associations:
  - A category has many products
  - Products and tags are linked many-to-many through `ProductTag`
- Seed script with sample data

## Built With

Node.js · Express.js · Sequelize · MySQL · dotenv

## API Routes

| Resource | Routes |
|---|---|
| Categories | `GET /api/categories`, `GET /api/categories/:id`, `POST /api/categories`, `PUT /api/categories/:id`, `DELETE /api/categories/:id` |
| Products | `GET /api/products`, `GET /api/products/:id`, `POST /api/products`, `PUT /api/products/:id`, `DELETE /api/products/:id` |
| Tags | `GET /api/tags`, `GET /api/tags/:id`, `POST /api/tags`, `PUT /api/tags/:id`, `DELETE /api/tags/:id` |

## Getting Started

**Prerequisites:** Node.js and MySQL

```bash
git clone https://github.com/Archo2/E-commerceBackEnd.git
cd E-commerceBackEnd
npm install
```

1. Create a `.env` file in the project root:
   ```
   DB_NAME=ecommerce_db
   DB_USER=your_mysql_user
   DB_PW=your_mysql_password
   ```
2. Create the database, seed it and start the server:
   ```bash
   mysql -u root -p < db/schema.sql
   npm run seed
   npm start
   ```
3. Test the routes with Insomnia or Postman at http://localhost:3001.

## Screenshots

<img width="800" alt="Screenshot" src="https://user-images.githubusercontent.com/87740574/157807200-a8e0191d-57c4-41ac-bb6f-0ac4bd4daefd.png">

<img width="800" alt="Screenshot" src="https://user-images.githubusercontent.com/87740574/157807387-3bf88ca6-0cdd-485d-a1e6-ae0b531a2c61.png">

## Author

**Archils Oburu**
- GitHub: [@Archo2](https://github.com/Archo2)
- Email: oburuarchils@gmail.com
