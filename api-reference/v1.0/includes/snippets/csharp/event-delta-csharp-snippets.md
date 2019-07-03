---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76caed15644c6173cd57aa364afde0bbd0cf3266
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startdatetime", "{start_datetime}"),
    new QueryOption("enddatetime", "{end_datetime}")
};

var delta = await graphClient.Me.CalendarView.Delta()
    .Request( queryOptions )
    .GetAsync();

```