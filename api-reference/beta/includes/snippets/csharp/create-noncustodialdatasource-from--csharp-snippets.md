---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20649078c41dd2201ec5fb1003ef3492d6aea433
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266907"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var noncustodialDataSource = new Microsoft.Graph.Ediscovery.NoncustodialDataSource
{
    ApplyHoldToSource = true,
    DataSource = new UserSource
    {
        Email = "adelev@contoso.com"
    }
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].NoncustodialDataSources
    .Request()
    .AddAsync(noncustodialDataSource);

```