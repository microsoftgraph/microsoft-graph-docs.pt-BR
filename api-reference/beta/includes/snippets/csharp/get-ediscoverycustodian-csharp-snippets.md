---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f10e499d07c3ee370af71b6dd86b276f6e3e6873
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryCustodian = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Custodians["{security.ediscoveryCustodian-id}"]
    .Request()
    .GetAsync();

```