---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d87f012945cf940faf8a875ee5103d9a6264dab
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844376"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xIdentityUserFlow = new B2xIdentityUserFlow
{
    Id = "UserFlowWithAPIConnector",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 1f,
    ApiConnectorConfiguration = new UserFlowApiConnectorConfiguration
    {
        PostFederationSignup = new IdentityApiConnector
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.id", "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"}
            }
        },
        PostAttributeCollection = new IdentityApiConnector
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"@odata.id", "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"}
            }
        }
    }
};

await graphClient.Identity.B2xUserFlows
    .Request()
    .AddAsync(b2xIdentityUserFlow);

```