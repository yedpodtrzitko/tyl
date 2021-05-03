# Migrate to new Postgres version

replace version numbers as needed

```shell
$ initdb /opt/homebrew/var/postgres --lc-collate="en_US.UTF-8"

$ pg_upgrade \
-b /opt/homebrew/Cellar/postgresql@12/12.6_1/bin \
-B /opt/homebrew/Cellar/postgresql/13.2_1/bin \
-d /opt/homebrew/var/postgresql@12 \
-D /opt/homebrew/var/postgres
```
