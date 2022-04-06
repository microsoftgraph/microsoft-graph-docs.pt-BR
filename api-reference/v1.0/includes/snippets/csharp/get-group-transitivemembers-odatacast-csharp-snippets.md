---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a663cfd9b2c3dddc3488f07a4dafb8d1cb198dcb
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63527983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var group = await graphClient.Groups["{group-id}"].TransitiveMembers
    .Request( queryOptions )
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```