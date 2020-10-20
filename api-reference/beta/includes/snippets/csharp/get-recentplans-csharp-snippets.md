---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 622bd3336eb4ecd100b23df4741a07a89fa2ec6e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622409"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recentPlans = await graphClient.Me.Planner.RecentPlans
    .Request()
    .GetAsync();

```