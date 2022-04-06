---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 468a6fa800455339cc0fe5bf44ec97391e882c28
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63527986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var servicePrincipals = await graphClient.ServicePrincipals
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Team")
    .GetAsync();

```