---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c15f7d080253824eb51a657dbdfe9cf2209d54c2
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521513"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{id}"]
    .Request()
    .Expand("assignments")
    .GetAsync();

```