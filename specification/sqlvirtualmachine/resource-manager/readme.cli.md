## CLI

These settings apply only when `--cli` is specified on the command line.

``` yaml $(cli)
cli:
  cli-name: sqlvirtualmachine
  package-name: azure-mgmt-sqlvirtualmachine
  namespace: azure.mgmt.sqlvirtualmachine
  test-scenario:
    - name: /SqlVirtualMachineGroups/put/Creates or updates a SQL virtual machine group.
    - name: /SqlVirtualMachines/put/Creates or updates a SQL virtual machine for Storage Configuration Settings to EXTEND Data, Log or TempDB storage pool.     
    - name: /SqlVirtualMachines/put/Creates or updates a SQL virtual machine for Storage Configuration Settings to NEW Data, Log and TempDB storage pool.
    - name: /SqlVirtualMachines/put/Creates or updates a SQL virtual machine with max parameters.
    - name: /SqlVirtualMachines/put/Creates or updates a SQL virtual machine with min parameters.
    - name: /SqlVirtualMachines/put/Creates or updates a SQL virtual machine and joins it to a SQL virtual machine group.
      disabled: true
    - name: /AvailabilityGroupListeners/put/Creates or updates an availability group listener.
      disabled: true
    - name: /AvailabilityGroupListeners/get/Gets an availability group listener.
      disabled: true
    - name: /AvailabilityGroupListeners/get/Lists all availability group listeners in a SQL virtual machine group.
      disabled: true
    - name: /SqlVirtualMachines/get/Gets the list of sql virtual machines in a SQL virtual machine group.
      disabled: true
    - name: /SqlVirtualMachineGroups/get/Gets a SQL virtual machine group.
    - name: /SqlVirtualMachines/get/Gets a SQL virtual machine.
    - name: /SqlVirtualMachineGroups/get/Gets all SQL virtual machine groups in a resource group.
    - name: /SqlVirtualMachines/get/Gets all SQL virtual machines in a resource group.
    - name: /SqlVirtualMachineGroups/get/Gets all SQL virtual machine groups in a subscription.
    - name: /SqlVirtualMachines/get/Gets all SQL virtual machines in a subscription.
    - name: /Operations/get/Lists all of the available SQL Rest API operations.
    - name: /SqlVirtualMachineGroups/patch/Updates a SQL virtual machine group tags.
      disabled: true
    - name: /SqlVirtualMachines/patch/Updates a SQL virtual machine tags.
      disabled: true
    - name: /AvailabilityGroupListeners/delete/Deletes an availability group listener.
      disabled: true
    - name: /SqlVirtualMachineGroups/delete/Deletes a SQL virtual machine group.
    - name: /SqlVirtualMachines/delete/Deletes a SQL virtual machine.
```
