---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9e0118912b015247682bf6a2dc2882df390e752e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106964"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var baseTask = new BaseTask
{
    Body = new ItemBody
    {
    },
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
    PersonalProperties = new PersonalTaskProperties
    {
    }
};

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"].Tasks["{baseTask-id}"]
    .Request()
    .UpdateAsync(baseTask);

```