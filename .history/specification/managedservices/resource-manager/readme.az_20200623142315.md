## AZ

These settings apply only when `--az` is specified on the command line.

``` yaml $(az)
az:
  extensions: managedservices
  namespace: azure.mgmt.managedservices
  package-name: azure-mgmt-kusto
az-output-folder: $(azure-cli-extension-folder)/src/kusto
python-sdk-output-folder: "$(az-output-folder)/azext_kusto/vendored_sdks/kusto"

```
