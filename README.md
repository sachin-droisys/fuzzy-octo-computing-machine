# Device Management Service - Setup & Deployment Steps

## Introduction

This helps to setup the development environment and deploy the Device Management Microservice into Kubernetes with Helm.

## Prerequisites
(Recommended Version)
- Visual Studio 2019/ VS Code 2019
- Mongodb 3.4.24
- Postman Client 8.0.3
- MiniKube 1.17+
- Docker 19.03+
- kubectl version 1.20+
- Helm Version: v3.5.1


## Installation & Code Setup

-Code checkout and build 

```
git clone https://github.com/realwear/Foresight-MS-DeviceManagement-RSystems.git -b Features/VL_NewProjectInitialCheckin
dotnet build
```

-Change the appsettings.config from application root location for Authority, Service Bus & MongoDb configuration.

```json
  "Storage": {
    "MongoDBConnectionString": "",
    "MongoDBDatabaseName": "",
    "ServiceBusConnectionString": ""
  },
  "Accounts": {
    "Authority": ""
  },

-Run the application
```
dotnet run

```
