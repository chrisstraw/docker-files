# Backup PostgreSQL to sql file

The file will be generated where the command is ran from

```
docker run -it -e PGPASSWORD=<password> postgres:alpine  pg_dump -h <host_name> -U <username> <database_name> > backup.sql
```

### Fake Example
```
docker run -it -e PGPASSWORD=FakePassword postgres:alpine  pg_dump -h myhost.fake.com -U MyFakeUserName MyDatabase > backup.sql
```
