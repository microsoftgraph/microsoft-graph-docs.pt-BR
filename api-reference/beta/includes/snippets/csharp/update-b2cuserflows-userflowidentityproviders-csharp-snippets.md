---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8bbcf37903b20c430502c5ed768db1acd84f34d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368805"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowIdentityProviders = new IdentityProvider
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/identity/identityProviders/{id}"}
    }
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserFlowIdentityProviders.References
    .Request()
    .UpdateAsync(userFlowIdentityProviders);

```