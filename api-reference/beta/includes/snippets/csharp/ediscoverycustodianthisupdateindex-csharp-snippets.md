---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24186dcba90b691a64a941e87529745ae13c7490
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095214"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"]
    .UpdateIndex()
    .Request()
    .PostAsync();

```