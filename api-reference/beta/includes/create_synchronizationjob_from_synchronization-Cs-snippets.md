---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6660f4cd63959c9c24ecae1a688bf9cede5ff29
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439509"
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