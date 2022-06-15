---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 948a99a2ca5c05a36dbc2d264df88bcea644ad40
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryReviewSet = new Microsoft.Graph.Security.EdiscoveryReviewSet
{
    DisplayName = "My review set 2"
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets
    .Request()
    .AddAsync(ediscoveryReviewSet);

```