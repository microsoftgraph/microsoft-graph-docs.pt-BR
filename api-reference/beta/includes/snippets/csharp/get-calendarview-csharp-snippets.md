---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7274e072411cfd5039f59132bba8a7676e469632992e34532b7efa58a315c13b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2017-01-01T19:00:00-08:00"),
    new QueryOption("endDateTime", "2017-01-07T19:00:00-08:00")
};

var calendarView = await graphClient.Me.Calendar.CalendarView
    .Request( queryOptions )
    .GetAsync();

```