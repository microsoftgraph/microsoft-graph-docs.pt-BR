---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25ac27c9234b9033063b8688db8ee7751330979f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096238"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryCase = new Microsoft.Graph.Security.EdiscoveryCase
{
    DisplayName = "My Case 1 - Renamed",
    Description = "Updated description"
};

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"]
    .Request()
    .UpdateAsync(ediscoveryCase);

```