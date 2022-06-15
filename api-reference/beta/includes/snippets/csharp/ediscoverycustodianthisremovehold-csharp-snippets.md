---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86501a54322e952cd85536f412d6dcd77e5356c1
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093753"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"]
    .RemoveHold()
    .Request()
    .PostAsync();

```