---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37dd6350563c2449bfe71fa7fb05baadcd77d9c0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerProgressTaskBoardTaskFormat = await graphClient.Planner.Tasks["{task-id}"].ProgressTaskBoardFormat
    .Request()
    .GetAsync();

```