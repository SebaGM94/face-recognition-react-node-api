Steps:

1.npm install  
2.npm start

Have a postres db and run the following :

CREATE TABLE users (
id serial PRIMARY KEY,
name VARCHAR(50),
email text UNIQUE NOT NULL,
entries BIGINT DEFAULT 0,
joined TIMESTAMP NOT NULL);

CREATE TABLE login (
hash VARCHAR(100),
email text UNIQUE NOT NULL
);
