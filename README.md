# Learn SQL Server
A basic Docker Compose to spin up a SQL Server instance along with a web-based database tool in case you don't already have one locally.

## Docker Instructions

Run on Intel or AMD based chipset (i.e. Intel based PC or Mac)

``` docker compose up -d sqlserver ```

Run on ARM based machines (i.e. M1 Mac)
Note: Azure SQL Edge is more geared for IoT, but still built on the same SQL Server engine

``` docker compose up -d sqledge ```

Work In Progress Notes:

Cloudbeaver is included in the docker compose, but will require setup.  Having trouble getting hostname to work with anything other an IP address.

If you connect with a local install of Azure Data Studio or SQL Management Studio you can use localhost for address.