# Changing collation of database

- useful when running `pg_upgrade` and getting this error message:

> lc_collate values for database “postgres” do not match

### command:

```sql
UPDATE pg_database SET datcollate='en_US.UTF-8', datctype='en_US.UTF-8' WHERE datname='postgres';
```