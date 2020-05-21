---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d21df060f3c9e52241685ade7b7ce82225c05213
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332845"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var microsoft.graph.group = await graphClient.Users["{id}"].TransitiveMemberOf.Microsoft.graph.group
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:tier")
    .Select( e => new {
             e.DisplayName,
             e.Id 
             })
    .OrderBy("displayName ")
    .GetAsync();

```