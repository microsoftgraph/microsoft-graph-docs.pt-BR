---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1e21b26803998071d6fc2699959dab6ad97d741cc174d3aef69aa85ee799c438
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSetQuery = new Microsoft.Graph.Ediscovery.ReviewSetQuery
{
    DisplayName = "My Query 1",
    Query = "(subject:\"Quarterly Financials\")"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].ReviewSets["{ediscovery.reviewSet-id}"].Queries
    .Request()
    .AddAsync(reviewSetQuery);

```