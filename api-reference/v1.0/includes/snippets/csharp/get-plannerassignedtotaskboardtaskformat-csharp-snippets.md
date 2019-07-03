---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcdadfc1f0ecea66573573b9e0ae02da33c3dfc6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerAssignedToTaskBoardTaskFormat = await graphClient.Planner.Tasks["{task-id}"].AssignedToTaskBoardFormat
    .Request()
    .GetAsync();

```