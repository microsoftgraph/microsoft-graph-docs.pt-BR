---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15544d3ee2905dc4729d0cbce91c7651fb15b56f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802262"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```