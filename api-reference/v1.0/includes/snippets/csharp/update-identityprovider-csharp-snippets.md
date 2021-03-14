---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75fd397b237775e400c5163e9750599ab599407c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800675"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new IdentityProvider
{
    ClientSecret = "1111111111111"
};

await graphClient.IdentityProviders["{identityProvider-id}"]
    .Request()
    .UpdateAsync(identityProvider);

```