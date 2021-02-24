# grakn-database-tenancy

## Getting started

### download

```
git clone https://github.com/JonThom/grakn-database-tenancy.git
```

### run

first make sure [Grakn 2.0](https://dev.docs.grakn.ai/docs/console/console) is installed. Then

```
cd grakn-database-tenancy
grakn server
console
database create tenancy
transaction tenancy write schema 
source ./tenancy_schema.gql 
commit
transaction tenancy write data
source ./tenancy_data.gql
commit
exit

```
