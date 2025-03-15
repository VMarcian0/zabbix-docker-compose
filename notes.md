## Zabbix Frontend

http://localhost:80

## Setup banco de dados aplicação

```bash
docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=YourStrong@Passw0rd" -p 1433:1433 --name sqlserver --network zabbix-docker-compose_network-zabbix -d mcr.microsoft.com/mssql/server:2022-latest
```

## Rodando migrations

```bash
dotnet ef database update --project 04_Infraestructure --startup-project 04_Infraestructure
```

## Grafa Acesso

usr: admin
pwd: 6zvDS.fZcydm9q@
