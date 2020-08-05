---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4b98ac931c4eeb4442d1309e1530536004453e44
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566799"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityProviders["{id}"]
    .Request()
    .DeleteAsync();

```