## AZ

These settings apply only when `--az` is specified on the command line.

``` yaml $(az)
az:
  extensions: managedservices
  namespace: azure.mgmt.managedservices
  package-name: azure-mgmt-managedservices
az-output-folder: $(azure-cli-extension-folder)/src/managedservices
python-sdk-output-folder: "$(az-output-folder)/azext_managedservices/vendored_sdks/managedservices"
```
