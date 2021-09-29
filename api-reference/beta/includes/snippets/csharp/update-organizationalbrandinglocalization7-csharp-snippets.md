---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 375e39bdc8dcd3aef25236ba82e23af33f51bba6
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996549"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBrandingLocalization = new OrganizationalBrandingLocalization
{
    SignInPageText = "Welcome to Contoso France.",
    UsernameHintText = " "
};

await graphClient.Organization["{organization-id}"].Branding.Localizations["{organizationalBrandingLocalization-id}"]
    .Request()
    .UpdateAsync(organizationalBrandingLocalization);

```