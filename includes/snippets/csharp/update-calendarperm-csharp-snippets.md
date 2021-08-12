---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0b765fb5586ff0f2adf898ccb5872d0c8afa5c169cdc7b987d7c3fddaae74b2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = new CalendarPermission
{
    Role = CalendarRoleType.Write
};

await graphClient.Users["AlexW@contoso.OnMicrosoft.com"].Calendars["AAMkADAwAABf02bAAAA="].CalendarPermissions["L289RXhjaGFuZ2VMYWJQWRlbGVW"]
    .Request()
    .UpdateAsync(calendarPermission);

```