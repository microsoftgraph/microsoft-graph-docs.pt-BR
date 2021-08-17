---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3c7d2be3df5a73dd1b1555de85f63d3a1c167e99
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368813"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = new SocialIdentityProvider
{
    ClientSecret = "1111111111111"
};

await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .UpdateAsync(identityProviderBase);

```