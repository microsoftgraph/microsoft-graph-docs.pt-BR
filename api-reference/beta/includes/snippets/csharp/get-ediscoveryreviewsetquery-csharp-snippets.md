---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d73cff55c9d6f17bfacbdd516de1452ffc865fce
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095431"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryReviewSetQuery = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets["{security.ediscoveryReviewSet-id}"].Queries["{security.ediscoveryReviewSetQuery-id}"]
    .Request()
    .GetAsync();

```