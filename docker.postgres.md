#### CMD to run docker

To persist data
```
docker run --name my-postgres-server -p 5432:5432 -e POSTGRES_PASSWORD=example -v pgdata:/var/lib/postgresql/data -d postgres
```
```
docker run --name my-postgres-server -p 5432:5432 -e POSTGRES_PASSWORD=example -d postgres
```
```
Access details
Host: localhost
Port: 5432
username: postgres
password: example
```
For windows we can use: DBeaver CE

- to go inside container
```
docker exec -it my-postgres-server bash
```
