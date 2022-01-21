---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d480473a794074d168b5cae9fa4f42c4b3953e3e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy
{
    DisplayName = "HR provisioning policy",
    Description = "Provisioning policy for India HR employees",
    OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701b553"
};

await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{cloudPcProvisioningPolicy-id}"]
    .Request()
    .UpdateAsync(cloudPcProvisioningPolicy);

```