# Analytics Engineering Pipeline with Mage, dbt, and Duckdb

## Overview

This project aims to leverage Mage, dbt, and duckdb to ingest data from various sources and demonstrate an end-to-end ETL pipeline, all developed within three hours. The result is a dbt model build in the `my_duck_db.duckdb` database outputted by Mage.

## Getting Started

It is recommend to follow [Mage.ai's intstructions](https://docs.mage.ai/getting-started/setup#docker-run) and run this via the Mage gui. The recommended docker route is preferrable.

Docker Compose Template
```
git clone https://github.com/mage-ai/compose-quickstart.git mage-quickstart \
&& cd mage-quickstart \
&& cp dev.env .env && rm dev.env \
&& docker compose up
```

Docker Run
```
docker run -it -p 6789:6789 -v $(pwd):/home/src mageai/mageai /app/run_app.sh mage start [project_name]
```
The `your_first_project` directory contains the code associated to this project.

To directly view the output of this, you can query the `my_duck_db.duckdb` database directly (located in the `dbt/brightwheel` directory). [DBeaver](https://dbeaver.io/) is a free IDE that connects with duckdb.

## Additional Resources

- [Mage Documentation](https://docs.mage.ai/)
- [dbt Documentation](https://docs.getdbt.com/)
- [DuckDB Documentation](https://duckdb.org/docs/)
