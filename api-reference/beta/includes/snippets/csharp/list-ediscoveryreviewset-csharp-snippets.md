---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9687732e8ece5b298e7223f8856111e0b9ecfc3c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093801"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSets = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets
    .Request()
    .GetAsync();

```