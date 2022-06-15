---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4718952546ae0b22d2047f3cab5f7e2564e8d72e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094804"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var asHierarchy = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Tags
    .AsHierarchy()
    .Request()
    .GetAsync();

```