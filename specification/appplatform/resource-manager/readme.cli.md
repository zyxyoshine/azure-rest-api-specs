## CLI

These settings apply only when `--cli` is specified on the command line.

``` yaml $(cli)
cli:
  cli-name: appplatform
  namespace: azure.mgmt.appplatform
  test-scenario:
    - name: /Services/put/Services_CreateOrUpdate
    - name: /Apps/put/Apps_CreateOrUpdate
    - name: /Certificates/put/Certificates_CreateOrUpdate
      disabled: true
      comment: Not available/tested yet
    - name: /CustomDomains/put/CustomDomains_CreateOrUpdate
      disabled: true
      comment: Not available/tested yet
    - name: /Bindings/put/Bindings_CreateOrUpdate
      disabled: true
      comment: Not available/tested yet
    - name: /Deployments/put/Deployments_CreateOrUpdate
      disabled: true
      comment: Not available/tested yet
    - name: /Deployments/get/Deployments_Get
      disabled: true
      comment: Not available/tested yet
    - name: /Bindings/get/Bindings_Get
      disabled: true
      comment: Not available/tested yet
    - name: /CustomDomains/get/CustomDomains_Get
      disabled: true
      comment: Not available/tested yet
    - name: /Certificates/get/Certificates_Get
      disabled: true
      comment: Not available/tested yet
    - name: /Deployments/get/Deployments_List
    - name: /Bindings/get/Bindings_List
    - name: /CustomDomains/get/CustomDomains_List
      disabled: true
      comment: Not available/tested yet
    - name: /Apps/get/Apps_Get
    - name: /Certificates/get/Certificates_List
      disabled: true
      comment: Not available/tested yet
    - name: /Deployments/get/Deployments_ListClusterAllDeployments
    - name: /Apps/get/Apps_List
    - name: /Services/get/Services_Get
    - name: /Services/get/Services_List
    - name: /Services/get/Services_ListBySubscription
    - name: /Operations/get/Operations_List
    - name: /Deployments/post/Deployments_GetLogFileUrl
      disabled: true
      comment: Not available/tested yet
    - name: /Deployments/post/Deployments_Restart
      disabled: true
      comment: Not available/tested yet
    - name: /Deployments/post/Deployments_Start
      disabled: true
      comment: Not available/tested yet
    - name: /Deployments/post/Deployments_Stop
      disabled: true
      comment: Not available/tested yet
    - name: /Deployments/patch/Deployments_Update
      disabled: true
      comment: Not available/tested yet
    - name: /Bindings/patch/Bindings_Update
      disabled: true
      comment: Not available/tested yet
    - name: /CustomDomains/patch/CustomDomains_Patch
      disabled: true
      comment: Not available/tested yet
    - name: /CustomDomains/post/CustomDomains_Validate
      disabled: true
      comment: Not available/tested yet
    - name: /Apps/post/Apps_GetResourceUploadUrl
    - name: /Apps/patch/Apps_Update
      disabled: true
      comment: Not available/tested yet
    - name: /Services/post/Services_DisableTestEndpoint
    - name: /Services/post/Services_EnableTestEndpoint
    - name: /Services/post/Services_RegenerateTestKey
    - name: /Services/post/Services_ListTestKeys
    - name: /Services/patch/Services_Update
      disabled: true
      comment: Not available/tested yet
    - name: /Services/post/Services_CheckNameAvailability
    - name: /Bindings/delete/Bindings_Delete
      disabled: true
      comment: Not available/tested yet
    - name: /CustomDomains/delete/CustomDomains_Delete
      disabled: true
      comment: Not available/tested yet
    - name: /Certificates/delete/Certificates_Delete
      disabled: true
      comment: Not available/tested yet
    - name: /Apps/delete/Apps_Delete
    - name: /Services/delete/Services_Delete
```
