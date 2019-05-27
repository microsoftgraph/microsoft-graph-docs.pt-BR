---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab63d70b639c3a4b5ff83bf207f9a41f6d0c7e05
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTaskDetails = await graphClient.Planner.Tasks["{task-id}"].Details
    .Request()
    .GetAsync();

```