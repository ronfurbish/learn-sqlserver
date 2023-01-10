# Learn SQL Server
A basic Docker Compose to spin up a SQL Server instance along with a web-based database tool in case you don't already have one locally.

## Docker Instructions
Notes: You'll need to run one of the commands below before you use the instuctions to connect.

Run on Intel or AMD based chipset (i.e. Intel based PC or Mac)

``` docker compose up -d sqlserver ```

Run on ARM based machines (i.e. M1 Mac)
Note: Azure SQL Edge is more geared for IoT, but still built on the same SQL Server engine

``` docker compose up -d sqledge ```

## How to connect with Azure Data Studio
Note: [Azure Data Studio](https://learn.microsoft.com/en-us/sql/azure-data-studio/download-azure-data-studio?view=sql-server-ver16) is a cross-platform database tool for data professionals who use on-premises and cloud data platforms on Windows, macOS, and Linux.  I personally like using this on my Mac.  It may not have all the features of Management Studio, yet, but it has a much more modern design and feel.

1. Open Azure Data Studio on your computer
2. Create a new server connection
    - Connection type: ``` Microsoft SQL Server ```
    - Server: ``` localhost,11433 ```
    - Authentication type: ``` SQL Login ```
    - User name: ``` sa ```
    - Password: ``` yourStrong(!)Password ```
3. Click Connect

## How to connect with SQL Management Studio
Note: [SQL Management Studio](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16) is the classic tool used to connect to SQL Server and faithful used by most Microsoft shops I've seen to date.

1. Open SQL Management Studio on your computer
2. Create a new server connection
    - Server type: ``` Database Engine ```
    - Server name: ``` localhost,11433 ```
    - Authentication: ``` SQL Server Authentication ```
    - Login: ``` sa ```
    - Password: ``` yourStrong(!)Password ```
3. Click Connect

##

### Work In Progress Notes:

[Cloudbeaver](https://github.com/dbeaver/cloudbeaver) is included in the docker compose, but will require setup.  Having trouble getting hostname to work with anything other an IP address. 
