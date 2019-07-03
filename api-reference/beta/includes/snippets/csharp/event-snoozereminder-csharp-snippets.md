---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e06954ee3c50dee067592fc3b54a523324b3656
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newReminderTime = new DateTimeTimeZone
{
    DateTime = "2016-10-19T10:37:00Z",
    TimeZone = "timeZone-value"
};

await graphClient.Me.Events["{id}"]
    .SnoozeReminder(newReminderTime)
    .Request()
    .PostAsync();

```