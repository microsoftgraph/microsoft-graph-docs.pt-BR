---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c85554b6678748011fbb1ec07bed999272f8b7a7
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTask = new TodoTask
{
    Title = "A new task",
    Categories = new List<String>()
    {
        "Important"
    },
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