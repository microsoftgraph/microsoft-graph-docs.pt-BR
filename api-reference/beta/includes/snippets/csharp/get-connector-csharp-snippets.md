---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ace122f6f003b68b9786ef4961949bdbb17ea89e
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printConnector = await graphClient.Print.Connectors["{id}"]
    .Request()
    .GetAsync();

```