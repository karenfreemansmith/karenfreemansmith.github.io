# PostgreSQL

## Installation
* Download and install Windows 64 version
* Add path to environment variables (c:\Program Files\PostgreSQL\9.6\bin)
* Add PGDATA to environment variables (c:\Program Files\PostgreSQL\9.6\data)
* (documentation on setting trusted username/password on local connections) https://www.postgresql.org/docs/9.6/static/auth-pg-hba-conf.html

## Start Server
* postgres

## Access Databases
* psql *(starts command line program)*
  * (on Windows) psql -U postgres -h localhost
* \l *(list databases)*
* \c databasename *(connects to specified database)*
* \dt *(displays tables in database)*
* \d tablename *(displays table schema)*

## Backup/Restore
* pg_dump datbase > db_backup.sql
* psql -U postgres database < db_backup.sql
