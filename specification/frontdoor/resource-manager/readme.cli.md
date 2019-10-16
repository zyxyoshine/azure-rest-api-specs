## CLI

These settings apply only when `--cli` is specified on the command line.

``` yaml $(cli)
cli:
  cli-name: networkexperiment
  namespace: azure.mgmt.frontdoor
  package-name: azure-mgmt-frontdoor
  debug: false
  cmd-override:
    "^.*frontdoor.*$": "-"
    "^.*[/]networkexperimentprofiles([/][^/]*)?$": "networkexperiment profile"
    "^.*[/]networkexperimentprofiles[/].*[/]preconfiguredendpoints[/].*$": "networkexperiment profile preconfiguredendpoint"
    "^.*[/]networkexperimentprofiles[/].*[/]experiments[/]([/][^/]*)?$": "networkexperiment profile experiment"
    "^.*[/]networkexperimentprofiles[/].*[/]experiments[/].*[/]latencyscorecard$": "networkexperiment profile experiment latencyscorecard"
    "^.*[/]networkexperimentprofiles[/].*[/]experiments[/].*[/]timeseries$": "networkexperiment profile experiment timeseries"
  adjustments:
    "/properties/endpointa": "EndpointA_*/"
    "/properties/endpointb": "EndpointB_*/"
  test-setup:
    - name: Create or Update a service with all parameters
```
