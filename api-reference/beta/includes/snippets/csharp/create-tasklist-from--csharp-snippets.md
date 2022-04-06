---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1960188abdb81f63c3929e87d2f9fbcf17405dcc
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528000"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var baseTaskList = new TaskList
{
    DisplayName = "Shopping list"
};

await graphClient.Me.Tasks.Lists
    .Request()
    .AddAsync(baseTaskList);

```