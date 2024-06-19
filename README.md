# Liquibase

Proof of concept for Liquibase migrations.

## Prerequisites

- **PlantUML**: Used for visualizing the database schema. [PlantUML](https://plantuml.com)

1- Run docker compose for the database
```bash
Docker-compose -f docker-compose.database.yml up
```

2- Run docker compose for the Liquibase migration
```bash
Docker-compose -f docker-compose.liquibase.yml up
```
or into your machine

```bash
liquibase --defaultsFile=config/liquibase.properties update 
```

All scripts inside /scripts folder will be executed on target database
