---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35010135767e4c663396ef1d3872c7a41cd122e8
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095566"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"]
    .ApplyHold()
    .Request()
    .PostAsync();

```