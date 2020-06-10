---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70dd474188648d37d1311f61fdbf008f229d1f29
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680875"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationFlowsPolicy = new AuthenticationFlowsPolicy
{
    SelfServiceSignUp = new SelfServiceSignUpAuthenticationFlowConfiguration
    {
        IsEnabled = true
    }
};

await graphClient.Policies.AuthenticationFlowsPolicy
    .Request()
    .UpdateAsync(authenticationFlowsPolicy);

```