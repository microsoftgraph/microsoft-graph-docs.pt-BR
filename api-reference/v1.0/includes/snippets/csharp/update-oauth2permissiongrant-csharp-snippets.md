---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd7ae49cb47c57f362dcbb88d5ebcce7ec0b9a83
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    Scope = "scope-value"
};

await graphClient.Oauth2PermissionGrants["{oAuth2PermissionGrant-id}"]
    .Request()
    .UpdateAsync(oAuth2PermissionGrant);

```