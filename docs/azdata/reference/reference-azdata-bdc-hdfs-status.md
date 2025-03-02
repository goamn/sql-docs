---
title: azdata bdc hdfs status reference
titleSuffix: SQL Server big data clusters
description: Reference article for azdata bdc hdfs status commands.
author: MikeRayMSFT
ms.author: mikeray
ms.reviewer: seanw
ms.date: 04/06/2021
ms.topic: reference
ms.prod: sql
ms.technology: big-data-cluster
---

# azdata bdc hdfs status

Applies to [!INCLUDE [azure-data-cli-azdata](../../includes/azure-data-cli-azdata.md)]

The following article provides reference for the **sql** commands in the **azdata** tool. For more information about other **azdata** commands, see [azdata reference](reference-azdata.md)

## Commands

|Command|Description|
| --- | --- |
[azdata bdc hdfs status show](#azdata-bdc-hdfs-status-show) | Hdfs service status.
## azdata bdc hdfs status show
Hdfs service status.
```bash
azdata bdc hdfs status show [--resource -r] 
                            [--all -a]
```
### Examples
Get status of hdfs service.
```bash
azdata bdc hdfs status show
```
Get status of hdfs service with all instances.
```bash
azdata bdc hdfs status show --all
```
Get status of the storage resource within the hdfs service.
```bash
azdata bdc hdfs status show --resource storage-0
```
### Optional Parameters
#### `--resource -r`
Get this resource in this service.
#### `--all -a`
Show all the instances of each resource within the service.
### Global Arguments
#### `--debug`
Increase logging verbosity to show all debug logs.
#### `--help -h`
Show this help message and exit.
#### `--output -o`
Output format.  Allowed values: json, jsonc, table, tsv.  Default: json.
#### `--query -q`
JMESPath query string. See [http://jmespath.org/](http://jmespath.org) for more information and examples.
#### `--verbose`
Increase logging verbosity. Use --debug for full debug logs.

## Next steps

For more information about other **azdata** commands, see [azdata reference](reference-azdata.md). 

For more information about how to install the **azdata** tool, see [Install azdata](..\install\deploy-install-azdata.md).

