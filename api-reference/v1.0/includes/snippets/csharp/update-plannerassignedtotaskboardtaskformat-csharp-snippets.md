---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c009cb4a608c14a3fab0a81891ecd290251cb3ea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerAssignedToTaskBoardTaskFormat = new PlannerAssignedToTaskBoardTaskFormat
{
    OrderHintsByAssignee = new PlannerOrderHintsByAssignee
    {
        Aaa27244-1db4-476a-a5cb-004607466324 = "8566473P 957764Jk!"
    }
};

await graphClient.Planner.Tasks["{task-id}"].AssignedToTaskBoardFormat
    .Request()
    .Header("If-Match","W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"")
    .UpdateAsync(plannerAssignedToTaskBoardTaskFormat);

```