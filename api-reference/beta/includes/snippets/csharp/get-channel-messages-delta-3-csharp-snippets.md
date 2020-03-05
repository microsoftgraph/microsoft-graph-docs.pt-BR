---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d1b7d3ed60d3a11348983a700d49439dc2f4aed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$skiptoken", "c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA=")
};

var delta = await graphClient.Teams["{id}"].Channels["{id}"].Messages
    .Delta()
    .Request()
    .GetAsync();

```