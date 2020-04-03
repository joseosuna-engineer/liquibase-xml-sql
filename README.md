# README #

Liquibase is an open-source database-independent library for tracking, managing and applying database schema changes. 
All changes to the database are stored in text files (XML, YAML, JSON or SQL) and identified by a combination of an "id" and "author" tag as well as the name of the file itself. A list of all applied changes is stored in each database which is consulted on all database updates to determine what new changes need to be applied. As a result, there is no database version number but this approach allows it to work in environments with multiple developers and code branches.

Liquibase automatically creates DatabaseChangeLog Table and DatabaseChangeLogLock Table when you first execute a changeLog File.


# Reference: 
http://www.liquibase.org/documentation/xml_format.html


# ROLLBACK:
liquibase:rollback -Dliquibase.rollbackTag=0.01
