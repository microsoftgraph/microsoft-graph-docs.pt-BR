---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44f0a918300ca0beed076e825b1aca4204d0e03b
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522332"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEffectivePermissions = await graphClient.DeviceManagement.VirtualEndpoint
    .GetEffectivePermissions()
    .Request()
    .GetAsync();

```