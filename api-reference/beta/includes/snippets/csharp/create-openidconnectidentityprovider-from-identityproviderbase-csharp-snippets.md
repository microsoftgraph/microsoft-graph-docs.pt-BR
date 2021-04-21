---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9cfe618722c2bd4450eb9773657fc3ef6c30caba
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = new OpenIdConnectIdentityProvider
{
    DisplayName = "Login with the Contoso identity provider",
    ClientId = "56433757-cadd-4135-8431-2c9e3fd68ae8",
    ClientSecret = "12345",
    ClaimsMapping = new ClaimsMapping
    {
        UserId = "myUserId",
        GivenName = "myGivenName",
        Surname = "mySurname",
        Email = "myEmail",
        DisplayName = "myDisplayName"
    },
    DomainHint = "mycustomoidc",
    MetadataUrl = "https://mycustomoidc.com/.well-known/openid-configuration",
    ResponseMode = OpenIdConnectResponseMode.Form_post,
    ResponseType = OpenIdConnectResponseTypes.Code,
    Scope = "openid"
};

await graphClient.Identity.IdentityProviders
    .Request()
    .AddAsync(identityProviderBase);

```