---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86efc57b97e44dcbecdf24b0cb62500105daf0e3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351129"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var users = await graphClient.Users
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:wa")
    .OrderBy("displayName")
    .GetAsync();

```