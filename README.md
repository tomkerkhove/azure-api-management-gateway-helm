# Azure API Management Gateway - Helm chart

[![Build Status](https://dev.azure.com/tomkerkhove/Azure%20API%20Management%20Gateway/_apis/build/status/CI%20-%20Helm?branchName=master)](https://dev.azure.com/tomkerkhove/Azure%20API%20Management%20Gateway/_build/latest?definitionId=85&branchName=master)

A Helm chart to deploy an Azure API Management Gateway on Kubernetes.

## Installing the Chart

```console
helm repo add tomkerkhove https://tomkerkhove.azurecr.io/helm/v1/repo
helm install --name azure-api-management-gateway tomkerkhove/azure-api-management-gateway \
               --set gateway.endpoint='<gateway-url>' \
               --set gateway.authKey='<gateway-key>'
```