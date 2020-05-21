---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5e153299ab1d594cb8149523d9f1c076e8c4ee2
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334481"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    ClientId = "clientId-value",
    ConsentType = "consentType-value",
    PrincipalId = "principalId-value",
    ResourceId = "resourceId-value",
    Scope = "scope-value"
};

await graphClient.Oauth2PermissionGrants
    .Request()
    .AddAsync(oAuth2PermissionGrant);

```