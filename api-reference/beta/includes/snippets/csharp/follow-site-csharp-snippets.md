---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9d5546c3a7ef5f5ea7cf9fbb3b96270c67211e1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<Site>()
{
    new Site
    {
        Id = "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740"
    },
    new Site
    {
        Id = "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851"
    }
};

await graphClient.Users["{user-id}"].FollowedSites
    .Add(value)
    .Request()
    .PostAsync();

```