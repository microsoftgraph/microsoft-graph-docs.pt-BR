---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9912355f20a6ba80374f022bb3e055ecf6e274b0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435344"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new IdentityProvider
{
    ClientSecret = "1111111111111"
};

await graphClient.IdentityProviders["Amazon-OAuth"]
    .Request()
    .UpdateAsync(identityProvider);

```