---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da130ceaf7edd12dc8d62f5458b6513e61508cb2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473009"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new MicrosoftAuthenticatorAuthenticationMethodConfiguration
{
    State = AuthenticationMethodState.Enabled
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["microsoftAuthenticator"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```