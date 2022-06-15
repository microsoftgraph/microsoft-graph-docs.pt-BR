---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6fce4b6816082c978bdf5f37be0cfdce3b1f47a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092489"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].LegalHolds["{security.ediscoveryHoldPolicy-id}"]
    .Request()
    .DeleteAsync();

```