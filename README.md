For SQL Server instance in local. First, create an .env file with name sql-server.env and following variables and their corresponding values within sql-server folder.

1. ACCEPT_EULA=Y
2. SA_PASSWORD=your_password
3. MSSQL_PID=Developer

For mongo db host:

1. MONGO_INITDB_ROOT_USERNAME
2. MONGO_INITDB_ROOT_PASSWORD

For SQL Server instance in local. First, create an .env file with name sql-server.env and following variables and their corresponding values within sql-server folder.

1. ACCEPT_EULA=Y
2. SA_PASSWORD=your_password
3. MSSQL_PID=Developer

For mongo db host:

1. MONGO_INITDB_ROOT_USERNAME
2. MONGO_INITDB_ROOT_PASSWORD

For PostgreSQL:
Two environment files are required within the postgresql folder:

1. postgresql.env - Database configuration
   - POSTGRES_USER=your_username
   - POSTGRES_PASSWORD=your_password
   - POSTGRES_DB=your_database
   - PGDATA=/var/lib/postgresql/data/pgdata (optional)

2. pgadmin.env - PgAdmin configuration
   - PGADMIN_DEFAULT_EMAIL=your_email@example.com
   - PGADMIN_DEFAULT_PASSWORD=your_pgadmin_password

Template files (postgresql.template and pgadmin.env.template) are provided as examples. Copy these files to create your environment files:

```bash
cp postgresql.template postgresql.env
cp pgadmin.env.template pgadmin.env