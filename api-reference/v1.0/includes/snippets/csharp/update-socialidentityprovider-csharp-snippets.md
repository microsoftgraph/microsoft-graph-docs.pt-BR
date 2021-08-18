---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d627a0457d98d1064191142f56ef561b602feb1a152893050e9e93ef391bf93f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = new SocialIdentityProvider
{
    ClientSecret = "1111111111111"
};

await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .UpdateAsync(identityProviderBase);

```