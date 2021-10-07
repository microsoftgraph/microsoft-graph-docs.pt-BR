---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78895f0b61d034c8cc2909c6aafca72840b339144516d3a8a1af775490d66930
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327824"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new MicrosoftAuthenticatorAuthenticationMethodConfiguration
{
    State = AuthenticationMethodState.Enabled
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```