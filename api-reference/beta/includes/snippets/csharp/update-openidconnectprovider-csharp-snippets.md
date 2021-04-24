---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd39d7434371aebf1b241c097bec378facae1410
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51987549"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new IdentityProvider
{
    ResponseType = OpenIdConnectResponseTypes.Id_token
};

await graphClient.IdentityProviders["{identityProvider-id}"]
    .Request()
    .UpdateAsync(identityProvider);

```