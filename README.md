**Node.js_MySQL_Sequelize_Many-to-Many_Association_Tutorial**

============================================================

This project demonstrates a basic Node.js application using Sequelize to interact with a MySQL database, with a many-to-many association between two models.

**Database Configuration**

---

The database configuration is stored in `db.config.js`, which uses environment variables to store sensitive information. The `dotenv` package is used to load these environment variables from a `.env` file.

- `HOST`: the database host

- `USER`: the database username

- `PASSWORD`: the database password

- `DB`: the database name

- `dialect`: the database dialect (in this case, MySQL)

- `pool`: the database connection pool settings

**Models**

---

The project defines two database models: `Tag` and `Tutorial`.

- `Tag`: defined in `tag.model.js`, with a single attribute `name` of type `STRING`.

- `Tutorial`: defined in `tutorial.model.js`, with two attributes `title` and `description` of type `STRING`.

**Contributing**

---

If you would like to contribute to this project, please feel free to submit a pull request or open an issue. Your feedback and contributions are greatly appreciated!

**License**

---

This project is licensed under the MIT License. You are free to use, modify, and distribute this code as you see fit. See the `LICENSE` file for more details.
