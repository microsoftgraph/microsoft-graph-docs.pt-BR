---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4e6690495432c5bfc5f6b940d64cf0467cae30006814b1c0846496b28a03f223
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    ClientId = "clientId-value",
    ConsentType = "consentType-value",
    PrincipalId = "principalId-value",
    ResourceId = "resourceId-value",
    Scope = "scope-value",
    StartTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    ExpiryTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z")
};

await graphClient.Oauth2PermissionGrants
    .Request()
    .AddAsync(oAuth2PermissionGrant);

```