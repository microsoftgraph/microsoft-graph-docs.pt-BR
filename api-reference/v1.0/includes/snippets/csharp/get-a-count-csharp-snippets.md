---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4291fc43853f7a462210b5b67547ec5094f820a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336351"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("$count", "true")
};

var contacts = await graphClient.Contacts
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("startswith(displayName,'A')")
    .OrderBy("displayName")
    .Top(1)
    .GetAsync();

```