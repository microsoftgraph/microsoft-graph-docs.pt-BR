---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aaa6bf759d8d127f39bda95fd5ae3858ce46075c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434410"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = new Calendar
{
    Name = "name-value",
    Color = new CalendarColor
    {
    }
};

await graphClient.Me.CalendarGroups["{id}"].Calendars
    .Request()
    .AddAsync(calendar);

```