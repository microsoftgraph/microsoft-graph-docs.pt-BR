---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 496da082dc65ce137f57333713623d97f674f4c17e58d4cf92eb8dbb1bf66ca4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendarPermission = await graphClient.Users["{user-id}"].Calendar.CalendarPermissions["{calendarPermission-id}"]
    .Request()
    .GetAsync();

```