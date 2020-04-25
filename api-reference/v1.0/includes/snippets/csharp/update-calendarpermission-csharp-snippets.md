---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6da481dff5a46e6723d163ca8d7f0ae02cbf103
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = new CalendarPermission
{
    Role = CalendarRoleType.Write
};

await graphClient.Users["{id}"].Calendar.CalendarPermissions["RGVmYXVsdA=="]
    .Request()
    .UpdateAsync(calendarPermission);

```