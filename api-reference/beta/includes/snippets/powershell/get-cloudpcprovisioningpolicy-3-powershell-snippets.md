---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 708438978368e1421d2b6f75456f0605ff3f262f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440571"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

Get-MgDeviceManagementVirtualEndpointProvisioningPolicy -CloudPcProvisioningPolicyId $cloudPcProvisioningPolicyId -Property "id,description,displayName,displayName,domainJoinConfiguration,imageDisplayName,imageId,imageType,onPremisesConnectionId,windowsSettings,managedBy,cloudPcGroupDisplayName,gracePeriodInHours,localAdminEnabled,alternateResourceUrl" 

```