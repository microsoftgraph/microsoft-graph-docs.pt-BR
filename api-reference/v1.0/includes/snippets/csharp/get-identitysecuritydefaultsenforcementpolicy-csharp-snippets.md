---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea045579040f086b73207651afd7c686934faf44
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567270"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identitySecurityDefaultsEnforcementPolicy = await graphClient.Policies.IdentitySecurityDefaultsEnforcementPolicy
    .Request()
    .GetAsync();

```