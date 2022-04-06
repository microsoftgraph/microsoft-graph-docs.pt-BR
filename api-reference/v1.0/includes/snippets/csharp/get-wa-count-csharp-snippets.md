---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e452dcd3eeb2648429de65a11c9c2ced857ae96
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528022"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var users = await graphClient.Users
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:wa")
    .OrderBy("displayName")
    .GetAsync();

```