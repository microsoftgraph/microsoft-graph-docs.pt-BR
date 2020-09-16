---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 413dcc805bda1c64c7211701e5027a2d3ea69b8a
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843132"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTaskList = new TodoTaskList
{
    DisplayName = "Travel items"
};

await graphClient.Me.Todo.Lists
    .Request()
    .AddAsync(todoTaskList);

```