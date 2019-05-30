---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76caed15644c6173cd57aa364afde0bbd0cf3266
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34535893"
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