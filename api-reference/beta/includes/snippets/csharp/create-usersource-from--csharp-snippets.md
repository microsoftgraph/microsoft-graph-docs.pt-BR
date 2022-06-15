---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28ce07ebb85562a7f28a95b1ab33ff56cd85e26e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095161"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSource = new Microsoft.Graph.Security.UserSource
{
    Email = "admin@M365x809305.onmicrosoft.com",
    IncludedSources = Microsoft.Graph.Security.SourceType.Mailbox | Microsoft.Graph.Security.SourceType.Site
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"].UserSources
    .Request()
    .AddAsync(userSource);

```