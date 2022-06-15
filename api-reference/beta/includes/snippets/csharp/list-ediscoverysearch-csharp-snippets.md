---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e15e681db3ad121002426dd1b5a56dc32429a43
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092883"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var searches = await graphClient.Security.Cases.EdiscoveryCases["{security.ediscoveryCase-id}"].Searches
    .Request()
    .GetAsync();

```