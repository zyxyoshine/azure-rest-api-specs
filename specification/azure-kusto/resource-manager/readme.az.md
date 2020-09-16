## AZ

These settings apply only when `--az` is specified on the command line.

``` yaml $(az)
cli:
    cli-directive:
      - where:
            group: 'DataConnections'
            op: 'CreateOrUpdate|Update'
            param: 'parameters'
        poly-resource: true
      - where:
            group: 'DataConnections'
            op: 'dataConnectionValidation'
            param: 'properties'
        poly-resource: true
      - where:
            param: virtualNetworkConfiguration
        alias:
            - vnet_config
      - where:
            param: principalAssignmentName
        alias:
            - pa_name
      - where:
            param: userAssignedIdentities
        alias:
            - uai
      - where:
            param: storageAccountResourceId
        alias:
            - sa_rid
      - where:
            param: eventHubResourceId
        alias:
            - eh_rid
      - where:
            param: defaultPrincipalsModificationKind
        alias:
            - pm_kind
      - where:
            param: sharedAccessPolicyName
        alias:
            - sap_name
      - where:
            param: eventSystemProperties
        alias:
            - es_props
      - where:
            param: blobStorageEventType
        alias:
            - bse_type
      - where:
            param: enableDiskEncryption
        alias:
            - enable_disk_e
      - where:
            param: enableDoubleEncryption
        alias:
            - enable_double_e
      - where:
            param: enableStreamingIngest
        alias:
            - enable_si
      - where:
            type: ReadOnlyFollowingDatabase
        alias:
            - rof_database
      - where:
            param: trustedExternalTenants
        alias:
            - trusted_ext
      - where:
            param: attachedDatabaseConfigurationName
        alias:
            - attached_dc_name
      - where:
            group: Clusters
            op: CreateOrUpdate
            param: parameters
        json: true
      - where:
            group: Clusters
            op: CreateOrUpdate#Create
            param: parameters
        json: true
```
``` yaml $(az) && $(target-mode) != 'core'
az:
  extensions: kustoext
  namespace: azure.mgmt.kusto
  package-name: azure-mgmt-kusto
az-output-folder: $(azure-cli-extension-folder)/src/kustoext
python-sdk-output-folder: $(az-output-folder)/azext_kustoext/vendored_sdks/kusto
```

``` yaml $(target-mode) == 'core'
az:
  extensions: kustotest
  namespace: azure.mgmt.kusto
  package-name: azure-mgmt-kusto
az-output-folder: $(azure-cli-folder)/src/azure-cli/azure/cli/command_modules/kustotest
python-sdk-output-folder: $(az-output-folder)/vendored_sdks/kusto
```