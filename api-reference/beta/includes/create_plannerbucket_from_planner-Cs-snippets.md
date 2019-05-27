---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1f49cfe4fc6c0f3bb63b7e7cbcaeb078940d05b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440020"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = new PlannerBucket
{
    Name = "Advertising",
    PlanId = "xqQg5FS2LkCp935s-FIFm2QAFkHM",
    OrderHint = " !"
};

await graphClient.Planner.Buckets
    .Request()
    .AddAsync(plannerBucket);

```