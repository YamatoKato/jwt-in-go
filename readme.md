# jwt-in-go

## DB migration

```
$ brew install golang-migrate
$ migrate create -ext sql -dir db/migrations -seq create_users_table
$ migrate --path db/migrations --database 'postgresql://user:password@localhost:5432/mydb?sslmode=disable' -verbose up
```
