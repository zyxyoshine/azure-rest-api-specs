## AZ

These settings apply only when `--az` is specified on the command line.

``` yaml $(az)
az:
  extensions: datashare
  namespace: azure.mgmt.datashare
  package-name: azure-mgmt-datashare
python-sdk-output-folder: "$(output-folder)/src/datashare/azext_datashare/vendored_sdks/datashare"
  
#cli:
#    cli-directive:
#      directive on operationGroup
#       - select: 'operationGroup'
#         where:
#             operationGroup: 'operations'
#         hidden: true
#       - where:
#             parameter: location
#         required: true

cli:
  test-scenario:
    - name: /Accounts/put/Accounts_Create
    - name: /Accounts/get/Accounts_Get
    - name: /Accounts/get/Accounts_ListByResourceGroup
    - name: /Accounts/get/Accounts_ListBySubscription
    - name: /Accounts/patch/Accounts_Update
    - name: /Accounts/delete/Accounts_Delete

```
