---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad32763535781755c3883aa1110b55eb75aa29be
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    OriginalStartTimeZone = "originalStartTimeZone-value",
    OriginalEndTimeZone = "originalEndTimeZone-value",
    ResponseStatus = new ResponseStatus
    {
        Response = ResponseType.None,
        Time = "datetime-value"
    },
    Uid = "iCalUId-value",
    ReminderMinutesBeforeStart = 99,
    IsReminderOn = true
};

await graphClient.Groups["{id}"].Events["{id}"]
    .Request()
    .UpdateAsync(@event);

```