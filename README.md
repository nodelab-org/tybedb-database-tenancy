# grakn-database-tenancy

## Getting started

### download

```
git clone https://github.com/JonThom/grakn-database-tenancy.git
```

### run

first make sure [Grakn 2.0](https://dev.docs.grakn.ai/docs/console/console) is installed and the server is running. 

Open a grakn console and create a new database
```
cd grakn-database-tenancy
console
database create tenancy
```
define the schema
```
transaction tenancy write schema 
source ./tenancy_schema.gql 
commit
```
insert the data
```
transaction tenancy write data
source ./tenancy_data.gql
commit
exit
```
enjoy!
