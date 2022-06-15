---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0dc0d47c25a8fb236032f98ee77fab658927d3ed
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094167"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var operations = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Operations
    .Request()
    .GetAsync();

```