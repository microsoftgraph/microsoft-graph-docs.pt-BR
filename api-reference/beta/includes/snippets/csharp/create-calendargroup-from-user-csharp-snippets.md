---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50119211e5d2a8361a5fd95bc8f9b1fc453e5359f5203698cbc7b3bfd203c9c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375876"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = new CalendarGroup
{
    Name = "Personal events"
};

await graphClient.Me.CalendarGroups
    .Request()
    .AddAsync(calendarGroup);

```