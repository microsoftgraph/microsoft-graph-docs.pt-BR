---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7edfaeee6d7a796156cac4a536d502308478e2a
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policies = await graphClient.Identity.ConditionalAccess.Policies
    .Request()
    .GetAsync();

```