---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c04da6bf8b4d26a015dcc3377787508dc4a700f1
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63527934"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var baseTask = new Task
{
    TextBody = "String",
    BodyLastModifiedDateTime = DateTimeOffset.Parse("String (timestamp)"),
    CompletedDateTime = DateTimeOffset.Parse("String (timestamp)"),
    DueDateTime = new DateTimeTimeZone
    {
    },
    StartDateTime = new DateTimeTimeZone
    {
    },
    Importance = Importance.Low,
    Recurrence = new PatternedRecurrence
    {
    },
    DisplayName = "String",
    Status = TaskStatus_v2.NotStarted,
    Viewpoint = new TaskViewpoint
    {
    }
};

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks
    .Request()
    .AddAsync(baseTask);

```