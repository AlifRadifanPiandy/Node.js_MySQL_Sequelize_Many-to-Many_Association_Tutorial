**Node.js MySQL Sequelize Many-to-Many Association Tutorial**

============================================================

Table of Contents

-----------------

* [Overview](#overview)

* [Configuration](#configuration)

* [Database Models](#database-models)

* [Associations](#associations)

* [License](#license)

Overview

--------

This project demonstrates a Node.js application using MySQL as a database and Sequelize as an ORM (Object-Relational Mapping) tool. The focus of this tutorial is on establishing many-to-many associations between tables.

Configuration

------------

The database configuration is stored in `db.config.js`, which uses environment variables to store sensitive information. The `dotenv` package is used to load these environment variables from a `.env` file.

* `HOST`: the database host

* `USER`: the database username

* `PASSWORD`: the database password

* `DB`: the database name

* `dialect`: the database dialect (in this case, MySQL)

* `pool`: the database connection pool settings

Database Models

----------------

The project defines two database models: `Tag` and `Tutorial`.

* `Tag`: defined in `tag.model.js`, with a single attribute `name` of type `STRING`.

* `Tutorial`: defined in `tutorial.model.js`, with two attributes `title` and `description` of type `STRING`.

Associations

------------

The `Tag` and `Tutorial` models are associated through a many-to-many relationship, established using the `belongsToMany` method in `index.js`. This relationship is defined through a junction table `tutorial_tag`.

License

-------

This project is licensed under the MIT License. See `LICENSE` for details.

**Note:** This README is a brief summary of the project structure and components. For a more in-depth understanding of the code, please refer to the individual files.