---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2470784d6e6e7e9006c4bbe80dec5a59dd4a17b0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTask = new TodoTask
{
    Title = "A new task",
    LinkedResources = new TodoTaskLinkedResourcesCollectionPage()
    {
        new LinkedResource
        {
            WebUrl = "http://microsoft.com",
            ApplicationName = "Microsoft",
            DisplayName = "Microsoft"
        }
    }
};

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks
    .Request()
    .AddAsync(todoTask);

```