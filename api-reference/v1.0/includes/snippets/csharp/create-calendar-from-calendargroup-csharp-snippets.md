---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a880c3e8bc48526fea17430970a02ce1cd03ced0
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753982"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = new Calendar
{
    Name = "Marketing calendar"
};

await graphClient.Me.CalendarGroups["AAMkADYAAAR9NR5AAA="].Calendars
    .Request()
    .AddAsync(calendar);

```