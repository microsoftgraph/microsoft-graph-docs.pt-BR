---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48031f2e1195b5265dddaa61d03d51b1226d61d9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches["{security.ediscoverySearch-id}"].NoncustodialSources["{security.ediscoveryNoncustodialDataSource-id}"].Reference
    .Request()
    .DeleteAsync();

```