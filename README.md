# Simple .NET 5.0 API for User Management  
Projects basically supports user registration, login with JWT authentication and user CRUD operations.

## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)
* [Contact](#contact)
----------
## General info
This API is configured to use a local SQLite database in development and a SQL Server database in production. It uses Entity Framework Core migrations to automatically generate the database on startup, for more info on EF Core migrations see [Micrososft Docs - EF Migrations](https://docs.microsoft.com/en-us/ef/core/managing-schemas/migrations).

Migrations Commands are in `~\Migrations\Commands.md`

The architecture of project combined of 
* Authorization
* Helpers
* Controllers
* Services

----------	
## Technologies
Project is created with:
* .Net version: **@5.0**
* AutoMapper version: **@10.1.1**
* BCrypt.Net-Next version: **@4.0.2**
* Microsoft.EntityFrameworkCore version: **@5.0.6**
* Microsoft.EntityFrameworkCore.Sqlite version: **@5.0.6**
* Microsoft.AspNetCore.Authentication.JwtBearer version: **@5.0.6**
* System.IdentityModel.Tokens.Jwt version: **@6.11.0**

----------
## Setup
To run this project:

```
$ cd ../net-5-simple-api-auth-reg-man
$ dotnet restore
$ dotnet run
```

Or build and run in Docker
```
$ docker build --pull --rm -f "Dockerfile" -t webapi-net-5-simple-api:latest "." 
$ docker run --rm -d  -p 4000:4000/tcp webapi-net-5-simple-api:latest
```
----------
## Contact
* Github : [slymnGms](https://github.com/slymnGms)
* LinkedIn: [Suleyman GUMUS](www.linkedin.com/in/sulaiman-gms)
* E-mail: [suleyman.gumus@outlook.com.tr](mailto:suleyman_gumus@outlook.com.tr)
