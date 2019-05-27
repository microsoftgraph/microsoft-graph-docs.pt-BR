---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12065c13a0c7e6ba103025ff3cd6cc28bb8c43fc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454822"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlan = await graphClient.Planner.Plans["{plan-id}"]
    .Request()
    .GetAsync();

```