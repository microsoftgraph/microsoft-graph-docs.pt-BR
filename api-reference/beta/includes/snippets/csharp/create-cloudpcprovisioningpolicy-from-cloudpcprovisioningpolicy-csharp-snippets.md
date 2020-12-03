---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae3f88ae2cd2f75b9f27389845a141eae1a951e7
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523166"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy
{
    DisplayName = "Display Name value",
    Description = "Description value",
    OnPremisesConnectionId = "6bf90392-5fea-459a-9e9d-a2484abbffff",
    ImageId = "Image ID value",
    ImageDisplayName = "Image Display Name value",
    ImageType = CloudPcProvisioningPolicyImageType.Gallery
};

await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies
    .Request()
    .AddAsync(cloudPcProvisioningPolicy);

```