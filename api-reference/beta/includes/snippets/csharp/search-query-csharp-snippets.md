---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 161260aa63d830d049e857c29f86a95b4b088b4b
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48317960"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var requests = new List<SearchRequestObject>()
{
    new SearchRequestObject
    {
        EntityTypes = new List<EntityType>()
        {
            EntityType.ExternalItem
        },
        ContentSources = new List<String>()
        {
            "/external/connections/connectionfriendlyname"
        },
        Query = new SearchQuery
        {
            QueryString = "contoso product"
        },
        From = 0,
        Size = 25,
        Fields = new List<String>()
        {
            "title",
            "description"
        }
    }
};

await graphClient.Search
    .Query(requests)
    .Request()
    .PostAsync();

```