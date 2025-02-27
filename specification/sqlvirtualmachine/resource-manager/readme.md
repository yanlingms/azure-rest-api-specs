# SQL virtual machine

> see https://aka.ms/autorest

This is the AutoRest configuration file for SQL virtual machine.

---

## Getting Started

To build the SDK for SQL virtual machine, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`

---

## Configuration

### Basic Information

These are the global settings for the SQL virtual machine API.

``` yaml
title: SqlVirtualMachineManagementClient
description: 'The SQL virtual machine management API provides a RESTful set of web APIs that interact with Azure Compute, Network & Storage services to manage your SQL Server virtual machine. The API enables users to create, delete and retrieve a SQL virtual machine, SQL virtual machine group or availability group listener.'
openapi-type: arm
tag: package-2022-02
```


### Tag: package-2022-02

These settings apply only when `--tag=package-2022-02` is specified on the command line.

```yaml $(tag) == 'package-2022-02'
input-file:
  - Microsoft.SqlVirtualMachine/stable/2022-02-01/sqlvm.json
```

### Tag: package-preview-2022-02

These settings apply only when `--tag=package-preview-2022-02` is specified on the command line.

```yaml $(tag) == 'package-preview-2022-02'
input-file:
  - Microsoft.SqlVirtualMachine/preview/2022-02-01-preview/sqlvm.json
```


### Tag: package-preview-2021-11

These settings apply only when `--tag=package-preview-2021-11` is specified on the command line.

``` yaml $(tag) == 'package-preview-2021-11'
input-file:
  - Microsoft.SqlVirtualMachine/preview/2021-11-01-preview/sqlvm.json
```

### Tag: package-2017-03-01-preview

These settings apply only when `--tag=package-2017-03-01-preview` is specified on the command line.

``` yaml $(tag) == 'package-2017-03-01-preview'
input-file:
- Microsoft.SqlVirtualMachine/preview/2017-03-01-preview/sqlvm.json
```

---

# Code Generation

## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

``` yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-net
  - repo: azure-sdk-for-python-track2
  - repo: azure-sdk-for-go
  - repo: azure-sdk-for-java
  - repo: azure-resource-manager-schemas
  - repo: azure-powershell
```

### C#

These settings apply only when `--csharp` is specified on the command line.
Please also specify `--csharp-sdks-folder=<path to "SDKs" directory of your azure-sdk-for-net clone>`.

``` yaml $(csharp)
csharp:
  azure-arm: true
  license-header: MICROSOFT_MIT_NO_VERSION
  namespace: Microsoft.Azure.Management.SqlVirtualMachine
  output-folder: $(csharp-sdks-folder)/sqlvirtualmachine/Microsoft.Azure.Management.SqlVirtualMachine/src/Generated
  clear-output-folder: true
```

## Python

See configuration in [readme.python.md](./readme.python.md)

### Go

See configuration in [readme.go.md](./readme.go.md)

### Java

See configuration in [readme.java.md](./readme.java.md)
