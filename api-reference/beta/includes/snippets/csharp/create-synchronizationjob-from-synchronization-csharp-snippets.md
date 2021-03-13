---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91558ecb5b3d0c37ea11664851b730899f361b4a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationJob = new SynchronizationJob
{
    TemplateId = "BoxOutDelta"
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs
    .Request()
    .AddAsync(synchronizationJob);

```