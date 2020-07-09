## TypeScript

These settings apply only when `--typescript` is specified on the command line.
Please also specify `--typescript-sdks-folder=<path to root folder of your azure-sdk-for-js clone>`.

``` yaml $(typescript)
typescript:
  azure-arm: true
  package-name: "@azure/synapse"
  output-folder: "$(typescript-sdks-folder)/sdk/synapse/synapse"
  generate-metadata: true
batch:
  - package-spark: true
  - package-artifacts: true
  - package-access-control: true
```