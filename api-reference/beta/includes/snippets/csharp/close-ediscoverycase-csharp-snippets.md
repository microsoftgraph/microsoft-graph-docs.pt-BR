---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1952a3b81de55dc826d2b98fb39bd2da294641b8
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095463"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"]
    .Close()
    .Request()
    .PostAsync();

```