---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61960b8cbf9c60013608ecbcf75010ed78baccaf
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758809"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    Scope = "User.ReadBasic.All Group.ReadWrite.All"
};

await graphClient.Oauth2PermissionGrants["{oAuth2PermissionGrant-id}"]
    .Request()
    .UpdateAsync(oAuth2PermissionGrant);

```