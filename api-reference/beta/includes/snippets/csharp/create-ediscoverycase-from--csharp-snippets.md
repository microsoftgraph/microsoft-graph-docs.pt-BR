---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a8a843b4d568c615c2ab89578facc7f6d26601b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryCase = new Microsoft.Graph.Security.EdiscoveryCase
{
    DisplayName = "CONTOSO LITIGATION-005",
    Description = "Project Bazooka",
    ExternalId = "324516"
};

await graphClient.Security.Cases.EdiscoveryCases
    .Request()
    .AddAsync(ediscoveryCase);

```