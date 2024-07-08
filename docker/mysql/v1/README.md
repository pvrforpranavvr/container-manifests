#### phpMYAdmin

    server: mysql
    username : user
    password: user

### MYSQLX (Document Store)

    mysqlsh
    mysqlsh -u <USER> -p

#### Switch to sql mode

    \sql
#### Create DB

    create database ds;
#### To connect

    \connect root@localhost:33060/ds

#### To execute js scripts

    \js
#### Create collection

    db.createCollection("users")

#### Create Index

    db.getCollection("users").createIndex("email", {fields: [{field: "$.email", type: "TEXT(10)"}]})
