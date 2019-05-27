---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0210192cdc78a4319d8fb5937cb5c27058dbd750
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicy = new GroupLifecyclePolicy
{
    GroupLifetimeInDays = 100,
    ManagedGroupTypes = "Selected",
    AlternateNotificationEmails = "admin@contoso.com"
};

await graphClient.GroupLifecyclePolicies
    .Request()
    .AddAsync(groupLifecyclePolicy);

```