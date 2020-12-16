# Database Design
* Database design is an art form of its own with particular skills and
experience.
* Our goal is to avoid the really bad mistakes and design clean and
easily understood databases.
* Others may performance tune things later.
* Database design starts with a picture...

## Building a Data Model
* Drawing a picture of the data objects for our application and then figuring
out how to represent the objects and their relationships.
* Basic Rule: Don't put the same string data in twice - use a relationship
instead.
* When there is one thing in the "real world" there should be one copy of that
thing in the database.

## Important things to remember
* Primary Key: uniquely identifies each record in a table. Primary keys must contain UNIQUE values and cannot contain NULL values. A table can have only ONE primary key. In the table, the primary key can conisist of single or multiple columns (end point)

* Logical Key: allows the application to assign a unique key value to each row in a table. Logical keys are useful when an application requires a table to have a unique key and the columns of the table do not comprise a unique key. 

* Foreign Key: is a column or combination of columns that is used to establish and enforce a link between the data in two tables to control the data that can be stored in the foreign key table. (starting point)

## Examples of SQLite code
* CREATE TABLE Genre(
		id INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT UNIQUE,
		name TEXT
		)
* insert into Artist (name) values ('Led Zepplin')

## Relational Power
* By removing the replicated data and replacing it with references to a single copy of each bit of data we build a "web" of information that the relational database can read through very quickly - even for very large amounts of data
* Often when you want some data it comes from a number of tables linked by these foreign keys

## The JOIN Operation
* The JOIN operation links across several tables as part of a select operation
* You must tell the JOIN how to use the keys that make the connection between tables using an ON clause

select Album.title, Artist.name from Album join Artist on Album.artist_id = Artist.id
