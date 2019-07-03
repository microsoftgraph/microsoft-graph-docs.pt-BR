---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d11d555fcd6d199befbc5969fee0a3859e01908
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465820"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerProgressTaskBoardTaskFormat = new PlannerProgressTaskBoardTaskFormat
{
    OrderHint = "A6673H Ejkl!"
};

await graphClient.Planner.Tasks["{task-id}"].ProgressTaskBoardFormat
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerProgressTaskBoardTaskFormat);

```