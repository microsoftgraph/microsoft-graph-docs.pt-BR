---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 107d171d56a61ba46bad32d9ca98ec082daa11d7
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095349"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Tags["{security.ediscoveryReviewTag-id}"]
    .Request()
    .DeleteAsync();

```