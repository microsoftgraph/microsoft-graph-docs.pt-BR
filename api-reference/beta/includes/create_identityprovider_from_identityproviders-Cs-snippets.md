---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 268f21e78095874ec41dfa63d0bed37e825961c6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480677"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new IdentityProvider
{
    Name = "Login with Amazon",
    Type = "Amazon",
    ClientId = "56433757-cadd-4135-8431-2c9e3fd68ae8",
    ClientSecret = "000000000000"
};

await graphClient.IdentityProviders
    .Request()
    .AddAsync(identityProvider);

```