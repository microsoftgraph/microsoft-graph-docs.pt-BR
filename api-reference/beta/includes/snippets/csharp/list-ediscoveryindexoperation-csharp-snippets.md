---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1000e281cd1c39ac8387d0ca74bebc1fcc02c6fd
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095973"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryIndexOperation = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"].LastIndexOperation
    .Request()
    .GetAsync();

```