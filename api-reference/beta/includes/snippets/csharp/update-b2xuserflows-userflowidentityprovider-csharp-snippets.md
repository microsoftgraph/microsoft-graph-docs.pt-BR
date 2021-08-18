---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c18c89ebfdfa50c0e49c84544a93ebd75b942b02
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowIdentityProviders = new IdentityProvider
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test"}
    }
};

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserFlowIdentityProviders.References
    .Request()
    .UpdateAsync(userFlowIdentityProviders);

```