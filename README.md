This is the example repository for [this blog post](https://www.sohamkamani.com/blog/2017/10/18/golang-adding-database-to-web-application/)

To run the server on your system:

1. Make sure you have [dep](https://github.com/golang/dep) installed
2. Run `dep ensure` to install dependencies
3. Run `go build` to create the binary (`blog_example__go_web_db`)
4. Run the binary : `./blog_example__go_web_db`

To run tests:

2. Run `dep ensure` to install dependencies
2. Run `go test ./...`


Create the `birds` table before running the application :

```sql
create table birds (
id serial primary key,
bird varchar(256),
description varchar(1024)
);
```

Before running the application, edit the `connString` variable inside the `main` function to specify your postgres database connection
