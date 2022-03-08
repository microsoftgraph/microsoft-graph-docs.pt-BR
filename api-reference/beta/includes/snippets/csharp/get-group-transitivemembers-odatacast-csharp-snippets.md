---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de0ba9b211c6f2078822d67ea1759ed220663cd0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var group = await graphClient.Groups["{group-id}"].TransitiveMembers
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```