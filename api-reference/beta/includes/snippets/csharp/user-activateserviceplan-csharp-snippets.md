---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 254f4df7f68680ebef983d6b5e109138d579f176
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775034"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePlanId = Guid.Parse("28f42d6f-8034-4a0f-9d8a-a218a63b3299");

var skuId = Guid.Parse("465a2a90-5e59-456d-a7b8-127b9fb2e484");

await graphClient.Me
    .ActivateServicePlan(servicePlanId,skuId)
    .Request()
    .PostAsync();

```