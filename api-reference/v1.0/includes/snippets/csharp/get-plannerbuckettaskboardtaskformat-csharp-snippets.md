---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8769ff563d6da859708eb1b95974ff0a4b9bd78
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucketTaskBoardTaskFormat = await graphClient.Planner.Tasks["{task-id}"].BucketTaskBoardFormat
    .Request()
    .GetAsync();

```