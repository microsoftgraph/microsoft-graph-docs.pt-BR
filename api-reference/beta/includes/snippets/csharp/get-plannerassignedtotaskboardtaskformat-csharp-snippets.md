---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 390734bc47bfe0e4674a11913a5a15200bbef100ff8c01f418f5b1e71c93e982
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217383"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerAssignedToTaskBoardTaskFormat = await graphClient.Planner.Tasks["{plannerTask-id}"].AssignedToTaskBoardFormat
    .Request()
    .GetAsync();

```