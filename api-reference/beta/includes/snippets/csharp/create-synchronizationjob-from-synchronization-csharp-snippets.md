---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6660f4cd63959c9c24ecae1a688bf9cede5ff29
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463284"
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