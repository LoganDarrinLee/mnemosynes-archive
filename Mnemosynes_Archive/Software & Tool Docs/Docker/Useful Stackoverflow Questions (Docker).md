
[Postgres image is not creating database](https://stackoverflow.com/questions/48629799/postgres-image-is-not-creating-database)
Most likely came from starting the container without environment variables set, an easy fix:
- Find volume `docker volume ls`
- Remove volume `docker volume rm <volume name>`

