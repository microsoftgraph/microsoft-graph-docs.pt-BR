---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1230c6068cffa349efc52a24317e79b5f42b84bf
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093878"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var run = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].ReviewSets["{security.ediscoveryReviewSet-id}"].Queries["{security.ediscoveryReviewSetQuery-id}"]
    .Run()
    .Request()
    .GetAsync();

```