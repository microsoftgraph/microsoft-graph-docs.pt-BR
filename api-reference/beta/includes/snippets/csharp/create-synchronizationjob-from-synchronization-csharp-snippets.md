---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6660f4cd63959c9c24ecae1a688bf9cede5ff29
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612069"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationJob = new SynchronizationJob
{
    TemplateId = "BoxOutDelta"
};

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs
    .Request()
    .AddAsync(synchronizationJob);

```