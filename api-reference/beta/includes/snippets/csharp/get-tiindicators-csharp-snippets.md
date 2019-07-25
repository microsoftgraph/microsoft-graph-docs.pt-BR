---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4ffe7448a8c5cd1e8294f5a0cb77349837bb7e04
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724445"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicators = await graphClient.Security.TiIndicators
    .Request()
    .GetAsync();

```