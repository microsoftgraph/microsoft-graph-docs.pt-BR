---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7501c0af4746217b2235ffa632db9b557bd7e0d9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472420"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new PasswordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
{
    State = AuthenticationMethodState.Enabled
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["passwordlessMicrosoftAuthenticator"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```