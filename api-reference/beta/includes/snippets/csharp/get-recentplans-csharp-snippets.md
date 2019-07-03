---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 622bd3336eb4ecd100b23df4741a07a89fa2ec6e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498249"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recentPlans = await graphClient.Me.Planner.RecentPlans
    .Request()
    .GetAsync();

```