sample-dotnetcore-microservices
==
A tiny sample microservices written in .NET Core.

## Requirement
* https://www.microsoft.com/net/core
* https://www.docker.com/

## Build & Publish
```
dotnet restore src/web
dotnet restore src/service1
dotnet restore src/service2

dotnet publish src/web
dotnet publish src/service1
dotnet publish src/service2
```
## Usage
* Run services
```
docker-compose up -d
```
* Get http://{docker-host}:5000/
  * -> Hello from WEB!
* Get http://{docker-host}:5000/service1
  * -> Hello from [SERVICE1]!
* Get http://{docker-host}:5000/service2
  * -> Hello from [SERVICE2]!
