---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1e33c16cad17404fdfb2c21b7be11a648deb9ced
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42536529"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$skiptoken", "R0usmcCM996atia_s")
};

var delta = await graphClient.Me.CalendarView
    .Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .GetAsync();

```