---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb496ff4dfaea9167c89e949aafaaad30e383a60
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286366"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = new SocialIdentityProvider
{
    DisplayName = "Apple"
};

await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .UpdateAsync(identityProviderBase);

```