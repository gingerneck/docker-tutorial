# SQL LANGUAGE

1. [COMMON](#common)
2. [POSTGRESQL](#postgresql)


## COMMON

- **CREATE DATABASE {name}** - creates db with {name};
- **\c** or **\connect {database_name}** - connects to database
- **CREATE TABLE {table_name}( column1 datatype, .. columnN datatype, PRIMARY KEY( one or more columns ));**
- **\d** - shows all tables
- **\d {table_name}** - shows table with name {table_name}
- **insert into {table_name} ({column_name}) values('value for column');** - inserts values for columns
- **select {column_name} from {table_name};** - selects columns from table\
    **select distinct ....** - gets without duplicates\
    **... order by {column_name}** - sorts by column\
    **... where {column_name} = '' and {column_name} = '' or {column_name} = ''**\
    **... where {column_name} in ('', '','')**\
    **... between '' and ''**\
    **... where {column_name} like %** - % some symbols

## POSTGRESQL

- **psql** - open console 
- 