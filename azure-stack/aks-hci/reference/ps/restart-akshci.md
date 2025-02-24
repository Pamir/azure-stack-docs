---
title: Restart-AksHci for AKS on Azure Stack HCI
author: mattbriggs
description: The Restart-AksHci PowerShell command restarts AKS on Azure Stack HCI and removes all deployed Kubernetes clusters.
ms.topic: reference
ms.date: 2/12/2021
ms.author: mabrigg 
ms.lastreviewed: 1/14/2022
ms.reviewer: jeguan

---

# Restart-AksHci

## Synopsis
Restart Azure Kubernetes Service on Azure Stack HCI and remove all deployed Kubernetes clusters.

## Syntax

### Restart AKS-HCI
```powershell
Restart-AksHci
```

## Description
Restarting Azure Kubernetes Service on Azure Stack HCI will remove all of your Kubernetes clusters if any, and the Azure Kubernetes Service host. It will also uninstall the Azure Kubernetes Service on Azure Stack HCI agents and services from the nodes. It will then go back through the original install process steps until the host is recreated. The Azure Kubernetes Service on Azure Stack HCI configuration that you configured via Set-AksHciConfig and the downloaded VHDX images are preserved.

## Examples

### Example
```powershell
Restart-AksHci
```

## Next steps

[AksHci PowerShell Reference](index.md)