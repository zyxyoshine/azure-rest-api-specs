## Python

These settings apply only when `--python` is specified on the command line.
Please also specify `--python-sdks-folder=<path to the root directory of your azure-sdk-for-python clone>`.
Use `--python-mode=update` if you already have a setup.py and just want to update the code itself.

``` yaml $(python)
python:
  azure-arm: true
  license-header: MICROSOFT_MIT_NO_VERSION
  payload-flattening-threshold: 2
  package-version: 0.1.0
  clear-output-folder: true
batch:
  - package-migrate: true
  - package-offazure: true
```

``` yaml $(python) && $(package-migrate)
python:
  namespace: azure.mgmt.migrate
  package-name: azure-mgmt-migrate
  basic-setup-py: true
  output-folder: $(python-sdks-folder)/migrate/azure-mgmt-migrate
```

``` yaml $(python) && $(package-offazure)
python:
  namespace: azure.mgmt.offazure
  package-name: azure-mgmt-migrate
  basic-setup-py: true
  output-folder: $(python-sdks-folder)/offazure/azure-mgmt-offazure
```