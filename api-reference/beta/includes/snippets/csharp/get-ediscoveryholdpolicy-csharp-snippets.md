---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e42cf6e1b06fd41c2990531785584cccb3ec044a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092945"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryHoldPolicy = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].LegalHolds["{security.ediscoveryHoldPolicy-id}"]
    .Request()
    .GetAsync();

```