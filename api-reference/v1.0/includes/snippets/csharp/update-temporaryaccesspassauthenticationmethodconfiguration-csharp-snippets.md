---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 303b155675471cddcc54fb6e5e2898a873a058a7
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437737"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new TemporaryAccessPassAuthenticationMethodConfiguration
{
    IsUsableOnce = true
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```