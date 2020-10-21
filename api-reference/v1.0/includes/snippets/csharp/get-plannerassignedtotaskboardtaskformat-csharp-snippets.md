---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcdadfc1f0ecea66573573b9e0ae02da33c3dfc6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerAssignedToTaskBoardTaskFormat = await graphClient.Planner.Tasks["{task-id}"].AssignedToTaskBoardFormat
    .Request()
    .GetAsync();

```