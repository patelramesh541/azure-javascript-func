To run it locally

`func start`

Run function in Azure cloud

`az group create --name AzureFunctionsQuickstart-rg --location westeurope`


`az storage account create --name <STORAGE_NAME> --location westeurope --resource-group AzureFunctionsQuickstart-rg --sku Standard_LRS
`

`az functionapp create --resource-group AzureFunctionsQuickstart-rg --consumption-plan-location westeurope --runtime node --runtime-version 12 --functions-version 3 --name <APP_NAME> --storage-account <STORAGE_NAME>`

publish function on cloud

`func azure functionapp publish <APP_NAME>`

check logs

`func azure functionapp logstream <APP_NAME> `