---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6048eecf0c23655bed7937281e3e121feac6d5b499ae433c71944535d73a9c09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = new CalendarPermission
{
    Role = CalendarRoleType.Write
};

await graphClient.Users["{user-id}"].Calendar.CalendarPermissions["{calendarPermission-id}"]
    .Request()
    .UpdateAsync(calendarPermission);

```