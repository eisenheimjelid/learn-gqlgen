# learn-gqlgen
My history about the process to learn GraphQL+Go

## Step 1. Setup gqlgen

Do next, with the current code, and it will run like the example from https://gqlgen.com/getting-started/.

```bash
$ mkdir learn-gqlgen
$ cd learn-gqlgen/
$ go mod init github.com/eisenheimjelid/learn-gqlgen
$ go get github.com/99designs/gqlgen
$ go run github.com/99designs/gqlgen init
Exec "go run ./server.go" to start GraphQL server
$ go run server.go 
2021/03/02 16:29:48 connect to http://localhost:8080/ for GraphQL playground
```

## Step 2. Add code slightly more realistic

Add new `graph/model/todo.go`, regenerate the code and implement the new resolver into `graph/schema.resolvers.go`.

```bash
$ go generate
$ go run server.go 
2021/03/02 20:35:39 connect to http://localhost:8080/ for GraphQL playground
```
