---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80b00009f2ef570a03f9325ac5170b463f5b3fb8486b551d7f8954e83ba65a9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326829"
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