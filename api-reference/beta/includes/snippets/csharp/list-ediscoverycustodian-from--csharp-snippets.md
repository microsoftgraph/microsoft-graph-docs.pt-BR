---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7bd70a298ae1f8037d0e993b69ce7961f8a578a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092092"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var custodians = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians
    .Request()
    .GetAsync();

```