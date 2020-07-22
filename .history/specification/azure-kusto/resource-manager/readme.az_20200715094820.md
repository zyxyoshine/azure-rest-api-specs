## AZ

These settings apply only when `--az` is specified on the command line.

``` yaml $(az)
az:
  extensions: kusto
  namespace: azure.mgmt.kusto
  package-name: azure-mgmt-kusto

cli:
    cli-directive:
      - where:
            group: 'DataConnections'
            op: 'CreateOrUpdate|Update'
            param: 'properties'
        poly-resource: true
      - where:
            group: 'DataConnections'
            op: 'dataConnectionValidation'
            param: 'properties'
        poly-resource: true
```

``` yaml $(az) && !$(cli-core)
az-output-folder: $(azure-cli-extension-folder)/src/kusto
python-sdk-output-folder: "$(az-output-folder)/azext_kusto/vendored_sdks/kusto"
```
``` yaml $(az) && $(cli-core)
az-output-folder: $(azure-cli-folder)/src/azure-cli/azure/cli/command_modules/kusto_test
python-sdk-output-folder: "$(az-output-folder)/vendored_sdks/kusto"
```