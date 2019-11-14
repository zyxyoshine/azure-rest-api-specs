## CLI

These settings apply only when `--cli` is specified on the command line.

``` yaml $(cli)
cli:
  namespace: azure.mgmt.healthcareapis
  flatten-all: true
  option-override:
    "cosmos_db_configuration_offer_throughput":
      name: "cosmos_db_offer_throughput"
    "authentication_configuration_authority":
      name: "authentication_authority"
    "authentication_configuration_audience":
      name: "authentication_audience"
    "authentication_configuration_smart_proxy_enabled":
      name: "authentication_smart_proxy_enabled"
    "cors_configuration_origins":
      name: "cors_origins"
    "cors_configuration_headers":
      name: "cors_headers"
    "cors_configuration_methods":
      name: "cors_methods"
    "cors_configuration_max_age":
      name: "cors_max_age"
    "cors_configuration_allow_credentials":
      name: "cors_allow_credentials"
  test-setup:
    - name: Check name availability
    - name: Lists all of the available Healthcare service REST API operations.
    - name: Create or Update a service with all parameters
    - name: Delete service
    - name: Create or Update a service with minimum parameters
    - name: Get the metadata of a service instance.
    - name: List all services in subscription
    - name: List all services in resource group
    - name: Delete service
```
