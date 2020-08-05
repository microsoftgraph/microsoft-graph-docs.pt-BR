---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6814d998bb18a644bab0e0dc3bed995017667147
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566939"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ediscoveryCase = new EdiscoveryCase
{
    DisplayName = "My Case 1"
};

await graphClient.Compliance.Ediscovery.Cases
    .Request()
    .AddAsync(ediscoveryCase);

```