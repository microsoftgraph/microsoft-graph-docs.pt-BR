---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1fe41cb8ec2be7ab104e2071409a2b4360dfa04
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413180"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerProgressTaskBoardTaskFormat = await graphClient.Planner.Tasks["{id}"].ProgressTaskBoardFormat
    .Request()
    .GetAsync();

```