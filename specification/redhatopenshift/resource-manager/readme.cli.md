## CLI

These settings apply only when `--cli` is specified on the command line.

``` yaml
cli:
  test-scenario:
    - name: /OpenShiftClusters/put/Creates or updates a OpenShift cluster with the specified subscription, resource group and resource name.
    - name: /OpenShiftClusters/get/Gets a OpenShift cluster with the specified subscription, resource group and resource name.
    - name: /OpenShiftClusters/get/Lists OpenShift clusters in the specified subscription and resource group.
    - name: /OpenShiftClusters/get/Lists OpenShift clusters in the specified subscription.
    - name: /Operations/get/Lists all of the available RP operations.
    - name: /OpenShiftClusters/post/Lists credentials of an OpenShift cluster with the specified subscription, resource group and resource name.
    - name: /OpenShiftClusters/patch/Creates or updates a OpenShift cluster with the specified subscription, resource group and resource name.
    - name: /OpenShiftClusters/delete/Deletes a OpenShift cluster with the specified subscription, resource group and resource name.
```

