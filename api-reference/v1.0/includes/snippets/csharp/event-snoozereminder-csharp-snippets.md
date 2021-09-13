---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f06466453f0b118dddf13fb0bbe3c97dc4444d611655356d2c723ad564a83099
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215109"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var newReminderTime = new DateTimeTimeZone
{
    DateTime = "dateTime-value",
    TimeZone = "timeZone-value"
};

await graphClient.Me.Events["{event-id}"]
    .SnoozeReminder(newReminderTime)
    .Request()
    .PostAsync();

```