# goexpert-13-graphql

This project is a simple implementation of a GraphQL playground using Go.
It is part of the Go Expert Course of [FullCycle Development](https://goexpert.fullcycle.com.br/pos-goexpert/).

## Commands to run

On the root of the project use the tidy command to organize the dependencies:

```sh
go mod tidy
```

Start the sqlite3 tables using the following commands:

```sh
sqlite3 data.db
create table categories (id string, name string, description string);
create table courses (id string, name string, description string, category_id string);
```

Then run the main function using the command below:
```sh
go run cmd/server/server.go
```

Access the GraphQL playground on your browser throught the [localhost](http://localhost:8080/#) addess