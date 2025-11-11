# Backup and Recovery in Postgresql Database

There are three ways to backup and restore postgresql database.

1. **SQL Dump**
The idea behind this method is to generate a file with SQL commands that, upon feeding back to the server, will recreate the database in the same state, as it was at the time of taking the dump. There is `pg_dump` utility provided for this purpose.

- One of the main advantages of using this method over others is that `pg_dump`'s output can generally be re-loaded into newer versions of Postgresql, whereas file-level backups and continuous archiving are both extremely server-version-specific.

>[!Important]
> Some OS have max file size limits that cause problems when creating large `pg_dump` output files. Handle this with `pg_dump dbname | gzip > filename.gz`, and reload with `gunzip -c filename.gz | psql dbname`