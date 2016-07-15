## Repository information

This repository contains the session databases for the [Iris web framework](https://github.com/kataras/iris) , contributions are welcome.

## How to Install?

```sh
$ go get github.com/iris-contrib/sessiondb/$FOLDER
```

## How to Register?


```go
db := $FOLDER.New(configurationHere{})
iris.UseSessionDB(db)
```

> Note: You can use more than one database to save the session values, but the initial data will come from the first non-empty `Load`, look inside [code](https://github.com/iris-contrib/sessiondb/blob/master/redis/database.go) for more information on how to create your own session database.
