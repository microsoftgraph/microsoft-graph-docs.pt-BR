---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba4f6e4122a93055e2bc5a910e74850334276f59
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521485"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{id}"]
    .Request()
    .DeleteAsync();

```