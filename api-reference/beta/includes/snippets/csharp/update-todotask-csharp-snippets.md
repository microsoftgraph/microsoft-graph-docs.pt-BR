---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 363bbe856e5f98f509bf29048d9a9608a0753d24e668467c01fde90629351473
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275534"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var todoTask = new TodoTask
{
    DueDateTime = new DateTimeTimeZone
    {
        DateTime = "2020-07-25T16:00:00",
        TimeZone = "Eastern Standard Time"
    }
};

await graphClient.Me.Todo.Lists["{todoTaskList-id}"].Tasks["{todoTask-id}"]
    .Request()
    .UpdateAsync(todoTask);

```