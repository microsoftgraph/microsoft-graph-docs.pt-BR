---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24fcf4b0b905a8105e68c2a454269e1c1fcd4c66
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776330"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new EmailAuthenticationMethodConfiguration
{
    AllowExternalIdToUseEmailOtp = ExternalEmailOtpState.Default
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```