# AdventureWorks for Postgres

This project provides the scripts necessary to set up the OLTP part of the go-to database used in
training classes and for sample apps on the Microsoft stack. The result is 68 tables containing HR,
sales, product, and purchasing data organized across 5 schemas. It represents a fictitious bicycle
parts wholesaler with a hierarchy of nearly 300 employees, 500 products, 20000 customers, and 31000
sales each having an average of 4 line items. So it's big enough to be interesting, but not
unwieldy. In addition to being a well-rounded OLTP sample, it is also a good choice to demonstrate
ETL into a data warehouse.



## How to set up the database:

Download [Adventure Works 2014 OLTP Script](https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorks-oltp-install-script.zip).


```

## Using with Docker
You can spin up a new database using **Docker** with `docker-compose up --build`. 
There is a helper script at `./run_docker.sh` that will download necessary files, build the image, and run the container. The database will be available on port 5432. Use the following environment variables to configure the database:

```sh
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
POSTGRES_DB=Adventureworks
POSTGRES_PORT=5432
POSTGRES_HOST=localhost

POSTGRES_URL="postgresql://postgres:postgres@127.0.0.1/Adventureworks"


_You will need to rename the Adventure Works 2014 OLTP Script archive to **adventure_works_2014_OLTP_script.zip** to get this to work!_


## Motivation

Thanlks @lorint/AdventureWorks-for-Postgres

Let's keep coding fun.

Enjoy!
