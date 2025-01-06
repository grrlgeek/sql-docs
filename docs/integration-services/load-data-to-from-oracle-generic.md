---
title: "Load data from or into Oracle database"
description: Learn how to load data from or into Oracle database
author: chugugrace
ms.author: chugu
ms.date: 01/06/2025
ms.service: sql
ms.subservice: integration-services
ms.topic: conceptual
ms.custom: intro-deployment
---

# Load data from or into Oracle database

This document focuses on how to export data from and load data into Oracle data database.

## Install Oracle Client

First, download [the latest Oracle Client for Microsoft Tools](https://www.oracle.com/technetwork/database/windows/downloads/index-090165.html) and install Oracle client.

> [!NOTE]
> Installing both 32-bit and 64-bit versions together may cause compatibility issues. Please install only one version.

## Configure ADO.NET connection manager

1. Create ADO.NET connection for Oracle connection
1. Choose .Net Providers\OracleClient Data Provider, then enter server name, username and password.

:::image type="content" source="media/load-data-to-from-oracle-generic/connection-manager.png" alt-text="connection-manager":::

For details, see [ADO.NET connection manager](connection-manager/ado-net-connection-manager.md).

## Configure ADO.NET Source

Export data using the ADO NET source. For details, see [ADO NET Source](data-flow/ado-net-source.md).

:::image type="content" source="media/load-data-to-from-oracle-generic/ado-source.png" alt-text="ado.net source":::

## Configure ADO.NET Destination

Use ADO NET destination loads data into ADO.NET-compliant databases. For details, see [ADO NET Destination](data-flow/ado-net-destination.md).

:::image type="content" source="media/load-data-to-from-oracle-generic/ado-destination.png" alt-text="ado.net destination":::