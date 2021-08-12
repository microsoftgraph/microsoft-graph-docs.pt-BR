---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68f52234866e1bd22872ba7778207531637a79b9bd40fd4f8bf8fb100eee5f6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54177823"
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