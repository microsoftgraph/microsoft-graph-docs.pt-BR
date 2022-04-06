---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24e1ef00b4e42f357422bf6602dca42804bf4315
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63527938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var applications = await graphClient.Applications
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Web")
    .GetAsync();

```