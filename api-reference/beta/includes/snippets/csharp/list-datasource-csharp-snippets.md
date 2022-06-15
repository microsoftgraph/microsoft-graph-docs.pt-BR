---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36751b9a45e199291f5f43234a1dacc725efb7bb
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094358"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodianSources = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"].CustodianSources
    .Request()
    .GetAsync();

```