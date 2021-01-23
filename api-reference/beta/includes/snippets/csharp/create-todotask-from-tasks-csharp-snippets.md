---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a15fb2158af849adf4426dd570e3dbf797e4a822
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945313"
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

await graphClient.Me.Todo.Lists["AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM"].Tasks
    .Request()
    .AddAsync(todoTask);

```