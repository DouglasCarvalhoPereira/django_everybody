# SQLITE3

1. CREATE TABLE
2. INSERT INTO -> VALUES
3. DELETE FROM -> WHERE
4. UPDATE -> SET -> WHERE
5. SELECT * FROM -> WHERE

$ sqlite3 zip.sqlite3

$ .tables
$ CREATE TABLE Users(
    id INTEGER NOT NULL
        PRIMARY KEY AUTOINCREMENT,
    name VARCHAR(128),
    email VARCHAR(128)
);

$ .tables
>>> Users
$ .schema Users
CREATE TABLE Users(
    id INTEGER NOT NULL
        PRIMARY KEY AUTOINCREMENT,
    name VARCHAR(128),
    email VARCHAR(128)
);

INSERT INTO Users(name, email) VALUES("Kristin",'kf@umich.edu')

DELETE FROM Users WHERE email='ted@umich@.edu'

UPDATE Users Set name= 'Charles' WHERE email='csev@umch.edu'

SELECT * FROM Users WHERE email='csev@umich.edu'

SELECT * FROM Users ORDER BY email

SELECT * FROM Users ORDER BY name DESC