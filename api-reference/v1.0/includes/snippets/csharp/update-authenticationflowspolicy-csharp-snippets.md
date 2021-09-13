---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f785b6838a4d5f3d3c326bee7b977e24c705b3d8a30ba2dc2d0a0dc28ad671f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329186"
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