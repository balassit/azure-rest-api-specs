# Microsoft Purview
    
> see https://aka.ms/autorest

This is the AutoRest configuration file for Purview Insights Service.



---
## Getting Started 
To build the SDK for Insights, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information 
These are the global settings for the Microsoft Purview Insights API.

``` yaml
openapi-type: data-plane
tag: package-2022-03-01-preview
```


### Tag: package-2022-03-01-preview

These settings apply only when `--tag=package-2022-03-01-preview` is specified on the command line.

``` yaml $(tag) == 'package-2022-03-01-preview'
input-file:
- preview/2022-03-01-preview/purviewinsights.json
```

---
# Code Generation

## C# 

These settings apply only when `--csharp` is specified on the command line.
Please also specify `--csharp-sdks-folder=<path to "SDKs" directory of your azure-sdk-for-net clone>`.

``` yaml $(csharp)
csharp:
  add-credentials: true
  sync-methods: all
  namespace: Microsoft.Azure.Babylon.ReportingClient
  output-folder: $(csharp-sdks-folder)/generated_csharp
  clear-output-folder: true
```
