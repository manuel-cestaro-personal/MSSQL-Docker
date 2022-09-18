# Microsoft SQL Server with Docker
Example of Microsoft SQL Server (MSSQL) with Docker container.

## Objective
The goal is to create a SQL Server container that saves data persistently and easily copied to a backup. I also followed the best practices from the docker documentation. I chose to use an Express license because my programs don't need more performance at the moment.

## Start the containers
- clone the repo https://github.com/manuel-cestaro-personal/MSSQL-Docker/archive/refs/heads/main.zip
- `cd MSSQL-Docker`
- `mkdir .secrets && cd .secrets`
- `nano mssql_sa_pwd.txt` --> write the pwd of the SuperAdministrator (SA) user of mssql db
- `cd ..`
- `docker network create <Your_Network_Name>` --> create your docker network
- `nano docker-compose.yml` --> edit the file with `<Your_Network_Name>`
- if you want edit the `docker-compose.yml` with differents paths for the `.secret` directory or the `mount bind` volumes
- `docker-compose up -d`
- use `docker ps -a` to check the containers

## Conclusions
Nothing&#128517;, this is my way of working!&#128513;<br>
It sounds simple but it took me many hours of work.<br>
Hope it can help you!&#128521;&#128406;