# NoSQL and Document-Oriented Databases

## Module 3 Assignment
Reproduce the live lecture task of setting up and
inserting the RPG data (specifically the `charactercreator_character`,
`charactercreator_character_inventory`, `armory_item`, and `armory_weapon` tables) into a MongoDB instance. Your documents in MongoDB should contain the character traits
(name, level, etc.) and skills (strength, wisdom, etc.) and a list of their items.
You should also store the weapons as a list in another key value pair (you will have duplicate items in both items and weapons) - see the example below.

Mongo document example:
```
mongo_document = {
  "name": <VALUE>,
  "level": <VALUE>,
  "exp": <VALUE>,
  "hp": <VALUE>,
  "strength": <VALUE>,
  "intelligence": <VALUE>,
  "dexterity": <VALUE>,
  "wisdom": <VALUE>,
  "items": [
    <ITEM NAME>,
    <ITEM NAME>
  ],
  "weapons" [
    <ITEM NAME>,
    <ITEM NAME>
  ]
}
```

## Answer the following question in your `README.md` file:

* How was working with MongoDB different from working with PostgreSQL?

PostgreSQL and MongoDB are database management tools that allow us to run the databases on a cloud server somewhere in the world, instead of on our local machines.

PostgreSQL is a highly influential and reliable open-source object-relational database management system (RDBMS) that stores data within tables and utilizes the Structured Query Language (SQL) to access the database.

In PostgreSQL, the database schema has to be planned out before adding data. The schema is the architecture of the database that tells us the relationship between tables and the rules that govern the database. We need to have a clear understanding of the relationship between the tables to be able to execute queries by using joins and primary or foreign keys.

On the other hand, MongoDB is a very scalable document-oriented database management system or NoSQL database that is capable of handling big data and stores data in the form of a JSON document, very similar to a Python dictionary, allowing us to retrieve specific data from the database using Mongo Query Language (MQL).

Since the structure of the data is flexible, it doesn't need to be established upfront. In MongoDB, collections and documents are equivalent to rows and embedded documents work just like joins in traditional relational databases.


* What was easier, and what was harder?

PostgreSQL was easier for me to work with since I am more familiar with structured databases.


Please turn in the MongoDB python file you used to generate the documents as well as your `README.md`.


## Authors

- [@jianninapinto](https://www.github.com/jianninapinto)
