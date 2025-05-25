# Play.Infra

This folder contains infrastructure and deployment resources for the GameShop solution.

## Add the Github package source
```sh
$owner="microservices-dotnetcore"
$gh_pat="[]"

dotnet nuget add source --username USERNAME --password $gh_pat --store-password-in-clear-text --name github "https://nuget.pkg.github.com/$owner/index.json"
```

## Creating the azure resource group
```powershell
$appname="game shop"
az group create --name $appname --location eastus
```


## Contents
- `docker-compose.yml`: Multi-service orchestration for local development.

## Usage
Use the provided Docker Compose file to spin up all services and dependencies for local development or testing.

---
