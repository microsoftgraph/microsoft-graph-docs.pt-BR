---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed5ad649f88816228ec9d092d5f3c3104b7b8410
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092337"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"]
    .Release()
    .Request()
    .PostAsync();

```