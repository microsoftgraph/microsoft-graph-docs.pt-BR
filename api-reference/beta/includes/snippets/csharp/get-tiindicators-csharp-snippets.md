---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4ffe7448a8c5cd1e8294f5a0cb77349837bb7e04
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518907"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicators = await graphClient.Security.TiIndicators
    .Request()
    .GetAsync();

```