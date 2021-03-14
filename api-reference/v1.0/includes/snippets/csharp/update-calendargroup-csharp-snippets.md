---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35794038dce2113011340f0aa801c054c0f1c00f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarGroup = new CalendarGroup
{
    Name = "name-value"
};

await graphClient.Me.CalendarGroups["{calendarGroup-id}"]
    .Request()
    .UpdateAsync(calendarGroup);

```