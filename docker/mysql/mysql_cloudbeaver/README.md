## CloudBeaver

    http://localhost:8978
finish setup with

    username: cbadmin
    password: Admin@123

click on icon to add new connection

    host: mysql
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
