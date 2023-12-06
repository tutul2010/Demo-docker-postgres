# AdventureWorks for Postgres

This project provides the scripts necessary to set up the OLTP part of the go-to database used in
training classes and for sample apps on the Microsoft stack. The result is 68 tables containing HR,
sales, product, and purchasing data organized across 5 schemas. It represents a fictitious bicycle
parts wholesaler with a hierarchy of nearly 300 employees, 500 products, 20000 customers, and 31000
sales each having an average of 4 line items. So it's big enough to be interesting, but not
unwieldy. In addition to being a well-rounded OLTP sample, it is also a good choice to demonstrate
ETL into a data warehouse.


# Main  AdventureWorks OLTP database:

Download [Adventure Works 2014 OLTP Script](https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorks-oltp-install-script.zip).

```

## Using with Docker at windows 10

You can spin up a new Postgres-database using  **Docker** at windows 10 enviroment  with `docker-compose up --build`. 
and it download necessary files, build the image, and run the container. The database will be available on port 5432. Use the following environment variables to configure the database:

```sh
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
POSTGRES_DB=Adventureworks
POSTGRES_PORT=5432
POSTGRES_HOST=localhost

POSTGRES_URL="postgresql://postgres:postgres@127.0.0.1/Adventureworks"

## Successful Running of Docker images , can connect by using DBeaver client tool 
WebLink - https://github.com/tutul2010/DemoWebApp/assets/13733464/e045a489-d7d4-459b-b56f-5dab65b1ae91 

_You will need to rename the Adventure Works 2014 OLTP Script archive to **adventure_works_2014_OLTP_script.zip** to get this to work!_


## Motivation

Thanks @lorint/AdventureWorks-for-Postgres

Let's keep coding fun.

Enjoy!
