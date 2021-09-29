---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5871a0dec2fbf2185ed6252fee106d154fd0bf4c
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996954"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBrandingLocalization = new OrganizationalBrandingLocalization
{
    BackgroundColor = "#00000F",
    Id = "fr-FR",
    SignInPageText = " "
};

await graphClient.Organization["{organization-id}"].Branding.Localizations
    .Request()
    .AddAsync(organizationalBrandingLocalization);

```