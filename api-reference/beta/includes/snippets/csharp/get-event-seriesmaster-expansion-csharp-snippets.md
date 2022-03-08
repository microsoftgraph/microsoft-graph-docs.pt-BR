---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f304af6244b9f915a9186ba2659148e07badaa33
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["{event-id}"]
    .Request()
    .Expand("exceptionOccurrences,cancelledOccurrences")
    .Select("subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences")
    .GetAsync();

```